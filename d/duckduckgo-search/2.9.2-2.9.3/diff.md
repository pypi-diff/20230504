# Comparing `tmp/duckduckgo_search-2.9.2.tar.gz` & `tmp/duckduckgo_search-2.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckduckgo_search-2.9.2.tar", last modified: Tue May  2 21:43:21 2023, max compression
+gzip compressed data, was "duckduckgo_search-2.9.3.tar", last modified: Thu May  4 16:32:07 2023, max compression
```

## Comparing `duckduckgo_search-2.9.2.tar` & `duckduckgo_search-2.9.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:43:21.987956 duckduckgo_search-2.9.2/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-05-02 21:42:59.000000 duckduckgo_search-2.9.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    35682 2023-05-02 21:43:21.987956 duckduckgo_search-2.9.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)    34567 2023-05-02 21:42:59.000000 duckduckgo_search-2.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:43:21.983956 duckduckgo_search-2.9.2/duckduckgo_search/
--rwxr-xr-x   0 runner    (1001) docker     (123)      671 2023-05-02 21:42:59.000000 duckduckgo_search-2.9.2/duckduckgo_search/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      145 2023-05-02 21:42:59.000000 duckduckgo_search-2.9.2/duckduckgo_search/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:43:21.983956 duckduckgo_search-2.9.2/duckduckgo_search/cli/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:42:59.000000 duckduckgo_search-2.9.2/duckduckgo_search/cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10405 2023-05-02 21:42:59.000000 duckduckgo_search-2.9.2/duckduckgo_search/cli/ddgs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6014 2023-05-02 21:42:59.000000 duckduckgo_search-2.9.2/duckduckgo_search/ddg.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2750 2023-05-02 21:42:59.000000 duckduckgo_search-2.9.2/duckduckgo_search/ddg_answers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6246 2023-05-02 21:42:59.000000 duckduckgo_search-2.9.2/duckduckgo_search/ddg_images.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7090 2023-05-02 21:42:59.000000 duckduckgo_search-2.9.2/duckduckgo_search/ddg_maps.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3644 2023-05-02 21:42:59.000000 duckduckgo_search-2.9.2/duckduckgo_search/ddg_news.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1005 2023-05-02 21:42:59.000000 duckduckgo_search-2.9.2/duckduckgo_search/ddg_suggestions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1580 2023-05-02 21:42:59.000000 duckduckgo_search-2.9.2/duckduckgo_search/ddg_translate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3765 2023-05-02 21:42:59.000000 duckduckgo_search-2.9.2/duckduckgo_search/ddg_videos.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3675 2023-05-02 21:42:59.000000 duckduckgo_search-2.9.2/duckduckgo_search/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       22 2023-05-02 21:42:59.000000 duckduckgo_search-2.9.2/duckduckgo_search/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:43:21.983956 duckduckgo_search-2.9.2/duckduckgo_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    35682 2023-05-02 21:43:21.000000 duckduckgo_search-2.9.2/duckduckgo_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-02 21:43:21.000000 duckduckgo_search-2.9.2/duckduckgo_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 21:43:21.000000 duckduckgo_search-2.9.2/duckduckgo_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-02 21:43:21.000000 duckduckgo_search-2.9.2/duckduckgo_search.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-02 21:43:21.000000 duckduckgo_search-2.9.2/duckduckgo_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-02 21:43:21.000000 duckduckgo_search-2.9.2/duckduckgo_search.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-02 21:42:59.000000 duckduckgo_search-2.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 21:43:21.987956 duckduckgo_search-2.9.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:43:21.987956 duckduckgo_search-2.9.2/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1619 2023-05-02 21:42:59.000000 duckduckgo_search-2.9.2/tests/test_ddg.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      994 2023-05-02 21:42:59.000000 duckduckgo_search-2.9.2/tests/test_ddg_answers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2510 2023-05-02 21:42:59.000000 duckduckgo_search-2.9.2/tests/test_ddg_images.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      418 2023-05-02 21:42:59.000000 duckduckgo_search-2.9.2/tests/test_ddg_maps.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1216 2023-05-02 21:42:59.000000 duckduckgo_search-2.9.2/tests/test_ddg_news.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      974 2023-05-02 21:42:59.000000 duckduckgo_search-2.9.2/tests/test_ddg_suggestions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1128 2023-05-02 21:42:59.000000 duckduckgo_search-2.9.2/tests/test_ddg_translate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1325 2023-05-02 21:42:59.000000 duckduckgo_search-2.9.2/tests/test_ddg_videos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:32:07.790330 duckduckgo_search-2.9.3/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-05-04 16:31:47.000000 duckduckgo_search-2.9.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35682 2023-05-04 16:32:07.790330 duckduckgo_search-2.9.3/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34567 2023-05-04 16:31:47.000000 duckduckgo_search-2.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:32:07.790330 duckduckgo_search-2.9.3/duckduckgo_search/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      671 2023-05-04 16:31:47.000000 duckduckgo_search-2.9.3/duckduckgo_search/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      145 2023-05-04 16:31:47.000000 duckduckgo_search-2.9.3/duckduckgo_search/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:32:07.790330 duckduckgo_search-2.9.3/duckduckgo_search/cli/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:31:47.000000 duckduckgo_search-2.9.3/duckduckgo_search/cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10405 2023-05-04 16:31:47.000000 duckduckgo_search-2.9.3/duckduckgo_search/cli/ddgs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6254 2023-05-04 16:31:47.000000 duckduckgo_search-2.9.3/duckduckgo_search/ddg.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2750 2023-05-04 16:31:47.000000 duckduckgo_search-2.9.3/duckduckgo_search/ddg_answers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6457 2023-05-04 16:31:47.000000 duckduckgo_search-2.9.3/duckduckgo_search/ddg_images.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7090 2023-05-04 16:31:47.000000 duckduckgo_search-2.9.3/duckduckgo_search/ddg_maps.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3855 2023-05-04 16:31:47.000000 duckduckgo_search-2.9.3/duckduckgo_search/ddg_news.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1005 2023-05-04 16:31:47.000000 duckduckgo_search-2.9.3/duckduckgo_search/ddg_suggestions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1550 2023-05-04 16:31:47.000000 duckduckgo_search-2.9.3/duckduckgo_search/ddg_translate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3976 2023-05-04 16:31:47.000000 duckduckgo_search-2.9.3/duckduckgo_search/ddg_videos.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3841 2023-05-04 16:31:47.000000 duckduckgo_search-2.9.3/duckduckgo_search/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       22 2023-05-04 16:31:47.000000 duckduckgo_search-2.9.3/duckduckgo_search/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:32:07.790330 duckduckgo_search-2.9.3/duckduckgo_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    35682 2023-05-04 16:32:07.000000 duckduckgo_search-2.9.3/duckduckgo_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-04 16:32:07.000000 duckduckgo_search-2.9.3/duckduckgo_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 16:32:07.000000 duckduckgo_search-2.9.3/duckduckgo_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-04 16:32:07.000000 duckduckgo_search-2.9.3/duckduckgo_search.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-04 16:32:07.000000 duckduckgo_search-2.9.3/duckduckgo_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-04 16:32:07.000000 duckduckgo_search-2.9.3/duckduckgo_search.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-04 16:31:47.000000 duckduckgo_search-2.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 16:32:07.790330 duckduckgo_search-2.9.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:32:07.790330 duckduckgo_search-2.9.3/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1619 2023-05-04 16:31:47.000000 duckduckgo_search-2.9.3/tests/test_ddg.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      994 2023-05-04 16:31:47.000000 duckduckgo_search-2.9.3/tests/test_ddg_answers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2510 2023-05-04 16:31:47.000000 duckduckgo_search-2.9.3/tests/test_ddg_images.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      418 2023-05-04 16:31:47.000000 duckduckgo_search-2.9.3/tests/test_ddg_maps.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1216 2023-05-04 16:31:47.000000 duckduckgo_search-2.9.3/tests/test_ddg_news.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      974 2023-05-04 16:31:47.000000 duckduckgo_search-2.9.3/tests/test_ddg_suggestions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1128 2023-05-04 16:31:47.000000 duckduckgo_search-2.9.3/tests/test_ddg_translate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1325 2023-05-04 16:31:47.000000 duckduckgo_search-2.9.3/tests/test_ddg_videos.py
```

### Comparing `duckduckgo_search-2.9.2/LICENSE.md` & `duckduckgo_search-2.9.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.2/PKG-INFO` & `duckduckgo_search-2.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo_search
-Version: 2.9.2
+Version: 2.9.3
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duckduckgo_search-2.9.2/README.md` & `duckduckgo_search-2.9.3/README.md`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.2/duckduckgo_search/__init__.py` & `duckduckgo_search-2.9.3/duckduckgo_search/__init__.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.2/duckduckgo_search/cli/ddgs.py` & `duckduckgo_search-2.9.3/duckduckgo_search/cli/ddgs.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.2/duckduckgo_search/ddg.py` & `duckduckgo_search-2.9.3/duckduckgo_search/ddg.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,22 @@
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from datetime import datetime
 from time import sleep
 from urllib.parse import unquote
 
 from click import progressbar
 
-from .utils import SESSION, _do_output, _download_file, _get_vqd, _normalize
+from .utils import (
+    SESSION,
+    _do_output,
+    _download_file,
+    _get_vqd,
+    _normalize,
+    _refresh_vqd,
+)
 
 logger = logging.getLogger(__name__)
 
 
 def ddg(
     keywords,
     region="wt-wt",
@@ -39,22 +46,27 @@
     Returns:
         Optional[List[dict]]: DuckDuckGo text search results.
     """
 
     def get_ddg_page(page):
         payload["s"] = max(PAGINATION_STEP * (page - 1), 0)
         page_data = None
-        try:
-            resp = SESSION.get("https://links.duckduckgo.com/d.js", params=payload)
-            resp.raise_for_status()
-            page_data = resp.json().get("results", None)
-        except Exception:
-            logger.exception("")
-            if not max_results:
-                return None
+        for i in range(2):
+            try:
+                resp = SESSION.get("https://links.duckduckgo.com/d.js", params=payload)
+                resp.raise_for_status()
+                page_data = resp.json().get("results", None)
+                break
+            except Exception:
+                logger.exception("")
+                if i == 1 and not max_results:
+                    return None
+                if "506-00.js" in resp.url:
+                    payload["vqd"] = _refresh_vqd(keywords)
+
         page_results = []
         if page_data:
             for row in page_data:
                 if "n" not in row and row["u"] not in cache:
                     cache.add(row["u"])
                     body = _normalize(row["a"])
                     if body:
```

### Comparing `duckduckgo_search-2.9.2/duckduckgo_search/ddg_answers.py` & `duckduckgo_search-2.9.3/duckduckgo_search/ddg_answers.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.2/duckduckgo_search/ddg_images.py` & `duckduckgo_search-2.9.3/duckduckgo_search/ddg_images.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from datetime import datetime
 from time import sleep
 from urllib.parse import unquote
 
 from click import progressbar
 
-from .utils import SESSION, _do_output, _download_file, _get_vqd
+from .utils import SESSION, _do_output, _download_file, _get_vqd, _refresh_vqd
 
 logger = logging.getLogger(__name__)
 
 
 def ddg_images(
     keywords,
     region="wt-wt",
@@ -54,22 +54,27 @@
     Returns:
         Optional[List[dict]]: DuckDuckGo text search results.
     """
 
     def get_ddg_images_page(page):
         payload["s"] = max(PAGINATION_STEP * (page - 1), 0)
         page_data = None
-        try:
-            resp = SESSION.get("https://duckduckgo.com/i.js", params=payload)
-            resp.raise_for_status()
-            page_data = resp.json().get("results", None)
-        except Exception:
-            logger.exception("")
-            if not max_results:
-                return None
+        for i in range(2):
+            try:
+                resp = SESSION.get("https://duckduckgo.com/i.js", params=payload)
+                resp.raise_for_status()
+                page_data = resp.json().get("results", None)
+                break
+            except Exception:
+                logger.exception("")
+                if i == 1 and not max_results:
+                    return None
+                if "506-00.js" in resp.url:
+                    payload["vqd"] = _refresh_vqd(keywords)
+
         page_results = []
         if page_data:
             for row in page_data:
                 if row["image"] not in cache:
                     cache.add(row["image"])
                     page_results.append(
                         {
```

### Comparing `duckduckgo_search-2.9.2/duckduckgo_search/ddg_maps.py` & `duckduckgo_search-2.9.3/duckduckgo_search/ddg_maps.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.2/duckduckgo_search/ddg_news.py` & `duckduckgo_search-2.9.3/duckduckgo_search/ddg_news.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from datetime import datetime
 from time import sleep
 
-from .utils import SESSION, _do_output, _get_vqd, _normalize
+from .utils import SESSION, _do_output, _get_vqd, _normalize, _refresh_vqd
 
 logger = logging.getLogger(__name__)
 
 
 def ddg_news(
     keywords,
     region="wt-wt",
@@ -32,22 +32,27 @@
     Returns:
         Optional[List[dict]]: DuckDuckGo news search results.
     """
 
     def get_ddg_news_page(page):
         payload["s"] = max(PAGINATION_STEP * (page - 1), 0)
         page_data = None
-        try:
-            resp = SESSION.get("https://duckduckgo.com/news.js", params=payload)
-            resp.raise_for_status()
-            page_data = resp.json().get("results", None)
-        except Exception:
-            logger.exception("")
-            if not max_results:
-                return None
+        for i in range(2):
+            try:
+                resp = SESSION.get("https://duckduckgo.com/news.js", params=payload)
+                resp.raise_for_status()
+                page_data = resp.json().get("results", None)
+                break
+            except Exception:
+                logger.exception("")
+                if i == 1 and not max_results:
+                    return None
+                if "506-00.js" in resp.url:
+                    payload["vqd"] = _refresh_vqd(keywords)
+
         page_results = []
         if page_data:
             for row in page_data:
                 if row["url"] not in cache:
                     cache.add(row["url"])
                     page_results.append(
                         {
```

### Comparing `duckduckgo_search-2.9.2/duckduckgo_search/ddg_suggestions.py` & `duckduckgo_search-2.9.3/duckduckgo_search/ddg_suggestions.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.2/duckduckgo_search/ddg_translate.py` & `duckduckgo_search-2.9.3/duckduckgo_search/ddg_translate.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,14 +52,13 @@
             )
             resp.raise_for_status()
             result = resp.json()
             result["original"] = data
             results.append(result)
         except Exception:
             VQD_CACHE.pop("translate", None)
-            VQD_CACHE.close()
             logger.exception("")
 
     if output:
         keywords = keywords[0]
         _do_output("ddg_translate", keywords, output, results)
     return results
```

### Comparing `duckduckgo_search-2.9.2/duckduckgo_search/ddg_videos.py` & `duckduckgo_search-2.9.3/duckduckgo_search/ddg_videos.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from time import sleep
 
-from .utils import SESSION, _do_output, _get_vqd
+from .utils import SESSION, _do_output, _get_vqd, _refresh_vqd
 
 logger = logging.getLogger(__name__)
 
 
 def ddg_videos(
     keywords,
     region="wt-wt",
@@ -37,22 +37,27 @@
     Returns:
         Optional[List[dict]]: DuckDuckGo videos search results
     """
 
     def get_ddg_videos_page(page):
         payload["s"] = max(PAGINATION_STEP * (page - 1), 0)
         page_data = None
-        try:
-            resp = SESSION.get("https://duckduckgo.com/v.js", params=payload)
-            resp.raise_for_status()
-            page_data = resp.json().get("results", None)
-        except Exception:
-            logger.exception("")
-            if not max_results:
-                return None
+        for i in range(2):
+            try:
+                resp = SESSION.get("https://duckduckgo.com/v.js", params=payload)
+                resp.raise_for_status()
+                page_data = resp.json().get("results", None)
+                break
+            except Exception:
+                logger.exception("")
+                if i == 1 and not max_results:
+                    return None
+                if "506-00.js" in resp.url:
+                    payload["vqd"] = _refresh_vqd(keywords)
+
         page_results = []
         if page_data:
             for row in page_data:
                 if row["content"] not in cache:
                     page_results.append(row)
                     cache.add(row["content"])
         return page_results
```

### Comparing `duckduckgo_search-2.9.2/duckduckgo_search/utils.py` & `duckduckgo_search-2.9.3/duckduckgo_search/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -68,14 +68,21 @@
         VQD_CACHE.pop(keywords, None)
         sleep(0.25)
 
     # sleep to prevent blocking
     sleep(0.25)
 
 
+def _refresh_vqd(keywords):
+    VQD_CACHE.pop(keywords, None)
+    vqd = _get_vqd(keywords)
+    logger.debug("keywords=%s. _refresh_vqd()", keywords)
+    return vqd
+
+
 def _save_json(jsonfile, data):
     with open(jsonfile, "w") as file:
         json.dump(data, file, ensure_ascii=False, indent=4)
 
 
 def _save_csv(csvfile, data):
     with open(csvfile, "w", newline="", encoding="utf-8") as file:
```

### Comparing `duckduckgo_search-2.9.2/duckduckgo_search.egg-info/PKG-INFO` & `duckduckgo_search-2.9.3/duckduckgo_search.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo-search
-Version: 2.9.2
+Version: 2.9.3
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duckduckgo_search-2.9.2/duckduckgo_search.egg-info/SOURCES.txt` & `duckduckgo_search-2.9.3/duckduckgo_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.2/pyproject.toml` & `duckduckgo_search-2.9.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.2/tests/test_ddg.py` & `duckduckgo_search-2.9.3/tests/test_ddg.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.2/tests/test_ddg_answers.py` & `duckduckgo_search-2.9.3/tests/test_ddg_answers.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.2/tests/test_ddg_images.py` & `duckduckgo_search-2.9.3/tests/test_ddg_images.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.2/tests/test_ddg_news.py` & `duckduckgo_search-2.9.3/tests/test_ddg_news.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.2/tests/test_ddg_suggestions.py` & `duckduckgo_search-2.9.3/tests/test_ddg_suggestions.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.2/tests/test_ddg_translate.py` & `duckduckgo_search-2.9.3/tests/test_ddg_translate.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.2/tests/test_ddg_videos.py` & `duckduckgo_search-2.9.3/tests/test_ddg_videos.py`

 * *Files identical despite different names*

