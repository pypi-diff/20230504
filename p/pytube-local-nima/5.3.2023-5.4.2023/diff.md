# Comparing `tmp/pytube_local_nima-5.3.2023.tar.gz` & `tmp/pytube_local_nima-5.4.2023.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytube_local_nima-5.3.2023.tar", last modified: Wed May  3 21:48:01 2023, max compression
+gzip compressed data, was "dist/pytube_local_nima-5.4.2023.tar", last modified: Thu May  4 00:51:02 2023, max compression
```

## Comparing `pytube_local_nima-5.3.2023.tar` & `pytube_local_nima-5.4.2023.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 nima       (501) staff       (20)        0 2023-05-03 21:48:01.000000 pytube_local_nima-5.3.2023/
--rw-r--r--   0 nima       (501) staff       (20)     5995 2023-05-03 21:48:01.000000 pytube_local_nima-5.3.2023/PKG-INFO
--rw-r--r--   0 nima       (501) staff       (20)     1211 2023-05-03 20:08:10.000000 pytube_local_nima-5.3.2023/LICENSE
-drwxr-xr-x   0 nima       (501) staff       (20)        0 2023-05-03 21:48:01.000000 pytube_local_nima-5.3.2023/pytube/
--rw-r--r--   0 nima       (501) staff       (20)    11654 2023-05-03 20:32:44.000000 pytube_local_nima-5.3.2023/pytube/innertube.py
--rw-r--r--   0 nima       (501) staff       (20)    15288 2023-05-03 20:32:44.000000 pytube_local_nima-5.3.2023/pytube/streams.py
--rw-r--r--   0 nima       (501) staff       (20)     1482 2023-05-03 20:32:44.000000 pytube_local_nima-5.3.2023/pytube/metadata.py
--rw-r--r--   0 nima       (501) staff       (20)       76 2023-05-03 21:04:35.000000 pytube_local_nima-5.3.2023/pytube/version.py
--rw-r--r--   0 nima       (501) staff       (20)      451 2023-05-03 20:32:44.000000 pytube_local_nima-5.3.2023/pytube/monostate.py
--rw-r--r--   0 nima       (501) staff       (20)    12844 2023-05-03 20:32:44.000000 pytube_local_nima-5.3.2023/pytube/query.py
--rw-r--r--   0 nima       (501) staff       (20)     8512 2023-05-03 20:32:44.000000 pytube_local_nima-5.3.2023/pytube/request.py
--rw-r--r--   0 nima       (501) staff       (20)      592 2023-05-03 20:32:44.000000 pytube_local_nima-5.3.2023/pytube/__init__.py
-drwxr-xr-x   0 nima       (501) staff       (20)        0 2023-05-03 21:48:01.000000 pytube_local_nima-5.3.2023/pytube/contrib/
--rw-r--r--   0 nima       (501) staff       (20)     6576 2023-05-03 20:32:44.000000 pytube_local_nima-5.3.2023/pytube/contrib/channel.py
--rw-r--r--   0 nima       (501) staff       (20)        0 2023-05-03 20:32:44.000000 pytube_local_nima-5.3.2023/pytube/contrib/__init__.py
--rw-r--r--   0 nima       (501) staff       (20)    14204 2023-05-03 20:32:44.000000 pytube_local_nima-5.3.2023/pytube/contrib/playlist.py
--rw-r--r--   0 nima       (501) staff       (20)     8886 2023-05-03 20:32:44.000000 pytube_local_nima-5.3.2023/pytube/contrib/search.py
--rw-r--r--   0 nima       (501) staff       (20)     5931 2023-05-03 20:32:44.000000 pytube_local_nima-5.3.2023/pytube/parser.py
--rw-r--r--   0 nima       (501) staff       (20)    22529 2023-05-03 20:32:44.000000 pytube_local_nima-5.3.2023/pytube/cipher.py
--rwxr-xr-x   0 nima       (501) staff       (20)    16635 2023-05-03 20:32:44.000000 pytube_local_nima-5.3.2023/pytube/cli.py
--rw-r--r--   0 nima       (501) staff       (20)     4311 2023-05-03 20:32:44.000000 pytube_local_nima-5.3.2023/pytube/itags.py
--rw-r--r--   0 nima       (501) staff       (20)     3907 2023-05-03 20:32:44.000000 pytube_local_nima-5.3.2023/pytube/exceptions.py
--rw-r--r--   0 nima       (501) staff       (20)     5648 2023-05-03 20:32:44.000000 pytube_local_nima-5.3.2023/pytube/captions.py
--rw-r--r--   0 nima       (501) staff       (20)     9794 2023-05-03 20:32:44.000000 pytube_local_nima-5.3.2023/pytube/helpers.py
--rw-r--r--   0 nima       (501) staff       (20)    17798 2023-05-03 20:32:44.000000 pytube_local_nima-5.3.2023/pytube/extract.py
--rw-r--r--   0 nima       (501) staff       (20)    15423 2023-05-03 20:32:44.000000 pytube_local_nima-5.3.2023/pytube/__main__.py
-drwxr-xr-x   0 nima       (501) staff       (20)        0 2023-05-03 21:48:01.000000 pytube_local_nima-5.3.2023/tests/
--rw-r--r--   0 nima       (501) staff       (20)     1406 2023-05-03 20:08:10.000000 pytube_local_nima-5.3.2023/tests/test_parser.py
--rw-r--r--   0 nima       (501) staff       (20)    13696 2023-05-03 20:08:10.000000 pytube_local_nima-5.3.2023/tests/test_streams.py
--rw-r--r--   0 nima       (501) staff       (20)     2736 2023-05-03 20:08:10.000000 pytube_local_nima-5.3.2023/tests/test_cipher.py
--rw-r--r--   0 nima       (501) staff       (20)     4921 2023-05-03 20:08:10.000000 pytube_local_nima-5.3.2023/tests/conftest.py
--rw-r--r--   0 nima       (501) staff       (20)      276 2023-05-03 20:08:10.000000 pytube_local_nima-5.3.2023/tests/test_itags.py
--rw-r--r--   0 nima       (501) staff       (20)     1820 2023-05-03 20:08:10.000000 pytube_local_nima-5.3.2023/tests/test_request.py
--rw-r--r--   0 nima       (501) staff       (20)      498 2023-05-03 20:08:10.000000 pytube_local_nima-5.3.2023/tests/test_metadata.py
--rw-r--r--   0 nima       (501) staff       (20)     3452 2023-05-03 20:08:10.000000 pytube_local_nima-5.3.2023/tests/test_exceptions.py
--rw-r--r--   0 nima       (501) staff       (20)       57 2023-05-03 20:08:10.000000 pytube_local_nima-5.3.2023/tests/__init__.py
-drwxr-xr-x   0 nima       (501) staff       (20)        0 2023-05-03 21:48:01.000000 pytube_local_nima-5.3.2023/tests/contrib/
--rw-r--r--   0 nima       (501) staff       (20)     3122 2023-05-03 20:08:10.000000 pytube_local_nima-5.3.2023/tests/contrib/test_channel.py
--rw-r--r--   0 nima       (501) staff       (20)    11623 2023-05-03 20:08:10.000000 pytube_local_nima-5.3.2023/tests/contrib/test_playlist.py
--rw-r--r--   0 nima       (501) staff       (20)     6148 2023-05-03 20:08:10.000000 pytube_local_nima-5.3.2023/tests/test_query.py
--rw-r--r--   0 nima       (501) staff       (20)     5024 2023-05-03 20:08:10.000000 pytube_local_nima-5.3.2023/tests/test_helpers.py
--rw-r--r--   0 nima       (501) staff       (20)     2957 2023-05-03 20:08:10.000000 pytube_local_nima-5.3.2023/tests/test_extract.py
--rw-r--r--   0 nima       (501) staff       (20)    17295 2023-05-03 20:08:10.000000 pytube_local_nima-5.3.2023/tests/test_cli.py
--rw-r--r--   0 nima       (501) staff       (20)     1915 2023-05-03 20:08:10.000000 pytube_local_nima-5.3.2023/tests/test_main.py
--rw-r--r--   0 nima       (501) staff       (20)     5759 2023-05-03 20:08:10.000000 pytube_local_nima-5.3.2023/tests/test_captions.py
--rw-r--r--   0 nima       (501) staff       (20)       55 2023-05-03 20:08:10.000000 pytube_local_nima-5.3.2023/MANIFEST.in
--rw-r--r--   0 nima       (501) staff       (20)     4054 2023-05-03 21:37:12.000000 pytube_local_nima-5.3.2023/README.md
-drwxr-xr-x   0 nima       (501) staff       (20)        0 2023-05-03 21:48:01.000000 pytube_local_nima-5.3.2023/pytube_local_nima.egg-info/
--rw-r--r--   0 nima       (501) staff       (20)     5995 2023-05-03 21:48:01.000000 pytube_local_nima-5.3.2023/pytube_local_nima.egg-info/PKG-INFO
--rw-r--r--   0 nima       (501) staff       (20)        1 2023-05-03 21:48:01.000000 pytube_local_nima-5.3.2023/pytube_local_nima.egg-info/zip-safe
--rw-r--r--   0 nima       (501) staff       (20)     1069 2023-05-03 21:48:01.000000 pytube_local_nima-5.3.2023/pytube_local_nima.egg-info/SOURCES.txt
--rw-r--r--   0 nima       (501) staff       (20)       55 2023-05-03 21:48:01.000000 pytube_local_nima-5.3.2023/pytube_local_nima.egg-info/entry_points.txt
--rw-r--r--   0 nima       (501) staff       (20)        7 2023-05-03 21:48:01.000000 pytube_local_nima-5.3.2023/pytube_local_nima.egg-info/top_level.txt
--rw-r--r--   0 nima       (501) staff       (20)        1 2023-05-03 21:48:01.000000 pytube_local_nima-5.3.2023/pytube_local_nima.egg-info/dependency_links.txt
--rwxr-xr-x   0 nima       (501) staff       (20)     1871 2023-05-03 21:38:46.000000 pytube_local_nima-5.3.2023/setup.py
--rw-r--r--   0 nima       (501) staff       (20)       38 2023-05-03 21:48:01.000000 pytube_local_nima-5.3.2023/setup.cfg
+drwxr-xr-x   0 nima       (501) staff       (20)        0 2023-05-04 00:51:02.000000 pytube_local_nima-5.4.2023/
+-rw-r--r--   0 nima       (501) staff       (20)     5995 2023-05-04 00:51:02.000000 pytube_local_nima-5.4.2023/PKG-INFO
+-rw-r--r--   0 nima       (501) staff       (20)     1211 2023-05-03 20:08:10.000000 pytube_local_nima-5.4.2023/LICENSE
+drwxr-xr-x   0 nima       (501) staff       (20)        0 2023-05-04 00:51:02.000000 pytube_local_nima-5.4.2023/pytube/
+-rw-r--r--   0 nima       (501) staff       (20)    15772 2023-05-04 00:45:23.000000 pytube_local_nima-5.4.2023/pytube/innertube.py
+-rw-r--r--   0 nima       (501) staff       (20)    15288 2023-05-03 20:32:44.000000 pytube_local_nima-5.4.2023/pytube/streams.py
+-rw-r--r--   0 nima       (501) staff       (20)     1482 2023-05-03 20:32:44.000000 pytube_local_nima-5.4.2023/pytube/metadata.py
+-rw-r--r--   0 nima       (501) staff       (20)       76 2023-05-04 00:48:00.000000 pytube_local_nima-5.4.2023/pytube/version.py
+-rw-r--r--   0 nima       (501) staff       (20)      451 2023-05-03 20:32:44.000000 pytube_local_nima-5.4.2023/pytube/monostate.py
+-rw-r--r--   0 nima       (501) staff       (20)    12844 2023-05-03 20:32:44.000000 pytube_local_nima-5.4.2023/pytube/query.py
+-rw-r--r--   0 nima       (501) staff       (20)     8656 2023-05-04 00:46:22.000000 pytube_local_nima-5.4.2023/pytube/request.py
+-rw-r--r--   0 nima       (501) staff       (20)      592 2023-05-03 20:32:44.000000 pytube_local_nima-5.4.2023/pytube/__init__.py
+drwxr-xr-x   0 nima       (501) staff       (20)        0 2023-05-04 00:51:02.000000 pytube_local_nima-5.4.2023/pytube/contrib/
+-rw-r--r--   0 nima       (501) staff       (20)     6576 2023-05-03 20:32:44.000000 pytube_local_nima-5.4.2023/pytube/contrib/channel.py
+-rw-r--r--   0 nima       (501) staff       (20)        0 2023-05-03 20:32:44.000000 pytube_local_nima-5.4.2023/pytube/contrib/__init__.py
+-rw-r--r--   0 nima       (501) staff       (20)    14204 2023-05-03 20:32:44.000000 pytube_local_nima-5.4.2023/pytube/contrib/playlist.py
+-rw-r--r--   0 nima       (501) staff       (20)     8886 2023-05-03 20:32:44.000000 pytube_local_nima-5.4.2023/pytube/contrib/search.py
+-rw-r--r--   0 nima       (501) staff       (20)     5931 2023-05-03 20:32:44.000000 pytube_local_nima-5.4.2023/pytube/parser.py
+-rw-r--r--   0 nima       (501) staff       (20)    22529 2023-05-03 20:32:44.000000 pytube_local_nima-5.4.2023/pytube/cipher.py
+-rwxr-xr-x   0 nima       (501) staff       (20)    16635 2023-05-03 20:32:44.000000 pytube_local_nima-5.4.2023/pytube/cli.py
+-rw-r--r--   0 nima       (501) staff       (20)     4311 2023-05-03 20:32:44.000000 pytube_local_nima-5.4.2023/pytube/itags.py
+-rw-r--r--   0 nima       (501) staff       (20)     3907 2023-05-03 20:32:44.000000 pytube_local_nima-5.4.2023/pytube/exceptions.py
+-rw-r--r--   0 nima       (501) staff       (20)     5648 2023-05-03 20:32:44.000000 pytube_local_nima-5.4.2023/pytube/captions.py
+-rw-r--r--   0 nima       (501) staff       (20)     9794 2023-05-03 20:32:44.000000 pytube_local_nima-5.4.2023/pytube/helpers.py
+-rw-r--r--   0 nima       (501) staff       (20)    17798 2023-05-03 20:32:44.000000 pytube_local_nima-5.4.2023/pytube/extract.py
+-rw-r--r--   0 nima       (501) staff       (20)    15423 2023-05-03 20:32:44.000000 pytube_local_nima-5.4.2023/pytube/__main__.py
+drwxr-xr-x   0 nima       (501) staff       (20)        0 2023-05-04 00:51:02.000000 pytube_local_nima-5.4.2023/tests/
+-rw-r--r--   0 nima       (501) staff       (20)     1406 2023-05-03 20:08:10.000000 pytube_local_nima-5.4.2023/tests/test_parser.py
+-rw-r--r--   0 nima       (501) staff       (20)    13696 2023-05-04 00:49:52.000000 pytube_local_nima-5.4.2023/tests/test_streams.py
+-rw-r--r--   0 nima       (501) staff       (20)     2736 2023-05-03 20:08:10.000000 pytube_local_nima-5.4.2023/tests/test_cipher.py
+-rw-r--r--   0 nima       (501) staff       (20)     4921 2023-05-03 20:08:10.000000 pytube_local_nima-5.4.2023/tests/conftest.py
+-rw-r--r--   0 nima       (501) staff       (20)      276 2023-05-03 20:08:10.000000 pytube_local_nima-5.4.2023/tests/test_itags.py
+-rw-r--r--   0 nima       (501) staff       (20)     1820 2023-05-03 20:08:10.000000 pytube_local_nima-5.4.2023/tests/test_request.py
+-rw-r--r--   0 nima       (501) staff       (20)      498 2023-05-03 20:08:10.000000 pytube_local_nima-5.4.2023/tests/test_metadata.py
+-rw-r--r--   0 nima       (501) staff       (20)     3452 2023-05-03 20:08:10.000000 pytube_local_nima-5.4.2023/tests/test_exceptions.py
+-rw-r--r--   0 nima       (501) staff       (20)       57 2023-05-03 20:08:10.000000 pytube_local_nima-5.4.2023/tests/__init__.py
+drwxr-xr-x   0 nima       (501) staff       (20)        0 2023-05-04 00:51:02.000000 pytube_local_nima-5.4.2023/tests/contrib/
+-rw-r--r--   0 nima       (501) staff       (20)     3122 2023-05-03 20:08:10.000000 pytube_local_nima-5.4.2023/tests/contrib/test_channel.py
+-rw-r--r--   0 nima       (501) staff       (20)    11623 2023-05-03 20:08:10.000000 pytube_local_nima-5.4.2023/tests/contrib/test_playlist.py
+-rw-r--r--   0 nima       (501) staff       (20)     6148 2023-05-03 20:08:10.000000 pytube_local_nima-5.4.2023/tests/test_query.py
+-rw-r--r--   0 nima       (501) staff       (20)     5024 2023-05-03 20:08:10.000000 pytube_local_nima-5.4.2023/tests/test_helpers.py
+-rw-r--r--   0 nima       (501) staff       (20)     2957 2023-05-03 20:08:10.000000 pytube_local_nima-5.4.2023/tests/test_extract.py
+-rw-r--r--   0 nima       (501) staff       (20)    17295 2023-05-03 20:08:10.000000 pytube_local_nima-5.4.2023/tests/test_cli.py
+-rw-r--r--   0 nima       (501) staff       (20)     1915 2023-05-03 20:08:10.000000 pytube_local_nima-5.4.2023/tests/test_main.py
+-rw-r--r--   0 nima       (501) staff       (20)     5759 2023-05-03 20:08:10.000000 pytube_local_nima-5.4.2023/tests/test_captions.py
+-rw-r--r--   0 nima       (501) staff       (20)       55 2023-05-03 20:08:10.000000 pytube_local_nima-5.4.2023/MANIFEST.in
+-rw-r--r--   0 nima       (501) staff       (20)     4054 2023-05-03 21:37:12.000000 pytube_local_nima-5.4.2023/README.md
+drwxr-xr-x   0 nima       (501) staff       (20)        0 2023-05-04 00:51:02.000000 pytube_local_nima-5.4.2023/pytube_local_nima.egg-info/
+-rw-r--r--   0 nima       (501) staff       (20)     5995 2023-05-04 00:51:02.000000 pytube_local_nima-5.4.2023/pytube_local_nima.egg-info/PKG-INFO
+-rw-r--r--   0 nima       (501) staff       (20)        1 2023-05-03 21:48:01.000000 pytube_local_nima-5.4.2023/pytube_local_nima.egg-info/zip-safe
+-rw-r--r--   0 nima       (501) staff       (20)     1069 2023-05-04 00:51:02.000000 pytube_local_nima-5.4.2023/pytube_local_nima.egg-info/SOURCES.txt
+-rw-r--r--   0 nima       (501) staff       (20)       55 2023-05-04 00:51:02.000000 pytube_local_nima-5.4.2023/pytube_local_nima.egg-info/entry_points.txt
+-rw-r--r--   0 nima       (501) staff       (20)        7 2023-05-04 00:51:02.000000 pytube_local_nima-5.4.2023/pytube_local_nima.egg-info/top_level.txt
+-rw-r--r--   0 nima       (501) staff       (20)        1 2023-05-04 00:51:02.000000 pytube_local_nima-5.4.2023/pytube_local_nima.egg-info/dependency_links.txt
+-rwxr-xr-x   0 nima       (501) staff       (20)     1871 2023-05-03 21:38:46.000000 pytube_local_nima-5.4.2023/setup.py
+-rw-r--r--   0 nima       (501) staff       (20)       38 2023-05-04 00:51:02.000000 pytube_local_nima-5.4.2023/setup.cfg
```

### Comparing `pytube_local_nima-5.3.2023/PKG-INFO` & `pytube_local_nima-5.4.2023/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytube_local_nima
-Version: 5.3.2023
+Version: 5.4.2023
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
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytube_local_nima Version: 5.3.2023 Summary: Python
+Metadata-Version: 2.1 Name: pytube_local_nima Version: 5.4.2023 Summary: Python
 3 library for downloading YouTube Videos. Home-page: https://github.com/nbehe/
 pytube_local_nima Author: Nima Beheshti License: The Unlicense (Unlicense)
 Description: # This is a pytube fork created for specific purpose This fork was
 created for the specific purpose of fixing a pytube bug #1594. This fix will be
 used for my specific project. I have not done testing to ensure other
 functionality of the package still work with this change. If you decide to use
 please know their could be issues with the code not working properly going
```

### Comparing `pytube_local_nima-5.3.2023/LICENSE` & `pytube_local_nima-5.4.2023/LICENSE`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-5.3.2023/pytube/streams.py` & `pytube_local_nima-5.4.2023/pytube/streams.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-5.3.2023/pytube/metadata.py` & `pytube_local_nima-5.4.2023/pytube/metadata.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-5.3.2023/pytube/query.py` & `pytube_local_nima-5.4.2023/pytube/query.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-5.3.2023/pytube/request.py` & `pytube_local_nima-5.4.2023/pytube/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,14 @@
     else:
         raise ValueError("Invalid URL")
     return urlopen(request, timeout=timeout)  # nosec
 
 
 def get(url, extra_headers=None, timeout=socket._GLOBAL_DEFAULT_TIMEOUT):
     """Send an http GET request.
-
     :param str url:
         The URL to perform the GET request for.
     :param dict extra_headers:
         Extra headers to add to the request
     :rtype: str
     :returns:
         UTF-8 encoded string of response
@@ -52,15 +51,14 @@
         extra_headers = {}
     response = _execute_request(url, headers=extra_headers, timeout=timeout)
     return response.read().decode("utf-8")
 
 
 def post(url, extra_headers=None, data=None, timeout=socket._GLOBAL_DEFAULT_TIMEOUT):
     """Send an http POST request.
-
     :param str url:
         The URL to perform the POST request for.
     :param dict extra_headers:
         Extra headers to add to the request
     :param dict data:
         The data to send on the POST request
     :rtype: str
@@ -151,17 +149,16 @@
             # If the max retries is exceeded, raise an exception
             if tries >= 1 + max_retries:
                 raise MaxRetriesExceeded()
 
             # Try to execute the request, ignoring socket timeouts
             try:
                 response = _execute_request(
-                    url,
+                    url + f"&range={downloaded}-{stop_pos}",
                     method="GET",
-                    headers={"Range": range_header},
                     timeout=timeout
                 )
             except URLError as e:
                 # We only want to skip over timeout errors, and
                 # raise any other URLError exceptions
                 if isinstance(e.reason, socket.timeout):
                     pass
@@ -173,41 +170,44 @@
             else:
                 # On a successful request, break from loop
                 break
             tries += 1
 
         if file_size == default_range_size:
             try:
-                content_range = response.info()["Content-Range"]
-                file_size = int(content_range.split("/")[1])
+                resp = _execute_request(
+                    url + f"&range={0}-{99999999999}",
+                    method="GET",
+                    timeout=timeout
+                )
+                content_range = resp.info()["Content-Length"]
+                file_size = int(content_range)
             except (KeyError, IndexError, ValueError) as e:
                 logger.error(e)
         while True:
             chunk = response.read()
             if not chunk:
                 break
             downloaded += len(chunk)
             yield chunk
     return  # pylint: disable=R1711
 
 
 @lru_cache()
 def filesize(url):
     """Fetch size in bytes of file at given URL
-
     :param str url: The URL to get the size of
     :returns: int: size in bytes of remote file
     """
     return int(head(url)["content-length"])
 
 
 @lru_cache()
 def seq_filesize(url):
     """Fetch size in bytes of file at given URL from sequential requests
-
     :param str url: The URL to get the size of
     :returns: int: size in bytes of remote file
     """
     total_filesize = 0
     # YouTube expects a request sequence number as part of the parameters.
     split_url = parse.urlsplit(url)
     base_url = '%s://%s/%s?' % (split_url.scheme, split_url.netloc, split_url.path)
@@ -250,16 +250,15 @@
         total_filesize += int(head(url)['content-length'])
         seq_num += 1
     return total_filesize
 
 
 def head(url):
     """Fetch headers returned http GET request.
-
     :param str url:
         The URL to perform the GET request for.
     :rtype: dict
     :returns:
         dictionary of lowercase headers
     """
     response_headers = _execute_request(url, method="HEAD").info()
-    return {k.lower(): v for k, v in response_headers.items()}
+    return {k.lower(): v for k, v in response_headers.items()}
```

### Comparing `pytube_local_nima-5.3.2023/pytube/__init__.py` & `pytube_local_nima-5.4.2023/pytube/__init__.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-5.3.2023/pytube/contrib/channel.py` & `pytube_local_nima-5.4.2023/pytube/contrib/channel.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-5.3.2023/pytube/contrib/playlist.py` & `pytube_local_nima-5.4.2023/pytube/contrib/playlist.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-5.3.2023/pytube/contrib/search.py` & `pytube_local_nima-5.4.2023/pytube/contrib/search.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-5.3.2023/pytube/parser.py` & `pytube_local_nima-5.4.2023/pytube/parser.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-5.3.2023/pytube/cipher.py` & `pytube_local_nima-5.4.2023/pytube/cipher.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-5.3.2023/pytube/cli.py` & `pytube_local_nima-5.4.2023/pytube/cli.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-5.3.2023/pytube/itags.py` & `pytube_local_nima-5.4.2023/pytube/itags.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-5.3.2023/pytube/exceptions.py` & `pytube_local_nima-5.4.2023/pytube/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-5.3.2023/pytube/captions.py` & `pytube_local_nima-5.4.2023/pytube/captions.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-5.3.2023/pytube/helpers.py` & `pytube_local_nima-5.4.2023/pytube/helpers.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-5.3.2023/pytube/extract.py` & `pytube_local_nima-5.4.2023/pytube/extract.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-5.3.2023/pytube/__main__.py` & `pytube_local_nima-5.4.2023/pytube/__main__.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-5.3.2023/tests/test_parser.py` & `pytube_local_nima-5.4.2023/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-5.3.2023/tests/test_streams.py` & `pytube_local_nima-5.4.2023/tests/test_streams.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-5.3.2023/tests/test_cipher.py` & `pytube_local_nima-5.4.2023/tests/test_cipher.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-5.3.2023/tests/conftest.py` & `pytube_local_nima-5.4.2023/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-5.3.2023/tests/test_request.py` & `pytube_local_nima-5.4.2023/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-5.3.2023/tests/test_exceptions.py` & `pytube_local_nima-5.4.2023/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-5.3.2023/tests/contrib/test_channel.py` & `pytube_local_nima-5.4.2023/tests/contrib/test_channel.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-5.3.2023/tests/contrib/test_playlist.py` & `pytube_local_nima-5.4.2023/tests/contrib/test_playlist.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-5.3.2023/tests/test_query.py` & `pytube_local_nima-5.4.2023/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-5.3.2023/tests/test_helpers.py` & `pytube_local_nima-5.4.2023/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-5.3.2023/tests/test_extract.py` & `pytube_local_nima-5.4.2023/tests/test_extract.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-5.3.2023/tests/test_cli.py` & `pytube_local_nima-5.4.2023/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-5.3.2023/tests/test_main.py` & `pytube_local_nima-5.4.2023/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-5.3.2023/tests/test_captions.py` & `pytube_local_nima-5.4.2023/tests/test_captions.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-5.3.2023/README.md` & `pytube_local_nima-5.4.2023/README.md`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-5.3.2023/pytube_local_nima.egg-info/PKG-INFO` & `pytube_local_nima-5.4.2023/pytube_local_nima.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytube-local-nima
-Version: 5.3.2023
+Version: 5.4.2023
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
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytube-local-nima Version: 5.3.2023 Summary: Python
+Metadata-Version: 2.1 Name: pytube-local-nima Version: 5.4.2023 Summary: Python
 3 library for downloading YouTube Videos. Home-page: https://github.com/nbehe/
 pytube_local_nima Author: Nima Beheshti License: The Unlicense (Unlicense)
 Description: # This is a pytube fork created for specific purpose This fork was
 created for the specific purpose of fixing a pytube bug #1594. This fix will be
 used for my specific project. I have not done testing to ensure other
 functionality of the package still work with this change. If you decide to use
 please know their could be issues with the code not working properly going
```

### Comparing `pytube_local_nima-5.3.2023/pytube_local_nima.egg-info/SOURCES.txt` & `pytube_local_nima-5.4.2023/pytube_local_nima.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-5.3.2023/setup.py` & `pytube_local_nima-5.4.2023/setup.py`

 * *Files identical despite different names*

