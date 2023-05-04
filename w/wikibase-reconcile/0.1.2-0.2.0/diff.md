# Comparing `tmp/wikibase_reconcile-0.1.2.tar.gz` & `tmp/wikibase_reconcile-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wikibase_reconcile-0.1.2.tar", last modified: Mon Apr  3 19:21:32 2023, max compression
+gzip compressed data, was "wikibase_reconcile-0.2.0.tar", last modified: Thu May  4 13:58:39 2023, max compression
```

## Comparing `wikibase_reconcile-0.1.2.tar` & `wikibase_reconcile-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 balluff   (1000) balluff   (1000)        0 2023-04-03 19:21:32.915481 wikibase_reconcile-0.1.2/
--rw-rw-r--   0 balluff   (1000) balluff   (1000)    11357 2023-04-03 17:26:24.000000 wikibase_reconcile-0.1.2/LICENSE
--rw-rw-r--   0 balluff   (1000) balluff   (1000)     1922 2023-04-03 19:21:32.915481 wikibase_reconcile-0.1.2/PKG-INFO
--rw-rw-r--   0 balluff   (1000) balluff   (1000)     1323 2023-04-03 18:06:21.000000 wikibase_reconcile-0.1.2/README.md
--rw-rw-r--   0 balluff   (1000) balluff   (1000)      672 2023-04-03 19:21:25.000000 wikibase_reconcile-0.1.2/pyproject.toml
--rw-rw-r--   0 balluff   (1000) balluff   (1000)       38 2023-04-03 19:21:32.915481 wikibase_reconcile-0.1.2/setup.cfg
--rw-rw-r--   0 balluff   (1000) balluff   (1000)      193 2023-04-03 16:56:45.000000 wikibase_reconcile-0.1.2/setup.py
-drwxrwxr-x   0 balluff   (1000) balluff   (1000)        0 2023-04-03 19:21:32.911481 wikibase_reconcile-0.1.2/src/
-drwxrwxr-x   0 balluff   (1000) balluff   (1000)        0 2023-04-03 19:21:32.911481 wikibase_reconcile-0.1.2/src/wikibase_reconcile/
--rw-rw-r--   0 balluff   (1000) balluff   (1000)       26 2023-04-03 16:55:03.000000 wikibase_reconcile-0.1.2/src/wikibase_reconcile/__init__.py
--rw-rw-r--   0 balluff   (1000) balluff   (1000)     9049 2023-04-03 19:20:23.000000 wikibase_reconcile-0.1.2/src/wikibase_reconcile/client.py
-drwxrwxr-x   0 balluff   (1000) balluff   (1000)        0 2023-04-03 19:21:32.915481 wikibase_reconcile-0.1.2/src/wikibase_reconcile.egg-info/
--rw-rw-r--   0 balluff   (1000) balluff   (1000)     1922 2023-04-03 19:21:32.000000 wikibase_reconcile-0.1.2/src/wikibase_reconcile.egg-info/PKG-INFO
--rw-rw-r--   0 balluff   (1000) balluff   (1000)      338 2023-04-03 19:21:32.000000 wikibase_reconcile-0.1.2/src/wikibase_reconcile.egg-info/SOURCES.txt
--rw-rw-r--   0 balluff   (1000) balluff   (1000)        1 2023-04-03 19:21:32.000000 wikibase_reconcile-0.1.2/src/wikibase_reconcile.egg-info/dependency_links.txt
--rw-rw-r--   0 balluff   (1000) balluff   (1000)       56 2023-04-03 19:21:32.000000 wikibase_reconcile-0.1.2/src/wikibase_reconcile.egg-info/requires.txt
--rw-rw-r--   0 balluff   (1000) balluff   (1000)       19 2023-04-03 19:21:32.000000 wikibase_reconcile-0.1.2/src/wikibase_reconcile.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:58:39.808684 wikibase_reconcile-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-04 13:58:28.000000 wikibase_reconcile-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-05-04 13:58:39.808684 wikibase_reconcile-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-04 13:58:28.000000 wikibase_reconcile-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-04 13:58:28.000000 wikibase_reconcile-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 13:58:39.808684 wikibase_reconcile-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-04 13:58:28.000000 wikibase_reconcile-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:58:39.804684 wikibase_reconcile-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:58:39.808684 wikibase_reconcile-0.2.0/src/wikibase_reconcile/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-04 13:58:28.000000 wikibase_reconcile-0.2.0/src/wikibase_reconcile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10369 2023-05-04 13:58:28.000000 wikibase_reconcile-0.2.0/src/wikibase_reconcile/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:58:39.808684 wikibase_reconcile-0.2.0/src/wikibase_reconcile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-05-04 13:58:39.000000 wikibase_reconcile-0.2.0/src/wikibase_reconcile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-04 13:58:39.000000 wikibase_reconcile-0.2.0/src/wikibase_reconcile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 13:58:39.000000 wikibase_reconcile-0.2.0/src/wikibase_reconcile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-04 13:58:39.000000 wikibase_reconcile-0.2.0/src/wikibase_reconcile.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-04 13:58:39.000000 wikibase_reconcile-0.2.0/src/wikibase_reconcile.egg-info/top_level.txt
```

### Comparing `wikibase_reconcile-0.1.2/LICENSE` & `wikibase_reconcile-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wikibase_reconcile-0.1.2/PKG-INFO` & `wikibase_reconcile-0.2.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,33 @@
-Metadata-Version: 2.1
-Name: wikibase_reconcile
-Version: 0.1.2
-Summary: An async client to reconcile entities against wikidata.
-Author-email: Paul Balluff <paul.balluff@gmail.com>
-Project-URL: Homepage, https://github.com/mrwunderbar666/wikibase_reconcile
-Project-URL: Bug Tracker, https://github.com/mrwunderbar666/wikibase_reconcile/sampleproject/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Wikibase Reconcile
 
-An async client to reconcile against wikidata.
+An multi-threaded client to reconcile against wikidata.
 
 This project is inspired by [reconciler](https://pypi.org/project/reconciler/). If you look for stable and mature software, I recommend using the excellent package `reconciler`.
 
 
 ## Features
 
-- Async requests to wikidata reconiliation API
+- Concurrent requests to wikidata reconiliation API
 - Makes atomic requests and is more robust when the API returns errors
 - Takes a pandas dataframe as input and also as output
 - User has rather high degree of control (but also needs more code)
 
+## Installation
+
+```
+pip install wikibase-reconcile
+```
 
 ## Usage
 
 ```python
 from wikibase_reconcile import Client
 
-client = Client(language="fr")
+client = Client()
 
 # Initialize some simple test data
 characters = [
     {"type": "Q15632617", "query": "Marge Simpson"},
     {"type": "Q15632617", "query": "Homer Simpson"},
     {"type": "Q15632617", "query": "Bart Simpson"},
     {"type": "Q15632617", "query": "Lisa Simpson"},
@@ -50,7 +41,22 @@
 
 # reconcile each search query against the type "Fictional Human"
 results = client.reconcile(df)
 
 # Turn results into a dataframe, keep only the top result
 df_reconciled = client.results_to_pandas(results)
 ```
+
+### Fallback Logic
+
+You can specify an additional fallback search string in case the first attempt did not yield any result:
+
+
+```python
+query = {"type": "Q15632617", "query": "Marge Simpson", "fallback_query": "Marjorie Bouvier"}
+```
+
+One use case for fallback queries are lemmatized versions of the original query.
+
+If this still yields no results, then the reconciler will attempt to match the first part of the query, by splitting the query at every hyphen character (`-`) and taking the first part. **This logic is likely to change in future versions.**
+
+The final fallback is to ignore the type and try to reconcile against any type. The default API server (`https://wikidata.reconci.link/`) will then match against the generic entity type (Q35120).
```

### Comparing `wikibase_reconcile-0.1.2/pyproject.toml` & `wikibase_reconcile-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "wikibase_reconcile"
-version = "0.1.2"
+version = "0.2.0"
 authors = [
   { name="Paul Balluff", email="paul.balluff@gmail.com" },
 ]
-description = "An async client to reconcile entities against wikidata."
+description = "A concurrent client to reconcile entities against wikidata."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `wikibase_reconcile-0.1.2/src/wikibase_reconcile/client.py` & `wikibase_reconcile-0.2.0/src/wikibase_reconcile/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 from typing import Union
 
 from functools import lru_cache
-import aiohttp
-import asyncio
 import json
-from tqdm.asyncio import tqdm
+from tqdm import tqdm
 import pandas as pd
+from concurrent.futures import ThreadPoolExecutor, as_completed
+import requests
 
 
 class Client:
 
-    def __init__(self, language="en", api="https://wikidata.reconci.link/") -> None:
+    def __init__(self, language="en", 
+                 api="https://wikidata.reconci.link/",
+                 threads=4) -> None:
         """Create a new Client.
 
         The client class handles everything for reconciliation and deals with 
-        async connections.
+        concurrent connections.
 
         Currently, only supports 'https://wikidata.reconci.link/' endpoints
 
         Args:
             language (str, optional): Set the language of your search terms. Defaults to "en".
             api (str, optional): URL to API endpoint. Defaults to "https://wikidata.reconci.link/".
+            threads (int, optional). Number of concurrent requests (more is faster, but might cause server to reject your requests). Defaults to 4.
         """
 
         if not api.endswith('/'):
             api += '/'
 
-        self.api = api + language + '/api'
-        self.language = language
+        self._api = api + language + '/api'
+        self._language = language
+        self._threads = threads
 
     def reconcile(self,
                   data: Union[list, dict, pd.DataFrame],
                   property_mapping: dict=None,
                   limit=50) -> list:
         """Main method for reconciling a collection of data.
 
@@ -39,14 +43,16 @@
         The required key for your dicts (or dataframe) is 'query' which is 
         the search string you want to look up at the reconciliation endpoint.
 
         You can additionally, provide the key 'type' to reconcile a specific type 
         (e.g. 'Q5' for humans). Then the client will request wikidata entries that 
         match against this type ("find me all entries with query keyword 'X' and are instance of 'Q5'")
 
+        A wrapper for the `Client.query()` method
+        
         Args:
             data (Union[list, dict, pd.DataFrame]): Your input data.
             property_mapping (dict, optional): A property matching dictionary for a pandas dataframe. 
                 In the style of {'<Column Name>': '<Wikidata Property>'}. Ex. {'country': 'P17'}. Defaults to None.
             limit (int, optional): Maximum number of results returned per query. Defaults to 50.
 
         Returns:
@@ -54,87 +60,103 @@
         """
         if isinstance(data, pd.DataFrame):
             data = self.pandas_to_query(
                 data, limit=limit, property_mapping=property_mapping)
         elif isinstance(data, dict):
             data = [data]
 
-        loop = asyncio.get_event_loop()
-        futures = loop.run_until_complete(self.query(data))
-        return futures
+        return self.query(data)
 
-    async def query(self, data: list) -> list:
-        """Async query Wikidata (or reconciliation service) 
+    def query(self, data: list) -> list:
+        """Concurrent query Wikidata (or reconciliation service) 
 
         Args:
             data (list): a list of dicts where each dict is a query.
 
         Returns:
             list: a list of dicts where ach dict is the reconciled response.
         """        
-        tasks = []
-        async with aiohttp.ClientSession() as session:
-            for single_query in data:
-                task = asyncio.ensure_future(
-                    self._single_query(session, single_query))
-                tasks.append(task)
-            responses = [await f for f in tqdm.as_completed(tasks, desc="Reconciling")]
-        return responses
+        results = []
+        with tqdm(total=len(data), unit="queries", desc="Reconciling") as pbar:
+            with ThreadPoolExecutor(max_workers=self._threads) as executor:
+                tasks = [executor.submit(self._single_query, q) for q in data]
+                for future in as_completed(tasks):
+                    results.append(future.result())
+                    pbar.update(1)
+
+        return results
 
     @lru_cache(maxsize=None)
-    async def _perform_single_query(self,
-                                    session: aiohttp.ClientSession,
-                                    query: str,
-                                    search_string: str,
-                                    max_retries=10) -> dict:
-        """Async low level function to performa a single query.
+    def _perform_single_query(self,
+                                query: str,
+                                search_string: str,
+                                max_retries=10,
+                                fallback_searchstring: bool = False) -> dict:
+        """ low level function to performa a single query.
 
         Args:
-            session (aiohttp.ClientSession): an aiohttp session object.
             query (str): a serialized JSON dict (generated with `json.dumps(data)`)
             search_string (str): the original search query.
             max_retries (int, optional): Maximum attempts to retry. Defaults to 10.
-
+            fallback_searchstring (bool, optional): Used for managing recursive calls.
         Returns:
             dict: A single query result
         """        
 
         formatted_query = {"query": query}
         tries = 0
         while tries < max_retries:
             try:
-                async with session.get(self.api, params=formatted_query) as response:
-                    # return await response.json()
-                    j = await response.json()
-                    j['search_string'] = search_string
-                    return j
-            except (aiohttp.ServerTimeoutError, aiohttp.ServerConnectionError, asyncio.TimeoutError):
+                r = requests.get(self._api, params=formatted_query)
+                r.raise_for_status()
+                j = r.json()
+                j['search_string'] = search_string
+                if "status" in j and j["status"] == "error":
+                    if tries == max_retries - 1:
+                        return {'search_string': search_string, 'result': [], 'status': j['status']}
+                    tries += 1
+                    continue
+                # What actions to perform when there is no result?
+                if len(j['result']) == 0:
+                    query = json.loads(query)
+                    # if a fallback query is specified, try that one first
+                    if 'fallback_query' in query:
+                        query["query"] = query.pop("fallback_query")
+                        return self._perform_single_query(json.dumps(query), search_string)
+                    # if the search query has hyphens, we try to search for the first element instead
+                    if "-" in search_string and not fallback_searchstring:
+                        query["query"] = search_string.split("-")[0]
+                        return self._perform_single_query(json.dumps(query), search_string, fallback_searchstring=True)
+                    # try to match against no type
+                    elif "type" in query:
+                        _ = query.pop("type")
+                        return self._perform_single_query(json.dumps(query), search_string)
+                return j
+
+            except (requests.ConnectionError, requests.ConnectTimeout):
                 tries += 1
             except Exception as e:
                 return {'search_string': search_string, 'result': [], 'error': e}
 
         if tries == max_retries:
             return {'search_string': search_string, 'result': [], 'error': 'Too many retries'}
 
-    async def _single_query(self,
-                            session: aiohttp.ClientSession,
-                            query: dict) -> dict:
-        """Async wrapper to prepare a dict for `_perform_single_query()` method.
+    def _single_query(self, query: dict) -> dict:
+        """Wrapper to prepare a dict for `_perform_single_query()` method.
 
         Args:
-            session (aiohttp.ClientSession): an aiohttp session object
             query (dict): A single query dictionary.
 
         Returns:
             dict: A single query result
         """        
 
         search_string = query['query']
 
-        return await self._perform_single_query(session, json.dumps(query), search_string)
+        return self._perform_single_query(json.dumps(query), search_string)
 
     @staticmethod
     def pandas_to_query(df: pd.DataFrame, limit=50, property_mapping: dict = None) -> list:
         """Transform a pandas dataframe to a list of dicts
 
         You can additionally, provide the key 'type' to reconcile a specific type 
         (e.g. 'Q5' for humans). Then the client will request wikidata entries that
```

### Comparing `wikibase_reconcile-0.1.2/src/wikibase_reconcile.egg-info/PKG-INFO` & `wikibase_reconcile-0.2.0/src/wikibase_reconcile.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,47 @@
 Metadata-Version: 2.1
 Name: wikibase-reconcile
-Version: 0.1.2
-Summary: An async client to reconcile entities against wikidata.
+Version: 0.2.0
+Summary: A concurrent client to reconcile entities against wikidata.
 Author-email: Paul Balluff <paul.balluff@gmail.com>
 Project-URL: Homepage, https://github.com/mrwunderbar666/wikibase_reconcile
 Project-URL: Bug Tracker, https://github.com/mrwunderbar666/wikibase_reconcile/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Wikibase Reconcile
 
-An async client to reconcile against wikidata.
+An multi-threaded client to reconcile against wikidata.
 
 This project is inspired by [reconciler](https://pypi.org/project/reconciler/). If you look for stable and mature software, I recommend using the excellent package `reconciler`.
 
 
 ## Features
 
-- Async requests to wikidata reconiliation API
+- Concurrent requests to wikidata reconiliation API
 - Makes atomic requests and is more robust when the API returns errors
 - Takes a pandas dataframe as input and also as output
 - User has rather high degree of control (but also needs more code)
 
+## Installation
+
+```
+pip install wikibase-reconcile
+```
 
 ## Usage
 
 ```python
 from wikibase_reconcile import Client
 
-client = Client(language="fr")
+client = Client()
 
 # Initialize some simple test data
 characters = [
     {"type": "Q15632617", "query": "Marge Simpson"},
     {"type": "Q15632617", "query": "Homer Simpson"},
     {"type": "Q15632617", "query": "Bart Simpson"},
     {"type": "Q15632617", "query": "Lisa Simpson"},
@@ -50,7 +55,22 @@
 
 # reconcile each search query against the type "Fictional Human"
 results = client.reconcile(df)
 
 # Turn results into a dataframe, keep only the top result
 df_reconciled = client.results_to_pandas(results)
 ```
+
+### Fallback Logic
+
+You can specify an additional fallback search string in case the first attempt did not yield any result:
+
+
+```python
+query = {"type": "Q15632617", "query": "Marge Simpson", "fallback_query": "Marjorie Bouvier"}
+```
+
+One use case for fallback queries are lemmatized versions of the original query.
+
+If this still yields no results, then the reconciler will attempt to match the first part of the query, by splitting the query at every hyphen character (`-`) and taking the first part. **This logic is likely to change in future versions.**
+
+The final fallback is to ignore the type and try to reconcile against any type. The default API server (`https://wikidata.reconci.link/`) will then match against the generic entity type (Q35120).
```

