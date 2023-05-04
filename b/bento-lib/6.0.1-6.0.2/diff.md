# Comparing `tmp/bento_lib-6.0.1.tar.gz` & `tmp/bento_lib-6.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bento_lib-6.0.1.tar", last modified: Tue Apr  4 01:04:10 2023, max compression
+gzip compressed data, was "bento_lib-6.0.2.tar", last modified: Thu May  4 20:37:40 2023, max compression
```

## Comparing `bento_lib-6.0.1.tar` & `bento_lib-6.0.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 01:04:10.339106 bento_lib-6.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-04-04 01:04:00.000000 bento_lib-6.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-04 01:04:00.000000 bento_lib-6.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-04-04 01:04:10.339106 bento_lib-6.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-04-04 01:04:00.000000 bento_lib-6.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 01:04:10.335106 bento_lib-6.0.1/bento_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-04 01:04:00.000000 bento_lib-6.0.1/bento_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 01:04:10.339106 bento_lib-6.0.1/bento_lib/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 01:04:00.000000 bento_lib-6.0.1/bento_lib/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-04 01:04:00.000000 bento_lib-6.0.1/bento_lib/auth/django_remote_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-04 01:04:00.000000 bento_lib-6.0.1/bento_lib/auth/flask_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-04 01:04:00.000000 bento_lib-6.0.1/bento_lib/auth/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-04 01:04:00.000000 bento_lib-6.0.1/bento_lib/auth/quart_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-04 01:04:00.000000 bento_lib-6.0.1/bento_lib/auth/roles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 01:04:10.339106 bento_lib-6.0.1/bento_lib/drs/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-04 01:04:00.000000 bento_lib-6.0.1/bento_lib/drs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-04-04 01:04:00.000000 bento_lib-6.0.1/bento_lib/drs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 01:04:10.339106 bento_lib-6.0.1/bento_lib/events/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-04 01:04:00.000000 bento_lib-6.0.1/bento_lib/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-04-04 01:04:00.000000 bento_lib-6.0.1/bento_lib/events/_event_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-04 01:04:00.000000 bento_lib-6.0.1/bento_lib/events/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-04 01:04:00.000000 bento_lib-6.0.1/bento_lib/events/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-04 01:04:00.000000 bento_lib-6.0.1/bento_lib/package.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 01:04:10.339106 bento_lib-6.0.1/bento_lib/responses/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-04 01:04:00.000000 bento_lib-6.0.1/bento_lib/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-04-04 01:04:00.000000 bento_lib-6.0.1/bento_lib/responses/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-04-04 01:04:00.000000 bento_lib-6.0.1/bento_lib/responses/flask_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-04-04 01:04:00.000000 bento_lib-6.0.1/bento_lib/responses/quart_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 01:04:10.339106 bento_lib-6.0.1/bento_lib/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-04 01:04:00.000000 bento_lib-6.0.1/bento_lib/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-04 01:04:00.000000 bento_lib-6.0.1/bento_lib/schemas/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-04 01:04:00.000000 bento_lib-6.0.1/bento_lib/schemas/bento.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-04 01:04:00.000000 bento_lib-6.0.1/bento_lib/schemas/bento_data_use.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-04 01:04:00.000000 bento_lib-6.0.1/bento_lib/schemas/bento_ingest.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-04 01:04:00.000000 bento_lib-6.0.1/bento_lib/schemas/ga4gh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-04 01:04:00.000000 bento_lib-6.0.1/bento_lib/schemas/ga4gh_service_info.schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 01:04:10.339106 bento_lib-6.0.1/bento_lib/search/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-04 01:04:00.000000 bento_lib-6.0.1/bento_lib/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-04 01:04:00.000000 bento_lib-6.0.1/bento_lib/search/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    26842 2023-04-04 01:04:00.000000 bento_lib-6.0.1/bento_lib/search/data_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-04 01:04:00.000000 bento_lib-6.0.1/bento_lib/search/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)    22589 2023-04-04 01:04:00.000000 bento_lib-6.0.1/bento_lib/search/postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-04-04 01:04:00.000000 bento_lib-6.0.1/bento_lib/search/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-04 01:04:00.000000 bento_lib-6.0.1/bento_lib/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-04-04 01:04:00.000000 bento_lib-6.0.1/bento_lib/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 01:04:10.335106 bento_lib-6.0.1/bento_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-04-04 01:04:10.000000 bento_lib-6.0.1/bento_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-04 01:04:10.000000 bento_lib-6.0.1/bento_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 01:04:10.000000 bento_lib-6.0.1/bento_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-04 01:04:10.000000 bento_lib-6.0.1/bento_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-04 01:04:10.000000 bento_lib-6.0.1/bento_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 01:04:10.339106 bento_lib-6.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-04 01:04:00.000000 bento_lib-6.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:37:40.115371 bento_lib-6.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-04 20:37:25.000000 bento_lib-6.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-04 20:37:25.000000 bento_lib-6.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-05-04 20:37:40.111371 bento_lib-6.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-05-04 20:37:25.000000 bento_lib-6.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:37:40.107371 bento_lib-6.0.2/bento_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-04 20:37:25.000000 bento_lib-6.0.2/bento_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:37:40.107371 bento_lib-6.0.2/bento_lib/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 20:37:25.000000 bento_lib-6.0.2/bento_lib/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-04 20:37:25.000000 bento_lib-6.0.2/bento_lib/auth/django_remote_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-04 20:37:25.000000 bento_lib-6.0.2/bento_lib/auth/flask_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-04 20:37:25.000000 bento_lib-6.0.2/bento_lib/auth/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-04 20:37:25.000000 bento_lib-6.0.2/bento_lib/auth/quart_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-04 20:37:25.000000 bento_lib-6.0.2/bento_lib/auth/roles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:37:40.107371 bento_lib-6.0.2/bento_lib/drs/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-04 20:37:25.000000 bento_lib-6.0.2/bento_lib/drs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-05-04 20:37:25.000000 bento_lib-6.0.2/bento_lib/drs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:37:40.107371 bento_lib-6.0.2/bento_lib/events/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-04 20:37:25.000000 bento_lib-6.0.2/bento_lib/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-05-04 20:37:25.000000 bento_lib-6.0.2/bento_lib/events/_event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-04 20:37:25.000000 bento_lib-6.0.2/bento_lib/events/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-04 20:37:25.000000 bento_lib-6.0.2/bento_lib/events/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-04 20:37:25.000000 bento_lib-6.0.2/bento_lib/package.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:37:40.111371 bento_lib-6.0.2/bento_lib/responses/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-04 20:37:25.000000 bento_lib-6.0.2/bento_lib/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-05-04 20:37:25.000000 bento_lib-6.0.2/bento_lib/responses/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-04 20:37:25.000000 bento_lib-6.0.2/bento_lib/responses/flask_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-05-04 20:37:25.000000 bento_lib-6.0.2/bento_lib/responses/quart_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:37:40.111371 bento_lib-6.0.2/bento_lib/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-04 20:37:25.000000 bento_lib-6.0.2/bento_lib/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-04 20:37:25.000000 bento_lib-6.0.2/bento_lib/schemas/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-04 20:37:25.000000 bento_lib-6.0.2/bento_lib/schemas/bento.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-04 20:37:25.000000 bento_lib-6.0.2/bento_lib/schemas/bento_data_use.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-04 20:37:25.000000 bento_lib-6.0.2/bento_lib/schemas/bento_ingest.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-04 20:37:25.000000 bento_lib-6.0.2/bento_lib/schemas/ga4gh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-04 20:37:25.000000 bento_lib-6.0.2/bento_lib/schemas/ga4gh_service_info.schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:37:40.111371 bento_lib-6.0.2/bento_lib/search/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-04 20:37:25.000000 bento_lib-6.0.2/bento_lib/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-04 20:37:25.000000 bento_lib-6.0.2/bento_lib/search/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26842 2023-05-04 20:37:25.000000 bento_lib-6.0.2/bento_lib/search/data_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-04 20:37:25.000000 bento_lib-6.0.2/bento_lib/search/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22589 2023-05-04 20:37:25.000000 bento_lib-6.0.2/bento_lib/search/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-05-04 20:37:25.000000 bento_lib-6.0.2/bento_lib/search/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-04 20:37:25.000000 bento_lib-6.0.2/bento_lib/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-05-04 20:37:25.000000 bento_lib-6.0.2/bento_lib/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:37:40.107371 bento_lib-6.0.2/bento_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-05-04 20:37:40.000000 bento_lib-6.0.2/bento_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-04 20:37:40.000000 bento_lib-6.0.2/bento_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 20:37:40.000000 bento_lib-6.0.2/bento_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-04 20:37:40.000000 bento_lib-6.0.2/bento_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-04 20:37:40.000000 bento_lib-6.0.2/bento_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 20:37:40.115371 bento_lib-6.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-04 20:37:25.000000 bento_lib-6.0.2/setup.py
```

### Comparing `bento_lib-6.0.1/LICENSE` & `bento_lib-6.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bento_lib-6.0.1/PKG-INFO` & `bento_lib-6.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bento_lib
-Version: 6.0.1
+Version: 6.0.2
 Summary: A set of common utilities and helpers for Bento platform services.
 Home-page: https://github.com/bento-platform/bento_lib
 Author: David Lougheed, Paul Pillot
 Author-email: david.lougheed@mail.mcgill.ca, paul.pillot@computationalgenomics.ca
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `bento_lib-6.0.1/README.md` & `bento_lib-6.0.2/README.md`

 * *Files identical despite different names*

### Comparing `bento_lib-6.0.1/bento_lib/auth/django_remote_user.py` & `bento_lib-6.0.2/bento_lib/auth/django_remote_user.py`

 * *Files identical despite different names*

### Comparing `bento_lib-6.0.1/bento_lib/auth/flask_decorators.py` & `bento_lib-6.0.2/bento_lib/auth/flask_decorators.py`

 * *Files identical despite different names*

### Comparing `bento_lib-6.0.1/bento_lib/auth/quart_decorators.py` & `bento_lib-6.0.2/bento_lib/auth/quart_decorators.py`

 * *Files identical despite different names*

### Comparing `bento_lib-6.0.1/bento_lib/drs/utils.py` & `bento_lib-6.0.2/bento_lib/drs/utils.py`

 * *Files identical despite different names*

### Comparing `bento_lib-6.0.1/bento_lib/events/_event_bus.py` & `bento_lib-6.0.2/bento_lib/events/_event_bus.py`

 * *Files identical despite different names*

### Comparing `bento_lib-6.0.1/bento_lib/events/notifications.py` & `bento_lib-6.0.2/bento_lib/events/notifications.py`

 * *Files identical despite different names*

### Comparing `bento_lib-6.0.1/bento_lib/events/types.py` & `bento_lib-6.0.2/bento_lib/events/types.py`

 * *Files identical despite different names*

### Comparing `bento_lib-6.0.1/bento_lib/responses/errors.py` & `bento_lib-6.0.2/bento_lib/responses/errors.py`

 * *Files identical despite different names*

### Comparing `bento_lib-6.0.1/bento_lib/responses/flask_errors.py` & `bento_lib-6.0.2/bento_lib/responses/flask_errors.py`

 * *Files identical despite different names*

### Comparing `bento_lib-6.0.1/bento_lib/responses/quart_errors.py` & `bento_lib-6.0.2/bento_lib/responses/quart_errors.py`

 * *Files identical despite different names*

### Comparing `bento_lib-6.0.1/bento_lib/schemas/bento_data_use.schema.json` & `bento_lib-6.0.2/bento_lib/schemas/bento_data_use.schema.json`

 * *Files identical despite different names*

### Comparing `bento_lib-6.0.1/bento_lib/schemas/bento_ingest.schema.json` & `bento_lib-6.0.2/bento_lib/schemas/bento_ingest.schema.json`

 * *Files identical despite different names*

### Comparing `bento_lib-6.0.1/bento_lib/schemas/ga4gh_service_info.schema.json` & `bento_lib-6.0.2/bento_lib/schemas/ga4gh_service_info.schema.json`

 * *Files identical despite different names*

### Comparing `bento_lib-6.0.1/bento_lib/search/data_structure.py` & `bento_lib-6.0.2/bento_lib/search/data_structure.py`

 * *Files identical despite different names*

### Comparing `bento_lib-6.0.1/bento_lib/search/operations.py` & `bento_lib-6.0.2/bento_lib/search/operations.py`

 * *Files identical despite different names*

### Comparing `bento_lib-6.0.1/bento_lib/search/postgres.py` & `bento_lib-6.0.2/bento_lib/search/postgres.py`

 * *Files identical despite different names*

### Comparing `bento_lib-6.0.1/bento_lib/search/queries.py` & `bento_lib-6.0.2/bento_lib/search/queries.py`

 * *Files identical despite different names*

### Comparing `bento_lib-6.0.1/bento_lib/types.py` & `bento_lib-6.0.2/bento_lib/types.py`

 * *Files identical despite different names*

### Comparing `bento_lib-6.0.1/bento_lib/workflows.py` & `bento_lib-6.0.2/bento_lib/workflows.py`

 * *Files identical despite different names*

### Comparing `bento_lib-6.0.1/bento_lib.egg-info/PKG-INFO` & `bento_lib-6.0.2/bento_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bento-lib
-Version: 6.0.1
+Version: 6.0.2
 Summary: A set of common utilities and helpers for Bento platform services.
 Home-page: https://github.com/bento-platform/bento_lib
 Author: David Lougheed, Paul Pillot
 Author-email: david.lougheed@mail.mcgill.ca, paul.pillot@computationalgenomics.ca
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `bento_lib-6.0.1/bento_lib.egg-info/SOURCES.txt` & `bento_lib-6.0.2/bento_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bento_lib-6.0.1/setup.py` & `bento_lib-6.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,17 +20,17 @@
         "jsonschema>=4.17.3,<5",
         "psycopg2-binary>=2.9.5,<3.0",
         "redis>=4.5.1,<5.0",
         "requests>=2.28.1,<3",
         "Werkzeug>=2.2.3,<3",
     ],
     extras_require={
-        "flask": ["Flask>=2.2.3,<3"],
+        "flask": ["Flask>=2.2.5,<3"],
         "django": ["Django>=4.1.7,<5", "djangorestframework>=3.14.0,<3.15"],
-        "quart": ["quart>=0.18.3,<0.19"],
+        "quart": ["quart>=0.18.4,<0.19"],
     },
 
     author=config["package"]["authors"],
     author_email=config["package"]["author_emails"],
 
     description="A set of common utilities and helpers for Bento platform services.",
     long_description=long_description,
```

