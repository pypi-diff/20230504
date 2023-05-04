# Comparing `tmp/recon_lw-2.0.0.dev4870468547.tar.gz` & `tmp/recon_lw-2.0.0.dev4882741872.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev4870468547.tar", last modified: Wed May  3 09:40:58 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev4882741872.tar", last modified: Thu May  4 12:26:23 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev4870468547.tar` & `recon_lw-2.0.0.dev4882741872.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 09:40:58.000000 recon_lw-2.0.0.dev4870468547/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-03 09:40:17.000000 recon_lw-2.0.0.dev4870468547/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-03 09:40:58.000000 recon_lw-2.0.0.dev4870468547/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-03 09:40:17.000000 recon_lw-2.0.0.dev4870468547/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-03 09:40:38.000000 recon_lw-2.0.0.dev4870468547/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 09:40:58.000000 recon_lw-2.0.0.dev4870468547/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-05-03 09:40:17.000000 recon_lw-2.0.0.dev4870468547/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     2748 2023-05-03 09:40:17.000000 recon_lw-2.0.0.dev4870468547/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-03 09:40:17.000000 recon_lw-2.0.0.dev4870468547/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13016 2023-05-03 09:40:17.000000 recon_lw-2.0.0.dev4870468547/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    21309 2023-05-03 09:40:17.000000 recon_lw-2.0.0.dev4870468547/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    14809 2023-05-03 09:40:17.000000 recon_lw-2.0.0.dev4870468547/recon_lw/recon_ob_cross_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 09:40:58.000000 recon_lw-2.0.0.dev4870468547/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-03 09:40:58.000000 recon_lw-2.0.0.dev4870468547/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      396 2023-05-03 09:40:58.000000 recon_lw-2.0.0.dev4870468547/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-03 09:40:58.000000 recon_lw-2.0.0.dev4870468547/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-03 09:40:58.000000 recon_lw-2.0.0.dev4870468547/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-03 09:40:58.000000 recon_lw-2.0.0.dev4870468547/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-03 09:40:17.000000 recon_lw-2.0.0.dev4870468547/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-03 09:40:58.000000 recon_lw-2.0.0.dev4870468547/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-03 09:40:17.000000 recon_lw-2.0.0.dev4870468547/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 09:40:58.000000 recon_lw-2.0.0.dev4870468547/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-05-03 09:40:17.000000 recon_lw-2.0.0.dev4870468547/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 12:26:22.000000 recon_lw-2.0.0.dev4882741872/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-04 12:25:53.000000 recon_lw-2.0.0.dev4882741872/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-04 12:26:22.000000 recon_lw-2.0.0.dev4882741872/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-04 12:25:53.000000 recon_lw-2.0.0.dev4882741872/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-04 12:26:01.000000 recon_lw-2.0.0.dev4882741872/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 12:26:22.000000 recon_lw-2.0.0.dev4882741872/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-05-04 12:25:53.000000 recon_lw-2.0.0.dev4882741872/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2748 2023-05-04 12:25:53.000000 recon_lw-2.0.0.dev4882741872/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-04 12:25:53.000000 recon_lw-2.0.0.dev4882741872/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13016 2023-05-04 12:25:53.000000 recon_lw-2.0.0.dev4882741872/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21366 2023-05-04 12:25:53.000000 recon_lw-2.0.0.dev4882741872/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14809 2023-05-04 12:25:53.000000 recon_lw-2.0.0.dev4882741872/recon_lw/recon_ob_cross_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 12:26:22.000000 recon_lw-2.0.0.dev4882741872/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-04 12:26:22.000000 recon_lw-2.0.0.dev4882741872/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      396 2023-05-04 12:26:22.000000 recon_lw-2.0.0.dev4882741872/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-04 12:26:22.000000 recon_lw-2.0.0.dev4882741872/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-04 12:26:22.000000 recon_lw-2.0.0.dev4882741872/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-04 12:26:22.000000 recon_lw-2.0.0.dev4882741872/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-04 12:25:53.000000 recon_lw-2.0.0.dev4882741872/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-04 12:26:22.000000 recon_lw-2.0.0.dev4882741872/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-04 12:25:53.000000 recon_lw-2.0.0.dev4882741872/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 12:26:22.000000 recon_lw-2.0.0.dev4882741872/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-05-04 12:25:53.000000 recon_lw-2.0.0.dev4882741872/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev4870468547/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev4882741872/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4870468547/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev4882741872/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4870468547/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev4882741872/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4870468547/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev4882741872/recon_lw/recon_ob.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,25 +63,27 @@
         sequence.pop(0)
 
 
 def process_market_data_update(mess: dict, events: list, books_cache: dict, get_book_id_func,
                                update_book_rule,
                                check_book_rule, event_sequence: dict, parent_event: dict,
                                initial_book_params: dict, log_books_filter) -> None:
-    book_id, result = get_book_id_func(mess)
+    book_ids_list, result = get_book_id_func(mess)
     if result is not None:
         book_id_event = recon_lw.create_event("GetBookEroor:" + parent_event["eventName"], "GetBookEroor",
                                               event_sequence,
                                               ok=False,
                                               body=result,
                                               parentId=parent_event["eventId"])
         book_id_event["attachedMessageIds"] = [mess["messageId"]]
         events.append(book_id_event)
 
-    if book_id is not None:
+    if book_ids_list is None:
+        return
+    for book_id in book_ids_list:
         if book_id not in books_cache:
             books_cache[book_id] = copy.deepcopy(initial_book_params)
             # books_cache[book_id] = {"ask": {}, "bid": {}, "status": "?"}
         book = books_cache[book_id]
         operations = update_book_rule(book, mess)
         if operations is None:
             return
```

### Comparing `recon_lw-2.0.0.dev4870468547/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev4882741872/recon_lw/recon_ob_cross_stream.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4870468547/setup.py` & `recon_lw-2.0.0.dev4882741872/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4870468547/test/test_recon_ob.py` & `recon_lw-2.0.0.dev4882741872/test/test_recon_ob.py`

 * *Files identical despite different names*

