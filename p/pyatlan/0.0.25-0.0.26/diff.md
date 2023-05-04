# Comparing `tmp/pyatlan-0.0.25.tar.gz` & `tmp/pyatlan-0.0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyatlan-0.0.25.tar", last modified: Tue May  2 14:02:19 2023, max compression
+gzip compressed data, was "pyatlan-0.0.26.tar", last modified: Thu May  4 15:48:25 2023, max compression
```

## Comparing `pyatlan-0.0.25.tar` & `pyatlan-0.0.26.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:02:19.986967 pyatlan-0.0.25/
--rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-05-02 14:02:05.000000 pyatlan-0.0.25/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-02 14:02:05.000000 pyatlan-0.0.25/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-02 14:02:05.000000 pyatlan-0.0.25/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-02 14:02:19.986967 pyatlan-0.0.25/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-02 14:02:05.000000 pyatlan-0.0.25/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:02:19.974967 pyatlan-0.0.25/pyatlan/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-02 14:02:05.000000 pyatlan-0.0.25/pyatlan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:02:19.974967 pyatlan-0.0.25/pyatlan/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-02 14:02:05.000000 pyatlan-0.0.25/pyatlan/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-05-02 14:02:05.000000 pyatlan-0.0.25/pyatlan/cache/classification_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     9761 2023-05-02 14:02:05.000000 pyatlan-0.0.25/pyatlan/cache/custom_metadata_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-02 14:02:05.000000 pyatlan-0.0.25/pyatlan/cache/role_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:02:19.978967 pyatlan-0.0.25/pyatlan/client/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-02 14:02:05.000000 pyatlan-0.0.25/pyatlan/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20816 2023-05-02 14:02:05.000000 pyatlan-0.0.25/pyatlan/client/atlan.py
--rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-05-02 14:02:05.000000 pyatlan-0.0.25/pyatlan/client/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-05-02 14:02:05.000000 pyatlan-0.0.25/pyatlan/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-05-02 14:02:05.000000 pyatlan-0.0.25/pyatlan/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:02:19.978967 pyatlan-0.0.25/pyatlan/generator/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-02 14:02:05.000000 pyatlan-0.0.25/pyatlan/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-05-02 14:02:05.000000 pyatlan-0.0.25/pyatlan/generator/generate_from_typdefs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:02:19.978967 pyatlan-0.0.25/pyatlan/generator/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-02 14:02:05.000000 pyatlan-0.0.25/pyatlan/generator/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:02:19.982967 pyatlan-0.0.25/pyatlan/model/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-02 14:02:05.000000 pyatlan-0.0.25/pyatlan/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   783914 2023-05-02 14:02:05.000000 pyatlan-0.0.25/pyatlan/model/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-05-02 14:02:05.000000 pyatlan-0.0.25/pyatlan/model/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-05-02 14:02:05.000000 pyatlan-0.0.25/pyatlan/model/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-02 14:02:05.000000 pyatlan-0.0.25/pyatlan/model/internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-05-02 14:02:05.000000 pyatlan-0.0.25/pyatlan/model/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-02 14:02:05.000000 pyatlan-0.0.25/pyatlan/model/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    58716 2023-05-02 14:02:05.000000 pyatlan-0.0.25/pyatlan/model/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-05-02 14:02:05.000000 pyatlan-0.0.25/pyatlan/model/structs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16433 2023-05-02 14:02:05.000000 pyatlan-0.0.25/pyatlan/model/typedef.py
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-05-02 14:02:05.000000 pyatlan-0.0.25/pyatlan/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-02 14:02:05.000000 pyatlan-0.0.25/pyatlan/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:02:19.974967 pyatlan-0.0.25/pyatlan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-02 14:02:19.000000 pyatlan-0.0.25/pyatlan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-02 14:02:19.000000 pyatlan-0.0.25/pyatlan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 14:02:19.000000 pyatlan-0.0.25/pyatlan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 14:02:19.000000 pyatlan-0.0.25/pyatlan.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-02 14:02:19.000000 pyatlan-0.0.25/pyatlan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-02 14:02:19.000000 pyatlan-0.0.25/pyatlan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 14:02:19.986967 pyatlan-0.0.25/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-02 14:02:05.000000 pyatlan-0.0.25/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:02:19.982967 pyatlan-0.0.25/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-02 14:02:05.000000 pyatlan-0.0.25/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:02:19.982967 pyatlan-0.0.25/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-02 14:02:05.000000 pyatlan-0.0.25/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-02 14:02:05.000000 pyatlan-0.0.25/tests/integration/classification_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-05-02 14:02:05.000000 pyatlan-0.0.25/tests/integration/custom_metadata_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-02 14:02:05.000000 pyatlan-0.0.25/tests/integration/role_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-02 14:02:05.000000 pyatlan-0.0.25/tests/integration/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    32057 2023-05-02 14:02:05.000000 pyatlan-0.0.25/tests/integration/test_entity_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-05-02 14:02:05.000000 pyatlan-0.0.25/tests/integration/test_index_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:02:19.986967 pyatlan-0.0.25/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-02 14:02:05.000000 pyatlan-0.0.25/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-05-02 14:02:05.000000 pyatlan-0.0.25/tests/unit/test_classification_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-05-02 14:02:05.000000 pyatlan-0.0.25/tests/unit/test_glossary_term.py
--rw-r--r--   0 runner    (1001) docker     (123)    51299 2023-05-02 14:02:05.000000 pyatlan-0.0.25/tests/unit/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    31771 2023-05-02 14:02:05.000000 pyatlan-0.0.25/tests/unit/test_search_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8483 2023-05-02 14:02:05.000000 pyatlan-0.0.25/tests/unit/test_typedef_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-02 14:02:05.000000 pyatlan-0.0.25/tests/unit/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:48:25.281848 pyatlan-0.0.26/
+-rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-05-04 15:48:12.000000 pyatlan-0.0.26/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-04 15:48:12.000000 pyatlan-0.0.26/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-04 15:48:12.000000 pyatlan-0.0.26/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-04 15:48:25.281848 pyatlan-0.0.26/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-04 15:48:12.000000 pyatlan-0.0.26/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:48:25.273848 pyatlan-0.0.26/pyatlan/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-04 15:48:12.000000 pyatlan-0.0.26/pyatlan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:48:25.273848 pyatlan-0.0.26/pyatlan/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-04 15:48:12.000000 pyatlan-0.0.26/pyatlan/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-05-04 15:48:12.000000 pyatlan-0.0.26/pyatlan/cache/classification_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9761 2023-05-04 15:48:12.000000 pyatlan-0.0.26/pyatlan/cache/custom_metadata_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-04 15:48:12.000000 pyatlan-0.0.26/pyatlan/cache/role_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:48:25.277848 pyatlan-0.0.26/pyatlan/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-04 15:48:12.000000 pyatlan-0.0.26/pyatlan/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24499 2023-05-04 15:48:12.000000 pyatlan-0.0.26/pyatlan/client/atlan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-05-04 15:48:12.000000 pyatlan-0.0.26/pyatlan/client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-05-04 15:48:12.000000 pyatlan-0.0.26/pyatlan/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-05-04 15:48:12.000000 pyatlan-0.0.26/pyatlan/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:48:25.277848 pyatlan-0.0.26/pyatlan/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-04 15:48:12.000000 pyatlan-0.0.26/pyatlan/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-05-04 15:48:12.000000 pyatlan-0.0.26/pyatlan/generator/generate_from_typdefs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:48:25.277848 pyatlan-0.0.26/pyatlan/generator/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-04 15:48:12.000000 pyatlan-0.0.26/pyatlan/generator/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:48:25.277848 pyatlan-0.0.26/pyatlan/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-04 15:48:12.000000 pyatlan-0.0.26/pyatlan/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   866175 2023-05-04 15:48:12.000000 pyatlan-0.0.26/pyatlan/model/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-05-04 15:48:12.000000 pyatlan-0.0.26/pyatlan/model/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-05-04 15:48:12.000000 pyatlan-0.0.26/pyatlan/model/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-04 15:48:12.000000 pyatlan-0.0.26/pyatlan/model/internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-05-04 15:48:12.000000 pyatlan-0.0.26/pyatlan/model/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-04 15:48:12.000000 pyatlan-0.0.26/pyatlan/model/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58716 2023-05-04 15:48:12.000000 pyatlan-0.0.26/pyatlan/model/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-05-04 15:48:12.000000 pyatlan-0.0.26/pyatlan/model/structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16433 2023-05-04 15:48:12.000000 pyatlan-0.0.26/pyatlan/model/typedef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-05-04 15:48:12.000000 pyatlan-0.0.26/pyatlan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-04 15:48:12.000000 pyatlan-0.0.26/pyatlan/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:48:25.273848 pyatlan-0.0.26/pyatlan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-04 15:48:25.000000 pyatlan-0.0.26/pyatlan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-04 15:48:25.000000 pyatlan-0.0.26/pyatlan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 15:48:25.000000 pyatlan-0.0.26/pyatlan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 15:48:25.000000 pyatlan-0.0.26/pyatlan.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-04 15:48:25.000000 pyatlan-0.0.26/pyatlan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-04 15:48:25.000000 pyatlan-0.0.26/pyatlan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 15:48:25.281848 pyatlan-0.0.26/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-04 15:48:12.000000 pyatlan-0.0.26/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:48:25.277848 pyatlan-0.0.26/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-04 15:48:12.000000 pyatlan-0.0.26/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:48:25.281848 pyatlan-0.0.26/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-04 15:48:12.000000 pyatlan-0.0.26/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-04 15:48:12.000000 pyatlan-0.0.26/tests/integration/classification_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-05-04 15:48:12.000000 pyatlan-0.0.26/tests/integration/custom_metadata_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-04 15:48:12.000000 pyatlan-0.0.26/tests/integration/role_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6901 2023-05-04 15:48:12.000000 pyatlan-0.0.26/tests/integration/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32057 2023-05-04 15:48:12.000000 pyatlan-0.0.26/tests/integration/test_entity_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-05-04 15:48:12.000000 pyatlan-0.0.26/tests/integration/test_index_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:48:25.281848 pyatlan-0.0.26/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-04 15:48:12.000000 pyatlan-0.0.26/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-05-04 15:48:12.000000 pyatlan-0.0.26/tests/unit/test_classification_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-05-04 15:48:12.000000 pyatlan-0.0.26/tests/unit/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-05-04 15:48:12.000000 pyatlan-0.0.26/tests/unit/test_glossary_term.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51397 2023-05-04 15:48:12.000000 pyatlan-0.0.26/tests/unit/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31771 2023-05-04 15:48:12.000000 pyatlan-0.0.26/tests/unit/test_search_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8483 2023-05-04 15:48:12.000000 pyatlan-0.0.26/tests/unit/test_typedef_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-04 15:48:12.000000 pyatlan-0.0.26/tests/unit/test_utils.py
```

### Comparing `pyatlan-0.0.25/LICENSE` & `pyatlan-0.0.26/LICENSE`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.25/PKG-INFO` & `pyatlan-0.0.26/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatlan
-Version: 0.0.25
+Version: 0.0.26
 Summary: Atlan Python Client
 Home-page: https://github.com/atlanhq/atlan-python
 Author: Atlan Technologies Pvt Ltd
 Author-email: engineering@atlan.com
 License: Apache LICENSE 2.0
 Keywords: atlan client
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyatlan-0.0.25/README.md` & `pyatlan-0.0.26/README.md`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.25/pyatlan/cache/classification_cache.py` & `pyatlan-0.0.26/pyatlan/cache/classification_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.25/pyatlan/cache/custom_metadata_cache.py` & `pyatlan-0.0.26/pyatlan/cache/custom_metadata_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.25/pyatlan/cache/role_cache.py` & `pyatlan-0.0.26/pyatlan/cache/role_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.25/pyatlan/client/atlan.py` & `pyatlan-0.0.26/pyatlan/client/atlan.py`

 * *Files 12% similar despite different names*

```diff
@@ -309,16 +309,15 @@
                     asset_type.__name__
                 ),
                 query_params,
             )
             raw_json["entity"]["attributes"].update(
                 raw_json["entity"]["relationshipAttributes"]
             )
-            asset = AssetResponse[A](**raw_json).entity
-            asset.is_incomplete = False
+            asset = self.handle_relationships(raw_json)
             if not isinstance(asset, asset_type):
                 raise NotFoundError(
                     message=f"Asset with qualifiedName {qualified_name} "
                     f"is not of the type requested: {asset_type.__name__}.",
                     code="ATLAN-PYTHON-404-002",
                 )
             return asset
@@ -341,35 +340,39 @@
         }
 
         try:
             raw_json = self._call_api(
                 GET_ENTITY_BY_GUID.format_path_with_params(guid),
                 query_params,
             )
-            if (
-                "relationshipAttributes" in raw_json["entity"]
-                and raw_json["entity"]["relationshipAttributes"]
-            ):
-                raw_json["entity"]["attributes"].update(
-                    raw_json["entity"]["relationshipAttributes"]
-                )
-            raw_json["entity"]["relationshipAttributes"] = {}
-            asset = AssetResponse[A](**raw_json).entity
-            asset.is_incomplete = False
+            asset = self.handle_relationships(raw_json)
             if not isinstance(asset, asset_type):
                 raise NotFoundError(
                     message=f"Asset with GUID {guid} is not of the type requested: {asset_type.__name__}.",
                     code="ATLAN-PYTHON-404-002",
                 )
             return asset
         except AtlanError as ae:
             if ae.status_code == HTTPStatus.NOT_FOUND:
                 raise NotFoundError(message=ae.user_message, code=ae.code) from ae
             raise ae
 
+    def handle_relationships(self, raw_json):
+        if (
+            "relationshipAttributes" in raw_json["entity"]
+            and raw_json["entity"]["relationshipAttributes"]
+        ):
+            raw_json["entity"]["attributes"].update(
+                raw_json["entity"]["relationshipAttributes"]
+            )
+        raw_json["entity"]["relationshipAttributes"] = {}
+        asset = AssetResponse[A](**raw_json).entity
+        asset.is_incomplete = False
+        return asset
+
     @validate_arguments()
     def retrieve_minimal(self, guid: str, asset_type: Type[A]) -> A:
         return self.get_asset_by_guid(
             guid=guid,
             asset_type=asset_type,
             min_ext_info=True,
             ignore_relationships=True,
@@ -598,7 +601,104 @@
         self._call_api(
             ADD_BUSINESS_ATTRIBUTE_BY_ID.format_path(
                 {"entity_guid": guid, "bm_id": custom_metadata._meta_data_type_id}
             ),
             None,
             custom_metadata_request,
         )
+
+    @validate_arguments()
+    def append_terms(
+        self,
+        asset_type: Type[A],
+        terms: list[AtlasGlossaryTerm],
+        guid: Optional[str] = None,
+        qualified_name: Optional[str] = None,
+    ) -> A:
+        if guid:
+            if qualified_name:
+                raise ValueError(
+                    "Either guid or qualified_name can be be specified not both"
+                )
+            asset = self.get_asset_by_guid(guid=guid, asset_type=asset_type)
+        elif qualified_name:
+            asset = self.get_asset_by_qualified_name(
+                qualified_name=qualified_name, asset_type=asset_type
+            )
+        else:
+            raise ValueError("Either guid or qualified name must be specified")
+        if not terms:
+            return asset
+        replacement_terms: list[AtlasGlossaryTerm] = []
+        if existing_terms := asset.terms:
+            replacement_terms.extend(
+                term for term in existing_terms if term.relationship_status != "DELETED"
+            )
+        replacement_terms.extend(terms)
+        asset.terms = replacement_terms
+        response = self.upsert(entity=asset)
+        if assets := response.assets_updated(asset_type=asset_type):
+            return assets[0]
+        return asset
+
+    @validate_arguments()
+    def replace_terms(
+        self,
+        asset_type: Type[A],
+        terms: list[AtlasGlossaryTerm],
+        guid: Optional[str] = None,
+        qualified_name: Optional[str] = None,
+    ) -> A:
+        if guid:
+            if qualified_name:
+                raise ValueError(
+                    "Either guid or qualified_name can be be specified not both"
+                )
+            asset = self.get_asset_by_guid(guid=guid, asset_type=asset_type)
+        elif qualified_name:
+            asset = self.get_asset_by_qualified_name(
+                qualified_name=qualified_name, asset_type=asset_type
+            )
+        else:
+            raise ValueError("Either guid or qualified name must be specified")
+        asset.terms = terms
+        response = self.upsert(entity=asset)
+        if assets := response.assets_updated(asset_type=asset_type):
+            return assets[0]
+        return asset
+
+    @validate_arguments()
+    def remove_terms(
+        self,
+        asset_type: Type[A],
+        terms: list[AtlasGlossaryTerm],
+        guid: Optional[str] = None,
+        qualified_name: Optional[str] = None,
+    ) -> A:
+        if not terms:
+            raise ValueError("A list of terms to remove must be specified")
+        if guid:
+            if qualified_name:
+                raise ValueError(
+                    "Either guid or qualified_name can be be specified not both"
+                )
+            asset = self.get_asset_by_guid(guid=guid, asset_type=asset_type)
+        elif qualified_name:
+            asset = self.get_asset_by_qualified_name(
+                qualified_name=qualified_name, asset_type=asset_type
+            )
+        else:
+            raise ValueError("Either guid or qualified name must be specified")
+        replacement_terms: list[AtlasGlossaryTerm] = []
+        guids_to_be_removed = {t.guid for t in terms}
+        if existing_terms := asset.terms:
+            replacement_terms.extend(
+                term
+                for term in existing_terms
+                if term.relationship_status != "DELETED"
+                and term.guid not in guids_to_be_removed
+            )
+        asset.terms = replacement_terms
+        response = self.upsert(entity=asset)
+        if assets := response.assets_updated(asset_type=asset_type):
+            return assets[0]
+        return asset
```

### Comparing `pyatlan-0.0.25/pyatlan/client/constants.py` & `pyatlan-0.0.26/pyatlan/client/constants.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.25/pyatlan/error.py` & `pyatlan-0.0.26/pyatlan/error.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.25/pyatlan/exceptions.py` & `pyatlan-0.0.26/pyatlan/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.25/pyatlan/generator/generate_from_typdefs.py` & `pyatlan-0.0.26/pyatlan/generator/generate_from_typdefs.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.25/pyatlan/model/assets.py` & `pyatlan-0.0.26/pyatlan/model/assets.py`

 * *Files 5% similar despite different names*

```diff
@@ -96,14 +96,15 @@
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "qualified_name",
         "replicated_from",
         "replicated_to",
+        "terms",
     ]
 
     @property
     def qualified_name(self) -> str:
         return self.attributes.qualified_name
 
     @qualified_name.setter
@@ -128,14 +129,26 @@
 
     @replicated_to.setter
     def replicated_to(self, replicated_to: Optional[list[AtlasServer]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.replicated_to = replicated_to
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     class Attributes(AtlanObject):
         qualified_name: str = Field("", description="", alias="qualifiedName")
         replicated_from: Optional[list[AtlasServer]] = Field(
             None, description="", alias="replicatedFrom"
         )
         replicated_to: Optional[list[AtlasServer]] = Field(
             None, description="", alias="replicatedTo"
@@ -396,14 +409,15 @@
         "asset_dbt_environment_name",
         "asset_dbt_environment_dbt_version",
         "asset_dbt_tags",
         "asset_dbt_semantic_layer_proxy_url",
         "asset_dbt_source_freshness_criteria",
         "sample_data_url",
         "asset_tags",
+        "terms",
     ]
 
     @property
     def name(self) -> str:
         return self.attributes.name
 
     @name.setter
@@ -1501,14 +1515,26 @@
 
     @asset_tags.setter
     def asset_tags(self, asset_tags: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_tags = asset_tags
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     _subtypes_: dict[str, type] = dict()
 
     def __init_subclass__(cls, type_name=None):
         cls._subtypes_[type_name or cls.__name__.lower()] = cls
 
     @classmethod
     def create_for_modification(
@@ -1926,14 +1952,15 @@
 
     _convience_properties: ClassVar[list[str]] = [
         "short_description",
         "long_description",
         "language",
         "usage",
         "additional_attributes",
+        "terms",
     ]
 
     @property
     def short_description(self) -> Optional[str]:
         return self.attributes.short_description
 
     @short_description.setter
@@ -1978,14 +2005,26 @@
 
     @additional_attributes.setter
     def additional_attributes(self, additional_attributes: Optional[dict[str, str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.additional_attributes = additional_attributes
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("AtlasGlossary", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "AtlasGlossary":
             raise ValueError("must be AtlasGlossary")
         return v
@@ -2054,15 +2093,29 @@
     """Description"""
 
     def __setattr__(self, name, value):
         if name in DataSet._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
-    _convience_properties: ClassVar[list[str]] = []
+    _convience_properties: ClassVar[list[str]] = [
+        "terms",
+    ]
+
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
 
     type_name: str = Field("DataSet", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "DataSet":
             raise ValueError("must be DataSet")
@@ -2093,15 +2146,29 @@
     """Description"""
 
     def __setattr__(self, name, value):
         if name in ProcessExecution._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
-    _convience_properties: ClassVar[list[str]] = []
+    _convience_properties: ClassVar[list[str]] = [
+        "terms",
+    ]
+
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
 
     type_name: str = Field("ProcessExecution", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "ProcessExecution":
             raise ValueError("must be ProcessExecution")
@@ -2139,14 +2206,15 @@
     _convience_properties: ClassVar[list[str]] = [
         "short_description",
         "long_description",
         "examples",
         "abbreviation",
         "usage",
         "additional_attributes",
+        "terms",
     ]
 
     @property
     def short_description(self) -> Optional[str]:
         return self.attributes.short_description
 
     @short_description.setter
@@ -2201,14 +2269,26 @@
 
     @additional_attributes.setter
     def additional_attributes(self, additional_attributes: Optional[dict[str, str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.additional_attributes = additional_attributes
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("AtlasGlossaryTerm", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "AtlasGlossaryTerm":
             raise ValueError("must be AtlasGlossaryTerm")
         return v
@@ -2378,15 +2458,29 @@
     """Description"""
 
     def __setattr__(self, name, value):
         if name in Cloud._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
-    _convience_properties: ClassVar[list[str]] = []
+    _convience_properties: ClassVar[list[str]] = [
+        "terms",
+    ]
+
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
 
     type_name: str = Field("Cloud", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Cloud":
             raise ValueError("must be Cloud")
@@ -2417,15 +2511,29 @@
     """Description"""
 
     def __setattr__(self, name, value):
         if name in Infrastructure._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
-    _convience_properties: ClassVar[list[str]] = []
+    _convience_properties: ClassVar[list[str]] = [
+        "terms",
+    ]
+
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
 
     type_name: str = Field("Infrastructure", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Infrastructure":
             raise ValueError("must be Infrastructure")
@@ -2478,14 +2586,15 @@
         "connector_icon",
         "connector_image",
         "source_logo",
         "is_sample_data_preview_enabled",
         "popularity_insights_timeframe",
         "has_popularity_insights",
         "connection_dbt_environments",
+        "terms",
     ]
 
     @property
     def category(self) -> Optional[str]:
         return self.attributes.category
 
     @category.setter
@@ -2698,14 +2807,26 @@
     def connection_dbt_environments(
         self, connection_dbt_environments: Optional[set[str]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.connection_dbt_environments = connection_dbt_environments
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("Connection", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Connection":
             raise ValueError("must be Connection")
         return v
@@ -2861,14 +2982,15 @@
 
     _convience_properties: ClassVar[list[str]] = [
         "inputs",
         "outputs",
         "code",
         "sql",
         "ast",
+        "terms",
     ]
 
     @property
     def inputs(self) -> Optional[list[Catalog]]:
         return self.attributes.inputs
 
     @inputs.setter
@@ -2913,14 +3035,26 @@
 
     @ast.setter
     def ast(self, ast: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.ast = ast
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("Process", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Process":
             raise ValueError("must be Process")
         return v
@@ -2962,14 +3096,15 @@
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "short_description",
         "long_description",
         "additional_attributes",
+        "terms",
     ]
 
     @property
     def short_description(self) -> Optional[str]:
         return self.attributes.short_description
 
     @short_description.setter
@@ -2994,14 +3129,26 @@
 
     @additional_attributes.setter
     def additional_attributes(self, additional_attributes: Optional[dict[str, str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.additional_attributes = additional_attributes
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("AtlasGlossaryCategory", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "AtlasGlossaryCategory":
             raise ValueError("must be AtlasGlossaryCategory")
         return v
@@ -3098,14 +3245,15 @@
         if name in Badge._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "badge_conditions",
         "badge_metadata_attribute",
+        "terms",
     ]
 
     @property
     def badge_conditions(self) -> Optional[list[BadgeCondition]]:
         return self.attributes.badge_conditions
 
     @badge_conditions.setter
@@ -3120,14 +3268,26 @@
 
     @badge_metadata_attribute.setter
     def badge_metadata_attribute(self, badge_metadata_attribute: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.badge_metadata_attribute = badge_metadata_attribute
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("Badge", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Badge":
             raise ValueError("must be Badge")
         return v
@@ -3163,15 +3323,29 @@
     """Description"""
 
     def __setattr__(self, name, value):
         if name in Namespace._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
-    _convience_properties: ClassVar[list[str]] = []
+    _convience_properties: ClassVar[list[str]] = [
+        "terms",
+    ]
+
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
 
     type_name: str = Field("Namespace", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Namespace":
             raise ValueError("must be Namespace")
@@ -3208,15 +3382,29 @@
     """Description"""
 
     def __setattr__(self, name, value):
         if name in Catalog._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
-    _convience_properties: ClassVar[list[str]] = []
+    _convience_properties: ClassVar[list[str]] = [
+        "terms",
+    ]
+
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
 
     type_name: str = Field("Catalog", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Catalog":
             raise ValueError("must be Catalog")
@@ -3262,14 +3450,15 @@
         "google_project_name",
         "google_project_id",
         "google_project_number",
         "google_location",
         "google_location_type",
         "google_labels",
         "google_tags",
+        "terms",
     ]
 
     @property
     def google_service(self) -> Optional[str]:
         return self.attributes.google_service
 
     @google_service.setter
@@ -3344,14 +3533,26 @@
 
     @google_tags.setter
     def google_tags(self, google_tags: Optional[list[GoogleTag]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.google_tags = google_tags
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("Google", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Google":
             raise ValueError("must be Google")
         return v
@@ -3410,14 +3611,15 @@
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "azure_resource_id",
         "azure_location",
         "adls_account_secondary_location",
         "azure_tags",
+        "terms",
     ]
 
     @property
     def azure_resource_id(self) -> Optional[str]:
         return self.attributes.azure_resource_id
 
     @azure_resource_id.setter
@@ -3456,14 +3658,26 @@
 
     @azure_tags.setter
     def azure_tags(self, azure_tags: Optional[list[AzureTag]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.azure_tags = azure_tags
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("Azure", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Azure":
             raise ValueError("must be Azure")
         return v
@@ -3515,14 +3729,15 @@
         "aws_service",
         "aws_region",
         "aws_account_id",
         "aws_resource_id",
         "aws_owner_name",
         "aws_owner_id",
         "aws_tags",
+        "terms",
     ]
 
     @property
     def aws_arn(self) -> Optional[str]:
         return self.attributes.aws_arn
 
     @aws_arn.setter
@@ -3607,14 +3822,26 @@
 
     @aws_tags.setter
     def aws_tags(self, aws_tags: Optional[list[AwsTag]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.aws_tags = aws_tags
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("AWS", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "AWS":
             raise ValueError("must be AWS")
         return v
@@ -3659,15 +3886,29 @@
     """Description"""
 
     def __setattr__(self, name, value):
         if name in BIProcess._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
-    _convience_properties: ClassVar[list[str]] = []
+    _convience_properties: ClassVar[list[str]] = [
+        "terms",
+    ]
+
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
 
     type_name: str = Field("BIProcess", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "BIProcess":
             raise ValueError("must be BIProcess")
@@ -3707,15 +3948,29 @@
     """Description"""
 
     def __setattr__(self, name, value):
         if name in ColumnProcess._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
-    _convience_properties: ClassVar[list[str]] = []
+    _convience_properties: ClassVar[list[str]] = [
+        "terms",
+    ]
+
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
 
     type_name: str = Field("ColumnProcess", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "ColumnProcess":
             raise ValueError("must be ColumnProcess")
@@ -3761,14 +4016,15 @@
         if name in Collection._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "icon",
         "icon_type",
+        "terms",
     ]
 
     @property
     def icon(self) -> Optional[str]:
         return self.attributes.icon
 
     @icon.setter
@@ -3783,14 +4039,26 @@
 
     @icon_type.setter
     def icon_type(self, icon_type: Optional[IconType]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.icon_type = icon_type
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("Collection", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Collection":
             raise ValueError("must be Collection")
         return v
@@ -3831,14 +4099,15 @@
         if name in Folder._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "parent_qualified_name",
         "collection_qualified_name",
+        "terms",
     ]
 
     @property
     def parent_qualified_name(self) -> str:
         return self.attributes.parent_qualified_name
 
     @parent_qualified_name.setter
@@ -3853,14 +4122,26 @@
 
     @collection_qualified_name.setter
     def collection_qualified_name(self, collection_qualified_name: str):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.collection_qualified_name = collection_qualified_name
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("Folder", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Folder":
             raise ValueError("must be Folder")
         return v
@@ -3903,15 +4184,29 @@
     """Description"""
 
     def __setattr__(self, name, value):
         if name in EventStore._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
-    _convience_properties: ClassVar[list[str]] = []
+    _convience_properties: ClassVar[list[str]] = [
+        "terms",
+    ]
+
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
 
     type_name: str = Field("EventStore", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "EventStore":
             raise ValueError("must be EventStore")
@@ -3948,15 +4243,29 @@
     """Description"""
 
     def __setattr__(self, name, value):
         if name in ObjectStore._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
-    _convience_properties: ClassVar[list[str]] = []
+    _convience_properties: ClassVar[list[str]] = [
+        "terms",
+    ]
+
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
 
     type_name: str = Field("ObjectStore", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "ObjectStore":
             raise ValueError("must be ObjectStore")
@@ -3993,15 +4302,29 @@
     """Description"""
 
     def __setattr__(self, name, value):
         if name in DataQuality._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
-    _convience_properties: ClassVar[list[str]] = []
+    _convience_properties: ClassVar[list[str]] = [
+        "terms",
+    ]
+
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
 
     type_name: str = Field("DataQuality", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "DataQuality":
             raise ValueError("must be DataQuality")
@@ -4038,15 +4361,29 @@
     """Description"""
 
     def __setattr__(self, name, value):
         if name in BI._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
-    _convience_properties: ClassVar[list[str]] = []
+    _convience_properties: ClassVar[list[str]] = [
+        "terms",
+    ]
+
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
 
     type_name: str = Field("BI", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "BI":
             raise ValueError("must be BI")
@@ -4083,15 +4420,29 @@
     """Description"""
 
     def __setattr__(self, name, value):
         if name in SaaS._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
-    _convience_properties: ClassVar[list[str]] = []
+    _convience_properties: ClassVar[list[str]] = [
+        "terms",
+    ]
+
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
 
     type_name: str = Field("SaaS", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "SaaS":
             raise ValueError("must be SaaS")
@@ -4147,14 +4498,15 @@
         "dbt_job_next_run",
         "dbt_job_next_run_humanized",
         "dbt_environment_name",
         "dbt_environment_dbt_version",
         "dbt_tags",
         "dbt_connection_context",
         "dbt_semantic_layer_proxy_url",
+        "terms",
     ]
 
     @property
     def dbt_alias(self) -> Optional[str]:
         return self.attributes.dbt_alias
 
     @dbt_alias.setter
@@ -4333,14 +4685,26 @@
 
     @dbt_semantic_layer_proxy_url.setter
     def dbt_semantic_layer_proxy_url(self, dbt_semantic_layer_proxy_url: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_semantic_layer_proxy_url = dbt_semantic_layer_proxy_url
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("Dbt", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Dbt":
             raise ValueError("must be Dbt")
         return v
@@ -4425,14 +4789,15 @@
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "link",
         "is_global",
         "reference",
         "resource_metadata",
+        "terms",
     ]
 
     @property
     def link(self) -> Optional[str]:
         return self.attributes.link
 
     @link.setter
@@ -4467,14 +4832,26 @@
 
     @resource_metadata.setter
     def resource_metadata(self, resource_metadata: Optional[dict[str, str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.resource_metadata = resource_metadata
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("Resource", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Resource":
             raise ValueError("must be Resource")
         return v
@@ -4516,15 +4893,29 @@
     """Description"""
 
     def __setattr__(self, name, value):
         if name in Insight._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
-    _convience_properties: ClassVar[list[str]] = []
+    _convience_properties: ClassVar[list[str]] = [
+        "terms",
+    ]
+
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
 
     type_name: str = Field("Insight", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Insight":
             raise ValueError("must be Insight")
@@ -4568,14 +4959,15 @@
     _convience_properties: ClassVar[list[str]] = [
         "api_spec_type",
         "api_spec_version",
         "api_spec_name",
         "api_spec_qualified_name",
         "api_external_docs",
         "api_is_auth_optional",
+        "terms",
     ]
 
     @property
     def api_spec_type(self) -> Optional[str]:
         return self.attributes.api_spec_type
 
     @api_spec_type.setter
@@ -4630,14 +5022,26 @@
 
     @api_is_auth_optional.setter
     def api_is_auth_optional(self, api_is_auth_optional: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.api_is_auth_optional = api_is_auth_optional
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("API", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "API":
             raise ValueError("must be API")
         return v
@@ -4702,14 +5106,15 @@
         "schema_qualified_name",
         "table_name",
         "table_qualified_name",
         "view_name",
         "view_qualified_name",
         "is_profiled",
         "last_profiled_at",
+        "terms",
     ]
 
     @property
     def query_count(self) -> Optional[int]:
         return self.attributes.query_count
 
     @query_count.setter
@@ -4844,14 +5249,26 @@
 
     @last_profiled_at.setter
     def last_profiled_at(self, last_profiled_at: Optional[datetime]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.last_profiled_at = last_profiled_at
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("SQL", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "SQL":
             raise ValueError("must be SQL")
         return v
@@ -4938,14 +5355,15 @@
         "google_project_name",
         "google_project_id",
         "google_project_number",
         "google_location",
         "google_location_type",
         "google_labels",
         "google_tags",
+        "terms",
     ]
 
     @property
     def google_service(self) -> Optional[str]:
         return self.attributes.google_service
 
     @google_service.setter
@@ -5020,14 +5438,26 @@
 
     @google_tags.setter
     def google_tags(self, google_tags: Optional[list[GoogleTag]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.google_tags = google_tags
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("DataStudio", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "DataStudio":
             raise ValueError("must be DataStudio")
         return v
@@ -5102,14 +5532,15 @@
         "google_project_name",
         "google_project_id",
         "google_project_number",
         "google_location",
         "google_location_type",
         "google_labels",
         "google_tags",
+        "terms",
     ]
 
     @property
     def gcs_storage_class(self) -> Optional[str]:
         return self.attributes.gcs_storage_class
 
     @gcs_storage_class.setter
@@ -5244,14 +5675,26 @@
 
     @google_tags.setter
     def google_tags(self, google_tags: Optional[list[GoogleTag]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.google_tags = google_tags
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("GCS", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "GCS":
             raise ValueError("must be GCS")
         return v
@@ -5340,14 +5783,15 @@
         "google_project_name",
         "google_project_id",
         "google_project_number",
         "google_location",
         "google_location_type",
         "google_labels",
         "google_tags",
+        "terms",
     ]
 
     @property
     def data_studio_asset_type(self) -> Optional[GoogleDatastudioAssetType]:
         return self.attributes.data_studio_asset_type
 
     @data_studio_asset_type.setter
@@ -5466,14 +5910,26 @@
 
     @google_tags.setter
     def google_tags(self, google_tags: Optional[list[GoogleTag]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.google_tags = google_tags
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("DataStudioAsset", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "DataStudioAsset":
             raise ValueError("must be DataStudioAsset")
         return v
@@ -5551,14 +6007,15 @@
 
     _convience_properties: ClassVar[list[str]] = [
         "adls_account_qualified_name",
         "azure_resource_id",
         "azure_location",
         "adls_account_secondary_location",
         "azure_tags",
+        "terms",
     ]
 
     @property
     def adls_account_qualified_name(self) -> Optional[str]:
         return self.attributes.adls_account_qualified_name
 
     @adls_account_qualified_name.setter
@@ -5607,14 +6064,26 @@
 
     @azure_tags.setter
     def azure_tags(self, azure_tags: Optional[list[AzureTag]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.azure_tags = azure_tags
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("ADLS", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "ADLS":
             raise ValueError("must be ADLS")
         return v
@@ -5677,14 +6146,15 @@
         "aws_service",
         "aws_region",
         "aws_account_id",
         "aws_resource_id",
         "aws_owner_name",
         "aws_owner_id",
         "aws_tags",
+        "terms",
     ]
 
     @property
     def s3_e_tag(self) -> Optional[str]:
         return self.attributes.s3_e_tag
 
     @s3_e_tag.setter
@@ -5789,14 +6259,26 @@
 
     @aws_tags.setter
     def aws_tags(self, aws_tags: Optional[list[AwsTag]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.aws_tags = aws_tags
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("S3", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "S3":
             raise ValueError("must be S3")
         return v
@@ -5874,14 +6356,15 @@
         "dbt_connection_context",
         "dbt_semantic_layer_proxy_url",
         "inputs",
         "outputs",
         "code",
         "sql",
         "ast",
+        "terms",
     ]
 
     @property
     def dbt_column_process_job_status(self) -> Optional[str]:
         return self.attributes.dbt_column_process_job_status
 
     @dbt_column_process_job_status.setter
@@ -6122,14 +6605,26 @@
 
     @ast.setter
     def ast(self, ast: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.ast = ast
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("DbtColumnProcess", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "DbtColumnProcess":
             raise ValueError("must be DbtColumnProcess")
         return v
@@ -6223,15 +6718,29 @@
     """Description"""
 
     def __setattr__(self, name, value):
         if name in Kafka._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
-    _convience_properties: ClassVar[list[str]] = []
+    _convience_properties: ClassVar[list[str]] = [
+        "terms",
+    ]
+
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
 
     type_name: str = Field("Kafka", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Kafka":
             raise ValueError("must be Kafka")
@@ -6273,14 +6782,15 @@
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "metric_type",
         "metric_s_q_l",
         "metric_filters",
         "metric_time_grains",
+        "terms",
     ]
 
     @property
     def metric_type(self) -> Optional[str]:
         return self.attributes.metric_type
 
     @metric_type.setter
@@ -6315,14 +6825,26 @@
 
     @metric_time_grains.setter
     def metric_time_grains(self, metric_time_grains: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.metric_time_grains = metric_time_grains
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("Metric", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Metric":
             raise ValueError("must be Metric")
         return v
@@ -6378,14 +6900,15 @@
         if name in Metabase._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "metabase_collection_name",
         "metabase_collection_qualified_name",
+        "terms",
     ]
 
     @property
     def metabase_collection_name(self) -> Optional[str]:
         return self.attributes.metabase_collection_name
 
     @metabase_collection_name.setter
@@ -6404,14 +6927,26 @@
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.metabase_collection_qualified_name = (
             metabase_collection_qualified_name
         )
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("Metabase", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Metabase":
             raise ValueError("must be Metabase")
         return v
@@ -6457,14 +6992,15 @@
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "quick_sight_id",
         "quick_sight_sheet_id",
         "quick_sight_sheet_name",
+        "terms",
     ]
 
     @property
     def quick_sight_id(self) -> Optional[str]:
         return self.attributes.quick_sight_id
 
     @quick_sight_id.setter
@@ -6489,14 +7025,26 @@
 
     @quick_sight_sheet_name.setter
     def quick_sight_sheet_name(self, quick_sight_sheet_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.quick_sight_sheet_name = quick_sight_sheet_name
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("QuickSight", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "QuickSight":
             raise ValueError("must be QuickSight")
         return v
@@ -6544,14 +7092,15 @@
         if name in Thoughtspot._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "thoughtspot_chart_type",
         "thoughtspot_question_text",
+        "terms",
     ]
 
     @property
     def thoughtspot_chart_type(self) -> Optional[str]:
         return self.attributes.thoughtspot_chart_type
 
     @thoughtspot_chart_type.setter
@@ -6566,14 +7115,26 @@
 
     @thoughtspot_question_text.setter
     def thoughtspot_question_text(self, thoughtspot_question_text: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.thoughtspot_question_text = thoughtspot_question_text
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("Thoughtspot", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Thoughtspot":
             raise ValueError("must be Thoughtspot")
         return v
@@ -6620,14 +7181,15 @@
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "power_b_i_is_hidden",
         "power_b_i_table_qualified_name",
         "power_b_i_format_string",
         "power_b_i_endorsement",
+        "terms",
     ]
 
     @property
     def power_b_i_is_hidden(self) -> Optional[bool]:
         return self.attributes.power_b_i_is_hidden
 
     @power_b_i_is_hidden.setter
@@ -6666,14 +7228,26 @@
     def power_b_i_endorsement(
         self, power_b_i_endorsement: Optional[PowerbiEndorsement]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.power_b_i_endorsement = power_b_i_endorsement
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("PowerBI", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "PowerBI":
             raise ValueError("must be PowerBI")
         return v
@@ -6726,14 +7300,15 @@
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "preset_workspace_id",
         "preset_workspace_qualified_name",
         "preset_dashboard_id",
         "preset_dashboard_qualified_name",
+        "terms",
     ]
 
     @property
     def preset_workspace_id(self) -> Optional[int]:
         return self.attributes.preset_workspace_id
 
     @preset_workspace_id.setter
@@ -6776,14 +7351,26 @@
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.preset_dashboard_qualified_name = (
             preset_dashboard_qualified_name
         )
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("Preset", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Preset":
             raise ValueError("must be Preset")
         return v
@@ -6841,14 +7428,15 @@
         "mode_workspace_name",
         "mode_workspace_username",
         "mode_workspace_qualified_name",
         "mode_report_name",
         "mode_report_qualified_name",
         "mode_query_name",
         "mode_query_qualified_name",
+        "terms",
     ]
 
     @property
     def mode_id(self) -> Optional[str]:
         return self.attributes.mode_id
 
     @mode_id.setter
@@ -6935,14 +7523,26 @@
 
     @mode_query_qualified_name.setter
     def mode_query_qualified_name(self, mode_query_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mode_query_qualified_name = mode_query_qualified_name
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("Mode", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Mode":
             raise ValueError("must be Mode")
         return v
@@ -7008,14 +7608,15 @@
     _convience_properties: ClassVar[list[str]] = [
         "sigma_workbook_qualified_name",
         "sigma_workbook_name",
         "sigma_page_qualified_name",
         "sigma_page_name",
         "sigma_data_element_qualified_name",
         "sigma_data_element_name",
+        "terms",
     ]
 
     @property
     def sigma_workbook_qualified_name(self) -> Optional[str]:
         return self.attributes.sigma_workbook_qualified_name
 
     @sigma_workbook_qualified_name.setter
@@ -7076,14 +7677,26 @@
 
     @sigma_data_element_name.setter
     def sigma_data_element_name(self, sigma_data_element_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sigma_data_element_name = sigma_data_element_name
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("Sigma", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Sigma":
             raise ValueError("must be Sigma")
         return v
@@ -7146,14 +7759,15 @@
         "qlik_q_r_i",
         "qlik_space_id",
         "qlik_space_qualified_name",
         "qlik_app_id",
         "qlik_app_qualified_name",
         "qlik_owner_id",
         "qlik_is_published",
+        "terms",
     ]
 
     @property
     def qlik_id(self) -> Optional[str]:
         return self.attributes.qlik_id
 
     @qlik_id.setter
@@ -7228,14 +7842,26 @@
 
     @qlik_is_published.setter
     def qlik_is_published(self, qlik_is_published: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.qlik_is_published = qlik_is_published
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("Qlik", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Qlik":
             raise ValueError("must be Qlik")
         return v
@@ -7285,15 +7911,29 @@
     """Description"""
 
     def __setattr__(self, name, value):
         if name in Tableau._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
-    _convience_properties: ClassVar[list[str]] = []
+    _convience_properties: ClassVar[list[str]] = [
+        "terms",
+    ]
+
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
 
     type_name: str = Field("Tableau", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Tableau":
             raise ValueError("must be Tableau")
@@ -7330,15 +7970,29 @@
     """Description"""
 
     def __setattr__(self, name, value):
         if name in Looker._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
-    _convience_properties: ClassVar[list[str]] = []
+    _convience_properties: ClassVar[list[str]] = [
+        "terms",
+    ]
+
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
 
     type_name: str = Field("Looker", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Looker":
             raise ValueError("must be Looker")
@@ -7367,25 +8021,99 @@
     attributes: "Looker.Attributes" = Field(
         None,
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
+class Redash(BI):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in Redash._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "redash_is_published",
+        "terms",
+    ]
+
+    @property
+    def redash_is_published(self) -> Optional[bool]:
+        return self.attributes.redash_is_published
+
+    @redash_is_published.setter
+    def redash_is_published(self, redash_is_published: Optional[bool]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.redash_is_published = redash_is_published
+
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
+    type_name: str = Field("Redash", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "Redash":
+            raise ValueError("must be Redash")
+        return v
+
+    class Attributes(BI.Attributes):
+        redash_is_published: Optional[bool] = Field(
+            None, description="", alias="redashIsPublished"
+        )
+        input_to_processes: Optional[list[Process]] = Field(
+            None, description="", alias="inputToProcesses"
+        )  # relationship
+        links: Optional[list[Link]] = Field(
+            None, description="", alias="links"
+        )  # relationship
+        metrics: Optional[list[Metric]] = Field(
+            None, description="", alias="metrics"
+        )  # relationship
+        readme: Optional[Readme] = Field(
+            None, description="", alias="readme"
+        )  # relationship
+        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="meanings"
+        )  # relationship
+        output_from_processes: Optional[list[Process]] = Field(
+            None, description="", alias="outputFromProcesses"
+        )  # relationship
+
+    attributes: "Redash.Attributes" = Field(
+        None,
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
 class Salesforce(SaaS):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in Salesforce._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "organization_qualified_name",
         "api_name",
+        "terms",
     ]
 
     @property
     def organization_qualified_name(self) -> Optional[str]:
         return self.attributes.organization_qualified_name
 
     @organization_qualified_name.setter
@@ -7400,14 +8128,26 @@
 
     @api_name.setter
     def api_name(self, api_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.api_name = api_name
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("Salesforce", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Salesforce":
             raise ValueError("must be Salesforce")
         return v
@@ -7451,14 +8191,15 @@
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "dbt_model_qualified_name",
         "dbt_model_column_data_type",
         "dbt_model_column_order",
+        "terms",
     ]
 
     @property
     def dbt_model_qualified_name(self) -> Optional[str]:
         return self.attributes.dbt_model_qualified_name
 
     @dbt_model_qualified_name.setter
@@ -7483,14 +8224,26 @@
 
     @dbt_model_column_order.setter
     def dbt_model_column_order(self, dbt_model_column_order: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_model_column_order = dbt_model_column_order
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("DbtModelColumn", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "DbtModelColumn":
             raise ValueError("must be DbtModelColumn")
         return v
@@ -7558,14 +8311,15 @@
         "dbt_model_compile_started_at",
         "dbt_model_compile_completed_at",
         "dbt_model_execute_started_at",
         "dbt_model_execute_completed_at",
         "dbt_model_execution_time",
         "dbt_model_run_generated_at",
         "dbt_model_run_elapsed_time",
+        "terms",
     ]
 
     @property
     def dbt_status(self) -> Optional[str]:
         return self.attributes.dbt_status
 
     @dbt_status.setter
@@ -7700,14 +8454,26 @@
 
     @dbt_model_run_elapsed_time.setter
     def dbt_model_run_elapsed_time(self, dbt_model_run_elapsed_time: Optional[float]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_model_run_elapsed_time = dbt_model_run_elapsed_time
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("DbtModel", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "DbtModel":
             raise ValueError("must be DbtModel")
         return v
@@ -7810,14 +8576,15 @@
         "dbt_tags",
         "dbt_connection_context",
         "dbt_semantic_layer_proxy_url",
         "metric_type",
         "metric_s_q_l",
         "metric_filters",
         "metric_time_grains",
+        "terms",
     ]
 
     @property
     def dbt_metric_filters(self) -> Optional[list[DbtMetricFilter]]:
         return self.attributes.dbt_metric_filters
 
     @dbt_metric_filters.setter
@@ -8046,14 +8813,26 @@
 
     @metric_time_grains.setter
     def metric_time_grains(self, metric_time_grains: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.metric_time_grains = metric_time_grains
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("DbtMetric", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "DbtMetric":
             raise ValueError("must be DbtMetric")
         return v
@@ -8162,14 +8941,15 @@
         if name in DbtSource._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "dbt_state",
         "dbt_freshness_criteria",
+        "terms",
     ]
 
     @property
     def dbt_state(self) -> Optional[str]:
         return self.attributes.dbt_state
 
     @dbt_state.setter
@@ -8184,14 +8964,26 @@
 
     @dbt_freshness_criteria.setter
     def dbt_freshness_criteria(self, dbt_freshness_criteria: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_freshness_criteria = dbt_freshness_criteria
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("DbtSource", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "DbtSource":
             raise ValueError("must be DbtSource")
         return v
@@ -8262,14 +9054,15 @@
         "dbt_connection_context",
         "dbt_semantic_layer_proxy_url",
         "inputs",
         "outputs",
         "code",
         "sql",
         "ast",
+        "terms",
     ]
 
     @property
     def dbt_process_job_status(self) -> Optional[str]:
         return self.attributes.dbt_process_job_status
 
     @dbt_process_job_status.setter
@@ -8508,14 +9301,26 @@
 
     @ast.setter
     def ast(self, ast: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.ast = ast
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("DbtProcess", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "DbtProcess":
             raise ValueError("must be DbtProcess")
         return v
@@ -8609,14 +9414,15 @@
         if name in ReadmeTemplate._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "icon",
         "icon_type",
+        "terms",
     ]
 
     @property
     def icon(self) -> Optional[str]:
         return self.attributes.icon
 
     @icon.setter
@@ -8631,14 +9437,26 @@
 
     @icon_type.setter
     def icon_type(self, icon_type: Optional[IconType]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.icon_type = icon_type
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("ReadmeTemplate", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "ReadmeTemplate":
             raise ValueError("must be ReadmeTemplate")
         return v
@@ -8676,15 +9494,29 @@
     """Description"""
 
     def __setattr__(self, name, value):
         if name in Readme._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
-    _convience_properties: ClassVar[list[str]] = []
+    _convience_properties: ClassVar[list[str]] = [
+        "terms",
+    ]
+
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
 
     type_name: str = Field("Readme", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Readme":
             raise ValueError("must be Readme")
@@ -8781,14 +9613,15 @@
         if name in Link._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "icon",
         "icon_type",
+        "terms",
     ]
 
     @property
     def icon(self) -> Optional[str]:
         return self.attributes.icon
 
     @icon.setter
@@ -8803,14 +9636,26 @@
 
     @icon_type.setter
     def icon_type(self, icon_type: Optional[IconType]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.icon_type = icon_type
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("Link", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Link":
             raise ValueError("must be Link")
         return v
@@ -8863,14 +9708,15 @@
         "api_spec_contact_email",
         "api_spec_contact_name",
         "api_spec_contact_url",
         "api_spec_license_name",
         "api_spec_license_url",
         "api_spec_contract_version",
         "api_spec_service_alias",
+        "terms",
     ]
 
     @property
     def api_spec_terms_of_service_url(self) -> Optional[str]:
         return self.attributes.api_spec_terms_of_service_url
 
     @api_spec_terms_of_service_url.setter
@@ -8947,14 +9793,26 @@
 
     @api_spec_service_alias.setter
     def api_spec_service_alias(self, api_spec_service_alias: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.api_spec_service_alias = api_spec_service_alias
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("APISpec", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "APISpec":
             raise ValueError("must be APISpec")
         return v
@@ -9024,14 +9882,15 @@
     _convience_properties: ClassVar[list[str]] = [
         "api_path_summary",
         "api_path_raw_u_r_i",
         "api_path_is_templated",
         "api_path_available_operations",
         "api_path_available_response_codes",
         "api_path_is_ingress_exposed",
+        "terms",
     ]
 
     @property
     def api_path_summary(self) -> Optional[str]:
         return self.attributes.api_path_summary
 
     @api_path_summary.setter
@@ -9092,14 +9951,26 @@
 
     @api_path_is_ingress_exposed.setter
     def api_path_is_ingress_exposed(self, api_path_is_ingress_exposed: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.api_path_is_ingress_exposed = api_path_is_ingress_exposed
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("APIPath", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "APIPath":
             raise ValueError("must be APIPath")
         return v
@@ -9172,14 +10043,15 @@
         "external_location",
         "external_location_region",
         "external_location_format",
         "is_partitioned",
         "partition_strategy",
         "partition_count",
         "partition_list",
+        "terms",
     ]
 
     @property
     def constraint(self) -> Optional[str]:
         return self.attributes.constraint
 
     @constraint.setter
@@ -9324,14 +10196,26 @@
 
     @partition_list.setter
     def partition_list(self, partition_list: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.partition_list = partition_list
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("TablePartition", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "TablePartition":
             raise ValueError("must be TablePartition")
         return v
@@ -9433,14 +10317,15 @@
         "external_location",
         "external_location_region",
         "external_location_format",
         "is_partitioned",
         "partition_strategy",
         "partition_count",
         "partition_list",
+        "terms",
     ]
 
     @property
     def column_count(self) -> Optional[int]:
         return self.attributes.column_count
 
     @column_count.setter
@@ -9575,14 +10460,26 @@
 
     @partition_list.setter
     def partition_list(self, partition_list: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.partition_list = partition_list
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("Table", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Table":
             raise ValueError("must be Table")
         return v
@@ -9721,14 +10618,15 @@
         "variables_schema_base64",
         "is_private",
         "is_sql_snippet",
         "parent_qualified_name",
         "collection_qualified_name",
         "is_visual_query",
         "visual_builder_schema_base64",
+        "terms",
     ]
 
     @property
     def raw_query(self) -> Optional[str]:
         return self.attributes.raw_query
 
     @raw_query.setter
@@ -9829,14 +10727,26 @@
 
     @visual_builder_schema_base64.setter
     def visual_builder_schema_base64(self, visual_builder_schema_base64: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.visual_builder_schema_base64 = visual_builder_schema_base64
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("Query", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Query":
             raise ValueError("must be Query")
         return v
@@ -9966,14 +10876,15 @@
         "column_mins",
         "column_missing_values_count",
         "column_missing_values_count_long",
         "column_missing_values_percentage",
         "column_uniqueness_percentage",
         "column_variance",
         "column_top_values",
+        "terms",
     ]
 
     @property
     def data_type(self) -> Optional[str]:
         return self.attributes.data_type
 
     @data_type.setter
@@ -10444,14 +11355,26 @@
     def column_top_values(
         self, column_top_values: Optional[list[ColumnValueFrequencyMap]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.column_top_values = column_top_values
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("Column", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Column":
             raise ValueError("must be Column")
         return v
@@ -10686,14 +11609,15 @@
         if name in Schema._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "table_count",
         "views_count",
+        "terms",
     ]
 
     @property
     def table_count(self) -> Optional[int]:
         return self.attributes.table_count
 
     @table_count.setter
@@ -10708,14 +11632,26 @@
 
     @views_count.setter
     def views_count(self, views_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.views_count = views_count
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("Schema", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Schema":
             raise ValueError("must be Schema")
         return v
@@ -10830,14 +11766,15 @@
 
     _convience_properties: ClassVar[list[str]] = [
         "snowflake_stream_type",
         "snowflake_stream_source_type",
         "snowflake_stream_mode",
         "snowflake_stream_is_stale",
         "snowflake_stream_stale_after",
+        "terms",
     ]
 
     @property
     def snowflake_stream_type(self) -> Optional[str]:
         return self.attributes.snowflake_stream_type
 
     @snowflake_stream_type.setter
@@ -10884,14 +11821,26 @@
     def snowflake_stream_stale_after(
         self, snowflake_stream_stale_after: Optional[datetime]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.snowflake_stream_stale_after = snowflake_stream_stale_after
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("SnowflakeStream", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "SnowflakeStream":
             raise ValueError("must be SnowflakeStream")
         return v
@@ -10961,14 +11910,15 @@
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "definition",
         "snowflake_pipe_is_auto_ingest_enabled",
         "snowflake_pipe_notification_channel_name",
+        "terms",
     ]
 
     @property
     def definition(self) -> Optional[str]:
         return self.attributes.definition
 
     @definition.setter
@@ -11001,14 +11951,26 @@
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.snowflake_pipe_notification_channel_name = (
             snowflake_pipe_notification_channel_name
         )
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("SnowflakePipe", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "SnowflakePipe":
             raise ValueError("must be SnowflakePipe")
         return v
@@ -11068,26 +12030,39 @@
     def __setattr__(self, name, value):
         if name in Database._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "schema_count",
+        "terms",
     ]
 
     @property
     def schema_count(self) -> Optional[int]:
         return self.attributes.schema_count
 
     @schema_count.setter
     def schema_count(self, schema_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.schema_count = schema_count
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("Database", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Database":
             raise ValueError("must be Database")
         return v
@@ -11188,26 +12163,39 @@
     def __setattr__(self, name, value):
         if name in Procedure._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "definition",
+        "terms",
     ]
 
     @property
     def definition(self) -> str:
         return self.attributes.definition
 
     @definition.setter
     def definition(self, definition: str):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.definition = definition
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("Procedure", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Procedure":
             raise ValueError("must be Procedure")
         return v
@@ -11268,14 +12256,15 @@
         "row_count",
         "size_bytes",
         "is_query_preview",
         "query_preview_config",
         "alias",
         "is_temporary",
         "definition",
+        "terms",
     ]
 
     @property
     def column_count(self) -> Optional[int]:
         return self.attributes.column_count
 
     @column_count.setter
@@ -11350,14 +12339,26 @@
 
     @definition.setter
     def definition(self, definition: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.definition = definition
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("View", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "View":
             raise ValueError("must be View")
         return v
@@ -11475,14 +12476,15 @@
         "row_count",
         "size_bytes",
         "is_query_preview",
         "query_preview_config",
         "alias",
         "is_temporary",
         "definition",
+        "terms",
     ]
 
     @property
     def refresh_mode(self) -> Optional[str]:
         return self.attributes.refresh_mode
 
     @refresh_mode.setter
@@ -11597,14 +12599,26 @@
 
     @definition.setter
     def definition(self, definition: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.definition = definition
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("MaterialisedView", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "MaterialisedView":
             raise ValueError("must be MaterialisedView")
         return v
@@ -11694,14 +12708,15 @@
         "gcs_object_m_d5_hash",
         "gcs_object_data_last_modified_time",
         "gcs_object_content_type",
         "gcs_object_content_encoding",
         "gcs_object_content_disposition",
         "gcs_object_content_language",
         "gcs_object_retention_expiration_date",
+        "terms",
     ]
 
     @property
     def gcs_bucket_name(self) -> Optional[str]:
         return self.attributes.gcs_bucket_name
 
     @gcs_bucket_name.setter
@@ -11856,14 +12871,26 @@
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.gcs_object_retention_expiration_date = (
             gcs_object_retention_expiration_date
         )
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("GCSObject", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "GCSObject":
             raise ValueError("must be GCSObject")
         return v
@@ -11955,14 +12982,15 @@
         "gcs_object_count",
         "gcs_bucket_versioning_enabled",
         "gcs_bucket_retention_locked",
         "gcs_bucket_retention_period",
         "gcs_bucket_retention_effective_time",
         "gcs_bucket_lifecycle_rules",
         "gcs_bucket_retention_policy",
+        "terms",
     ]
 
     @property
     def gcs_object_count(self) -> Optional[int]:
         return self.attributes.gcs_object_count
 
     @gcs_object_count.setter
@@ -12033,14 +13061,26 @@
 
     @gcs_bucket_retention_policy.setter
     def gcs_bucket_retention_policy(self, gcs_bucket_retention_policy: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.gcs_bucket_retention_policy = gcs_bucket_retention_policy
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("GCSBucket", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "GCSBucket":
             raise ValueError("must be GCSBucket")
         return v
@@ -12111,14 +13151,15 @@
         "adls_account_subscription",
         "adls_account_performance",
         "adls_account_replication",
         "adls_account_kind",
         "adls_primary_disk_state",
         "adls_account_provision_state",
         "adls_account_access_tier",
+        "terms",
     ]
 
     @property
     def adls_e_tag(self) -> Optional[str]:
         return self.attributes.adls_e_tag
 
     @adls_e_tag.setter
@@ -12223,14 +13264,26 @@
     def adls_account_access_tier(
         self, adls_account_access_tier: Optional[ADLSAccessTier]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.adls_account_access_tier = adls_account_access_tier
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("ADLSAccount", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "ADLSAccount":
             raise ValueError("must be ADLSAccount")
         return v
@@ -12304,14 +13357,15 @@
     _convience_properties: ClassVar[list[str]] = [
         "adls_container_url",
         "adls_container_lease_state",
         "adls_container_lease_status",
         "adls_container_encryption_scope",
         "adls_container_version_level_immutability_support",
         "adls_object_count",
+        "terms",
     ]
 
     @property
     def adls_container_url(self) -> Optional[str]:
         return self.attributes.adls_container_url
 
     @adls_container_url.setter
@@ -12378,14 +13432,26 @@
 
     @adls_object_count.setter
     def adls_object_count(self, adls_object_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.adls_object_count = adls_object_count
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("ADLSContainer", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "ADLSContainer":
             raise ValueError("must be ADLSContainer")
         return v
@@ -12463,14 +13529,15 @@
         "adls_object_content_type",
         "adls_object_content_m_d5_hash",
         "adls_object_content_language",
         "adls_object_lease_status",
         "adls_object_lease_state",
         "adls_object_metadata",
         "adls_container_qualified_name",
+        "terms",
     ]
 
     @property
     def adls_object_url(self) -> Optional[str]:
         return self.attributes.adls_object_url
 
     @adls_object_url.setter
@@ -12657,14 +13724,26 @@
     def adls_container_qualified_name(
         self, adls_container_qualified_name: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.adls_container_qualified_name = adls_container_qualified_name
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("ADLSObject", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "ADLSObject":
             raise ValueError("must be ADLSObject")
         return v
@@ -12757,14 +13836,15 @@
         if name in S3Bucket._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "s3_object_count",
         "s3_bucket_versioning_enabled",
+        "terms",
     ]
 
     @property
     def s3_object_count(self) -> Optional[int]:
         return self.attributes.s3_object_count
 
     @s3_object_count.setter
@@ -12781,14 +13861,26 @@
     def s3_bucket_versioning_enabled(
         self, s3_bucket_versioning_enabled: Optional[bool]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.s3_bucket_versioning_enabled = s3_bucket_versioning_enabled
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("S3Bucket", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "S3Bucket":
             raise ValueError("must be S3Bucket")
         return v
@@ -12887,14 +13979,15 @@
         "s3_bucket_qualified_name",
         "s3_object_size",
         "s3_object_storage_class",
         "s3_object_key",
         "s3_object_content_type",
         "s3_object_content_disposition",
         "s3_object_version_id",
+        "terms",
     ]
 
     @property
     def s3_object_last_modified_time(self) -> Optional[datetime]:
         return self.attributes.s3_object_last_modified_time
 
     @s3_object_last_modified_time.setter
@@ -12983,14 +14076,26 @@
 
     @s3_object_version_id.setter
     def s3_object_version_id(self, s3_object_version_id: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.s3_object_version_id = s3_object_version_id
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("S3Object", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "S3Object":
             raise ValueError("must be S3Object")
         return v
@@ -13119,14 +14224,15 @@
         "kafka_topic_compression_type",
         "kafka_topic_replication_factor",
         "kafka_topic_segment_bytes",
         "kafka_topic_partitions_count",
         "kafka_topic_size_in_bytes",
         "kafka_topic_record_count",
         "kafka_topic_cleanup_policy",
+        "terms",
     ]
 
     @property
     def kafka_topic_is_internal(self) -> Optional[bool]:
         return self.attributes.kafka_topic_is_internal
 
     @kafka_topic_is_internal.setter
@@ -13207,14 +14313,26 @@
     def kafka_topic_cleanup_policy(
         self, kafka_topic_cleanup_policy: Optional[PowerbiEndorsement]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.kafka_topic_cleanup_policy = kafka_topic_cleanup_policy
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("KafkaTopic", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "KafkaTopic":
             raise ValueError("must be KafkaTopic")
         return v
@@ -13282,14 +14400,15 @@
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "kafka_consumer_group_topic_consumption_properties",
         "kafka_consumer_group_member_count",
         "kafka_topic_names",
         "kafka_topic_qualified_names",
+        "terms",
     ]
 
     @property
     def kafka_consumer_group_topic_consumption_properties(
         self,
     ) -> Optional[list[KafkaTopicConsumption]]:
         return self.attributes.kafka_consumer_group_topic_consumption_properties
@@ -13339,14 +14458,26 @@
     def kafka_topic_qualified_names(
         self, kafka_topic_qualified_names: Optional[set[str]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.kafka_topic_qualified_names = kafka_topic_qualified_names
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("KafkaConsumerGroup", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "KafkaConsumerGroup":
             raise ValueError("must be KafkaConsumerGroup")
         return v
@@ -13403,14 +14534,15 @@
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "metabase_dashboard_count",
         "metabase_query_type",
         "metabase_query",
+        "terms",
     ]
 
     @property
     def metabase_dashboard_count(self) -> Optional[int]:
         return self.attributes.metabase_dashboard_count
 
     @metabase_dashboard_count.setter
@@ -13435,14 +14567,26 @@
 
     @metabase_query.setter
     def metabase_query(self, metabase_query: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.metabase_query = metabase_query
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("MetabaseQuestion", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "MetabaseQuestion":
             raise ValueError("must be MetabaseQuestion")
         return v
@@ -13498,14 +14642,15 @@
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "metabase_slug",
         "metabase_color",
         "metabase_namespace",
         "metabase_is_personal_collection",
+        "terms",
     ]
 
     @property
     def metabase_slug(self) -> Optional[str]:
         return self.attributes.metabase_slug
 
     @metabase_slug.setter
@@ -13544,14 +14689,26 @@
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.metabase_is_personal_collection = (
             metabase_is_personal_collection
         )
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("MetabaseCollection", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "MetabaseCollection":
             raise ValueError("must be MetabaseCollection")
         return v
@@ -13605,26 +14762,39 @@
     def __setattr__(self, name, value):
         if name in MetabaseDashboard._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "metabase_question_count",
+        "terms",
     ]
 
     @property
     def metabase_question_count(self) -> Optional[int]:
         return self.attributes.metabase_question_count
 
     @metabase_question_count.setter
     def metabase_question_count(self, metabase_question_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.metabase_question_count = metabase_question_count
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("MetabaseDashboard", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "MetabaseDashboard":
             raise ValueError("must be MetabaseDashboard")
         return v
@@ -13672,14 +14842,15 @@
         if name in QuickSightFolder._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "quick_sight_folder_type",
         "quick_sight_folder_hierarchy",
+        "terms",
     ]
 
     @property
     def quick_sight_folder_type(self) -> Optional[QuickSightFolderType]:
         return self.attributes.quick_sight_folder_type
 
     @quick_sight_folder_type.setter
@@ -13698,14 +14869,26 @@
     def quick_sight_folder_hierarchy(
         self, quick_sight_folder_hierarchy: Optional[list[dict[str, str]]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.quick_sight_folder_hierarchy = quick_sight_folder_hierarchy
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("QuickSightFolder", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "QuickSightFolder":
             raise ValueError("must be QuickSightFolder")
         return v
@@ -13758,14 +14941,15 @@
     def __setattr__(self, name, value):
         if name in QuickSightDashboardVisual._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "quick_sight_dashboard_qualified_name",
+        "terms",
     ]
 
     @property
     def quick_sight_dashboard_qualified_name(self) -> Optional[str]:
         return self.attributes.quick_sight_dashboard_qualified_name
 
     @quick_sight_dashboard_qualified_name.setter
@@ -13774,14 +14958,26 @@
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.quick_sight_dashboard_qualified_name = (
             quick_sight_dashboard_qualified_name
         )
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("QuickSightDashboardVisual", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "QuickSightDashboardVisual":
             raise ValueError("must be QuickSightDashboardVisual")
         return v
@@ -13825,14 +15021,15 @@
     def __setattr__(self, name, value):
         if name in QuickSightAnalysisVisual._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "quick_sight_analysis_qualified_name",
+        "terms",
     ]
 
     @property
     def quick_sight_analysis_qualified_name(self) -> Optional[str]:
         return self.attributes.quick_sight_analysis_qualified_name
 
     @quick_sight_analysis_qualified_name.setter
@@ -13841,14 +15038,26 @@
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.quick_sight_analysis_qualified_name = (
             quick_sight_analysis_qualified_name
         )
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("QuickSightAnalysisVisual", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "QuickSightAnalysisVisual":
             raise ValueError("must be QuickSightAnalysisVisual")
         return v
@@ -13893,14 +15102,15 @@
         if name in QuickSightDatasetField._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "quick_sight_dataset_field_type",
         "quick_sight_dataset_qualified_name",
+        "terms",
     ]
 
     @property
     def quick_sight_dataset_field_type(self) -> Optional[QuickSightDatasetFieldType]:
         return self.attributes.quick_sight_dataset_field_type
 
     @quick_sight_dataset_field_type.setter
@@ -13921,14 +15131,26 @@
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.quick_sight_dataset_qualified_name = (
             quick_sight_dataset_qualified_name
         )
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("QuickSightDatasetField", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "QuickSightDatasetField":
             raise ValueError("must be QuickSightDatasetField")
         return v
@@ -13978,14 +15200,15 @@
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "quick_sight_analysis_status",
         "quick_sight_analysis_calculated_fields",
         "quick_sight_analysis_parameter_declarations",
         "quick_sight_analysis_filter_groups",
+        "terms",
     ]
 
     @property
     def quick_sight_analysis_status(self) -> Optional[QuickSightAnalysisStatus]:
         return self.attributes.quick_sight_analysis_status
 
     @quick_sight_analysis_status.setter
@@ -14034,14 +15257,26 @@
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.quick_sight_analysis_filter_groups = (
             quick_sight_analysis_filter_groups
         )
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("QuickSightAnalysis", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "QuickSightAnalysis":
             raise ValueError("must be QuickSightAnalysis")
         return v
@@ -14098,14 +15333,15 @@
         if name in QuickSightDashboard._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "quick_sight_dashboard_published_version_number",
         "quick_sight_dashboard_last_published_time",
+        "terms",
     ]
 
     @property
     def quick_sight_dashboard_published_version_number(self) -> Optional[int]:
         return self.attributes.quick_sight_dashboard_published_version_number
 
     @quick_sight_dashboard_published_version_number.setter
@@ -14128,14 +15364,26 @@
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.quick_sight_dashboard_last_published_time = (
             quick_sight_dashboard_last_published_time
         )
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("QuickSightDashboard", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "QuickSightDashboard":
             raise ValueError("must be QuickSightDashboard")
         return v
@@ -14188,14 +15436,15 @@
         if name in QuickSightDataset._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "quick_sight_dataset_import_mode",
         "quick_sight_dataset_column_count",
+        "terms",
     ]
 
     @property
     def quick_sight_dataset_import_mode(self) -> Optional[QuickSightDatasetImportMode]:
         return self.attributes.quick_sight_dataset_import_mode
 
     @quick_sight_dataset_import_mode.setter
@@ -14218,14 +15467,26 @@
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.quick_sight_dataset_column_count = (
             quick_sight_dataset_column_count
         )
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("QuickSightDataset", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "QuickSightDataset":
             raise ValueError("must be QuickSightDataset")
         return v
@@ -14273,15 +15534,29 @@
     """Description"""
 
     def __setattr__(self, name, value):
         if name in ThoughtspotLiveboard._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
-    _convience_properties: ClassVar[list[str]] = []
+    _convience_properties: ClassVar[list[str]] = [
+        "terms",
+    ]
+
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
 
     type_name: str = Field("ThoughtspotLiveboard", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "ThoughtspotLiveboard":
             raise ValueError("must be ThoughtspotLiveboard")
@@ -14324,14 +15599,15 @@
         if name in ThoughtspotDashlet._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "thoughtspot_liveboard_name",
         "thoughtspot_liveboard_qualified_name",
+        "terms",
     ]
 
     @property
     def thoughtspot_liveboard_name(self) -> Optional[str]:
         return self.attributes.thoughtspot_liveboard_name
 
     @thoughtspot_liveboard_name.setter
@@ -14350,14 +15626,26 @@
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.thoughtspot_liveboard_qualified_name = (
             thoughtspot_liveboard_qualified_name
         )
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("ThoughtspotDashlet", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "ThoughtspotDashlet":
             raise ValueError("must be ThoughtspotDashlet")
         return v
@@ -14402,15 +15690,29 @@
     """Description"""
 
     def __setattr__(self, name, value):
         if name in ThoughtspotAnswer._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
-    _convience_properties: ClassVar[list[str]] = []
+    _convience_properties: ClassVar[list[str]] = [
+        "terms",
+    ]
+
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
 
     type_name: str = Field("ThoughtspotAnswer", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "ThoughtspotAnswer":
             raise ValueError("must be ThoughtspotAnswer")
@@ -14452,14 +15754,15 @@
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "workspace_qualified_name",
         "dataset_qualified_name",
         "web_url",
         "page_count",
+        "terms",
     ]
 
     @property
     def workspace_qualified_name(self) -> Optional[str]:
         return self.attributes.workspace_qualified_name
 
     @workspace_qualified_name.setter
@@ -14494,14 +15797,26 @@
 
     @page_count.setter
     def page_count(self, page_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.page_count = page_count
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("PowerBIReport", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "PowerBIReport":
             raise ValueError("must be PowerBIReport")
         return v
@@ -14562,14 +15877,15 @@
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "workspace_qualified_name",
         "dataset_qualified_name",
         "power_b_i_measure_expression",
         "power_b_i_is_external_measure",
+        "terms",
     ]
 
     @property
     def workspace_qualified_name(self) -> Optional[str]:
         return self.attributes.workspace_qualified_name
 
     @workspace_qualified_name.setter
@@ -14606,14 +15922,26 @@
     def power_b_i_is_external_measure(
         self, power_b_i_is_external_measure: Optional[bool]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.power_b_i_is_external_measure = power_b_i_is_external_measure
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("PowerBIMeasure", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "PowerBIMeasure":
             raise ValueError("must be PowerBIMeasure")
         return v
@@ -14671,14 +15999,15 @@
     _convience_properties: ClassVar[list[str]] = [
         "workspace_qualified_name",
         "dataset_qualified_name",
         "power_b_i_column_data_category",
         "power_b_i_column_data_type",
         "power_b_i_sort_by_column",
         "power_b_i_column_summarize_by",
+        "terms",
     ]
 
     @property
     def workspace_qualified_name(self) -> Optional[str]:
         return self.attributes.workspace_qualified_name
 
     @workspace_qualified_name.setter
@@ -14737,14 +16066,26 @@
     def power_b_i_column_summarize_by(
         self, power_b_i_column_summarize_by: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.power_b_i_column_summarize_by = power_b_i_column_summarize_by
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("PowerBIColumn", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "PowerBIColumn":
             raise ValueError("must be PowerBIColumn")
         return v
@@ -14807,14 +16148,15 @@
 
     _convience_properties: ClassVar[list[str]] = [
         "workspace_qualified_name",
         "dataset_qualified_name",
         "power_b_i_table_source_expressions",
         "power_b_i_table_column_count",
         "power_b_i_table_measure_count",
+        "terms",
     ]
 
     @property
     def workspace_qualified_name(self) -> Optional[str]:
         return self.attributes.workspace_qualified_name
 
     @workspace_qualified_name.setter
@@ -14865,14 +16207,26 @@
     def power_b_i_table_measure_count(
         self, power_b_i_table_measure_count: Optional[int]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.power_b_i_table_measure_count = power_b_i_table_measure_count
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("PowerBITable", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "PowerBITable":
             raise ValueError("must be PowerBITable")
         return v
@@ -14935,14 +16289,15 @@
         if name in PowerBITile._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "workspace_qualified_name",
         "dashboard_qualified_name",
+        "terms",
     ]
 
     @property
     def workspace_qualified_name(self) -> Optional[str]:
         return self.attributes.workspace_qualified_name
 
     @workspace_qualified_name.setter
@@ -14957,14 +16312,26 @@
 
     @dashboard_qualified_name.setter
     def dashboard_qualified_name(self, dashboard_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dashboard_qualified_name = dashboard_qualified_name
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("PowerBITile", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "PowerBITile":
             raise ValueError("must be PowerBITile")
         return v
@@ -15017,26 +16384,39 @@
     def __setattr__(self, name, value):
         if name in PowerBIDatasource._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "connection_details",
+        "terms",
     ]
 
     @property
     def connection_details(self) -> Optional[dict[str, str]]:
         return self.attributes.connection_details
 
     @connection_details.setter
     def connection_details(self, connection_details: Optional[dict[str, str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.connection_details = connection_details
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("PowerBIDatasource", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "PowerBIDatasource":
             raise ValueError("must be PowerBIDatasource")
         return v
@@ -15084,14 +16464,15 @@
 
     _convience_properties: ClassVar[list[str]] = [
         "web_url",
         "report_count",
         "dashboard_count",
         "dataset_count",
         "dataflow_count",
+        "terms",
     ]
 
     @property
     def web_url(self) -> Optional[str]:
         return self.attributes.web_url
 
     @web_url.setter
@@ -15136,14 +16517,26 @@
 
     @dataflow_count.setter
     def dataflow_count(self, dataflow_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dataflow_count = dataflow_count
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("PowerBIWorkspace", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "PowerBIWorkspace":
             raise ValueError("must be PowerBIWorkspace")
         return v
@@ -15203,14 +16596,15 @@
         if name in PowerBIDataset._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "workspace_qualified_name",
         "web_url",
+        "terms",
     ]
 
     @property
     def workspace_qualified_name(self) -> Optional[str]:
         return self.attributes.workspace_qualified_name
 
     @workspace_qualified_name.setter
@@ -15225,14 +16619,26 @@
 
     @web_url.setter
     def web_url(self, web_url: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.web_url = web_url
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("PowerBIDataset", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "PowerBIDataset":
             raise ValueError("must be PowerBIDataset")
         return v
@@ -15294,14 +16700,15 @@
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "workspace_qualified_name",
         "web_url",
         "tile_count",
+        "terms",
     ]
 
     @property
     def workspace_qualified_name(self) -> Optional[str]:
         return self.attributes.workspace_qualified_name
 
     @workspace_qualified_name.setter
@@ -15326,14 +16733,26 @@
 
     @tile_count.setter
     def tile_count(self, tile_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.tile_count = tile_count
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("PowerBIDashboard", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "PowerBIDashboard":
             raise ValueError("must be PowerBIDashboard")
         return v
@@ -15383,14 +16802,15 @@
         if name in PowerBIDataflow._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "workspace_qualified_name",
         "web_url",
+        "terms",
     ]
 
     @property
     def workspace_qualified_name(self) -> Optional[str]:
         return self.attributes.workspace_qualified_name
 
     @workspace_qualified_name.setter
@@ -15405,14 +16825,26 @@
 
     @web_url.setter
     def web_url(self, web_url: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.web_url = web_url
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("PowerBIDataflow", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "PowerBIDataflow":
             raise ValueError("must be PowerBIDataflow")
         return v
@@ -15461,14 +16893,15 @@
         if name in PowerBIPage._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "workspace_qualified_name",
         "report_qualified_name",
+        "terms",
     ]
 
     @property
     def workspace_qualified_name(self) -> Optional[str]:
         return self.attributes.workspace_qualified_name
 
     @workspace_qualified_name.setter
@@ -15483,14 +16916,26 @@
 
     @report_qualified_name.setter
     def report_qualified_name(self, report_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.report_qualified_name = report_qualified_name
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("PowerBIPage", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "PowerBIPage":
             raise ValueError("must be PowerBIPage")
         return v
@@ -15538,14 +16983,15 @@
         if name in PresetChart._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "preset_chart_description_markdown",
         "preset_chart_form_data",
+        "terms",
     ]
 
     @property
     def preset_chart_description_markdown(self) -> Optional[str]:
         return self.attributes.preset_chart_description_markdown
 
     @preset_chart_description_markdown.setter
@@ -15564,14 +17010,26 @@
 
     @preset_chart_form_data.setter
     def preset_chart_form_data(self, preset_chart_form_data: Optional[dict[str, str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.preset_chart_form_data = preset_chart_form_data
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("PresetChart", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "PresetChart":
             raise ValueError("must be PresetChart")
         return v
@@ -15620,14 +17078,15 @@
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "preset_dataset_datasource_name",
         "preset_dataset_id",
         "preset_dataset_type",
+        "terms",
     ]
 
     @property
     def preset_dataset_datasource_name(self) -> Optional[str]:
         return self.attributes.preset_dataset_datasource_name
 
     @preset_dataset_datasource_name.setter
@@ -15654,14 +17113,26 @@
 
     @preset_dataset_type.setter
     def preset_dataset_type(self, preset_dataset_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.preset_dataset_type = preset_dataset_type
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("PresetDataset", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "PresetDataset":
             raise ValueError("must be PresetDataset")
         return v
@@ -15716,14 +17187,15 @@
     _convience_properties: ClassVar[list[str]] = [
         "preset_dashboard_changed_by_name",
         "preset_dashboard_changed_by_url",
         "preset_dashboard_is_managed_externally",
         "preset_dashboard_is_published",
         "preset_dashboard_thumbnail_url",
         "preset_dashboard_chart_count",
+        "terms",
     ]
 
     @property
     def preset_dashboard_changed_by_name(self) -> Optional[str]:
         return self.attributes.preset_dashboard_changed_by_name
 
     @preset_dashboard_changed_by_name.setter
@@ -15794,14 +17266,26 @@
 
     @preset_dashboard_chart_count.setter
     def preset_dashboard_chart_count(self, preset_dashboard_chart_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.preset_dashboard_chart_count = preset_dashboard_chart_count
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("PresetDashboard", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "PresetDashboard":
             raise ValueError("must be PresetDashboard")
         return v
@@ -15874,14 +17358,15 @@
         "preset_workspace_hostname",
         "preset_workspace_is_in_maintenance_mode",
         "preset_workspace_region",
         "preset_workspace_status",
         "preset_workspace_deployment_id",
         "preset_workspace_dashboard_count",
         "preset_workspace_dataset_count",
+        "terms",
     ]
 
     @property
     def preset_workspace_public_dashboards_allowed(self) -> Optional[bool]:
         return self.attributes.preset_workspace_public_dashboards_allowed
 
     @preset_workspace_public_dashboards_allowed.setter
@@ -15982,14 +17467,26 @@
     def preset_workspace_dataset_count(
         self, preset_workspace_dataset_count: Optional[int]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.preset_workspace_dataset_count = preset_workspace_dataset_count
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("PresetWorkspace", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "PresetWorkspace":
             raise ValueError("must be PresetWorkspace")
         return v
@@ -16063,14 +17560,15 @@
         "mode_collection_token",
         "mode_report_published_at",
         "mode_query_count",
         "mode_chart_count",
         "mode_query_preview",
         "mode_is_public",
         "mode_is_shared",
+        "terms",
     ]
 
     @property
     def mode_collection_token(self) -> Optional[str]:
         return self.attributes.mode_collection_token
 
     @mode_collection_token.setter
@@ -16135,14 +17633,26 @@
 
     @mode_is_shared.setter
     def mode_is_shared(self, mode_is_shared: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mode_is_shared = mode_is_shared
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("ModeReport", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "ModeReport":
             raise ValueError("must be ModeReport")
         return v
@@ -16208,14 +17718,15 @@
         if name in ModeQuery._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "mode_raw_query",
         "mode_report_import_count",
+        "terms",
     ]
 
     @property
     def mode_raw_query(self) -> Optional[str]:
         return self.attributes.mode_raw_query
 
     @mode_raw_query.setter
@@ -16230,14 +17741,26 @@
 
     @mode_report_import_count.setter
     def mode_report_import_count(self, mode_report_import_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mode_report_import_count = mode_report_import_count
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("ModeQuery", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "ModeQuery":
             raise ValueError("must be ModeQuery")
         return v
@@ -16287,26 +17810,39 @@
     def __setattr__(self, name, value):
         if name in ModeChart._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "mode_chart_type",
+        "terms",
     ]
 
     @property
     def mode_chart_type(self) -> Optional[str]:
         return self.attributes.mode_chart_type
 
     @mode_chart_type.setter
     def mode_chart_type(self, mode_chart_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mode_chart_type = mode_chart_type
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("ModeChart", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "ModeChart":
             raise ValueError("must be ModeChart")
         return v
@@ -16350,26 +17886,39 @@
     def __setattr__(self, name, value):
         if name in ModeWorkspace._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "mode_collection_count",
+        "terms",
     ]
 
     @property
     def mode_collection_count(self) -> Optional[int]:
         return self.attributes.mode_collection_count
 
     @mode_collection_count.setter
     def mode_collection_count(self, mode_collection_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mode_collection_count = mode_collection_count
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("ModeWorkspace", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "ModeWorkspace":
             raise ValueError("must be ModeWorkspace")
         return v
@@ -16414,14 +17963,15 @@
         if name in ModeCollection._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "mode_collection_type",
         "mode_collection_state",
+        "terms",
     ]
 
     @property
     def mode_collection_type(self) -> Optional[str]:
         return self.attributes.mode_collection_type
 
     @mode_collection_type.setter
@@ -16436,14 +17986,26 @@
 
     @mode_collection_state.setter
     def mode_collection_state(self, mode_collection_state: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mode_collection_state = mode_collection_state
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("ModeCollection", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "ModeCollection":
             raise ValueError("must be ModeCollection")
         return v
@@ -16494,14 +18056,15 @@
         if name in SigmaDatasetColumn._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "sigma_dataset_qualified_name",
         "sigma_dataset_name",
+        "terms",
     ]
 
     @property
     def sigma_dataset_qualified_name(self) -> Optional[str]:
         return self.attributes.sigma_dataset_qualified_name
 
     @sigma_dataset_qualified_name.setter
@@ -16516,14 +18079,26 @@
 
     @sigma_dataset_name.setter
     def sigma_dataset_name(self, sigma_dataset_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sigma_dataset_name = sigma_dataset_name
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("SigmaDatasetColumn", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "SigmaDatasetColumn":
             raise ValueError("must be SigmaDatasetColumn")
         return v
@@ -16570,26 +18145,39 @@
     def __setattr__(self, name, value):
         if name in SigmaDataset._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "sigma_dataset_column_count",
+        "terms",
     ]
 
     @property
     def sigma_dataset_column_count(self) -> Optional[int]:
         return self.attributes.sigma_dataset_column_count
 
     @sigma_dataset_column_count.setter
     def sigma_dataset_column_count(self, sigma_dataset_column_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sigma_dataset_column_count = sigma_dataset_column_count
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("SigmaDataset", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "SigmaDataset":
             raise ValueError("must be SigmaDataset")
         return v
@@ -16633,26 +18221,39 @@
     def __setattr__(self, name, value):
         if name in SigmaWorkbook._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "sigma_page_count",
+        "terms",
     ]
 
     @property
     def sigma_page_count(self) -> Optional[int]:
         return self.attributes.sigma_page_count
 
     @sigma_page_count.setter
     def sigma_page_count(self, sigma_page_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sigma_page_count = sigma_page_count
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("SigmaWorkbook", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "SigmaWorkbook":
             raise ValueError("must be SigmaWorkbook")
         return v
@@ -16697,14 +18298,15 @@
         if name in SigmaDataElementField._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "sigma_data_element_field_is_hidden",
         "sigma_data_element_field_formula",
+        "terms",
     ]
 
     @property
     def sigma_data_element_field_is_hidden(self) -> Optional[bool]:
         return self.attributes.sigma_data_element_field_is_hidden
 
     @sigma_data_element_field_is_hidden.setter
@@ -16727,14 +18329,26 @@
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sigma_data_element_field_formula = (
             sigma_data_element_field_formula
         )
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("SigmaDataElementField", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "SigmaDataElementField":
             raise ValueError("must be SigmaDataElementField")
         return v
@@ -16781,26 +18395,39 @@
     def __setattr__(self, name, value):
         if name in SigmaPage._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "sigma_data_element_count",
+        "terms",
     ]
 
     @property
     def sigma_data_element_count(self) -> Optional[int]:
         return self.attributes.sigma_data_element_count
 
     @sigma_data_element_count.setter
     def sigma_data_element_count(self, sigma_data_element_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sigma_data_element_count = sigma_data_element_count
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("SigmaPage", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "SigmaPage":
             raise ValueError("must be SigmaPage")
         return v
@@ -16849,14 +18476,15 @@
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "sigma_data_element_query",
         "sigma_data_element_type",
         "sigma_data_element_field_count",
+        "terms",
     ]
 
     @property
     def sigma_data_element_query(self) -> Optional[str]:
         return self.attributes.sigma_data_element_query
 
     @sigma_data_element_query.setter
@@ -16883,14 +18511,26 @@
     def sigma_data_element_field_count(
         self, sigma_data_element_field_count: Optional[int]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sigma_data_element_field_count = sigma_data_element_field_count
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("SigmaDataElement", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "SigmaDataElement":
             raise ValueError("must be SigmaDataElement")
         return v
@@ -16943,26 +18583,39 @@
     def __setattr__(self, name, value):
         if name in QlikSpace._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "qlik_space_type",
+        "terms",
     ]
 
     @property
     def qlik_space_type(self) -> Optional[str]:
         return self.attributes.qlik_space_type
 
     @qlik_space_type.setter
     def qlik_space_type(self, qlik_space_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.qlik_space_type = qlik_space_type
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("QlikSpace", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "QlikSpace":
             raise ValueError("must be QlikSpace")
         return v
@@ -17013,14 +18666,15 @@
 
     _convience_properties: ClassVar[list[str]] = [
         "qlik_has_section_access",
         "qlik_origin_app_id",
         "qlik_is_encrypted",
         "qlik_is_direct_query_mode",
         "qlik_app_static_byte_size",
+        "terms",
     ]
 
     @property
     def qlik_has_section_access(self) -> Optional[bool]:
         return self.attributes.qlik_has_section_access
 
     @qlik_has_section_access.setter
@@ -17065,14 +18719,26 @@
 
     @qlik_app_static_byte_size.setter
     def qlik_app_static_byte_size(self, qlik_app_static_byte_size: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.qlik_app_static_byte_size = qlik_app_static_byte_size
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("QlikApp", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "QlikApp":
             raise ValueError("must be QlikApp")
         return v
@@ -17134,14 +18800,15 @@
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "qlik_chart_subtitle",
         "qlik_chart_footnote",
         "qlik_chart_orientation",
         "qlik_chart_type",
+        "terms",
     ]
 
     @property
     def qlik_chart_subtitle(self) -> Optional[str]:
         return self.attributes.qlik_chart_subtitle
 
     @qlik_chart_subtitle.setter
@@ -17176,14 +18843,26 @@
 
     @qlik_chart_type.setter
     def qlik_chart_type(self, qlik_chart_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.qlik_chart_type = qlik_chart_type
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("QlikChart", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "QlikChart":
             raise ValueError("must be QlikChart")
         return v
@@ -17239,14 +18918,15 @@
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "qlik_dataset_technical_name",
         "qlik_dataset_type",
         "qlik_dataset_uri",
         "qlik_dataset_subtype",
+        "terms",
     ]
 
     @property
     def qlik_dataset_technical_name(self) -> Optional[str]:
         return self.attributes.qlik_dataset_technical_name
 
     @qlik_dataset_technical_name.setter
@@ -17281,14 +18961,26 @@
 
     @qlik_dataset_subtype.setter
     def qlik_dataset_subtype(self, qlik_dataset_subtype: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.qlik_dataset_subtype = qlik_dataset_subtype
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("QlikDataset", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "QlikDataset":
             raise ValueError("must be QlikDataset")
         return v
@@ -17341,26 +19033,39 @@
     def __setattr__(self, name, value):
         if name in QlikSheet._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "qlik_sheet_is_approved",
+        "terms",
     ]
 
     @property
     def qlik_sheet_is_approved(self) -> Optional[bool]:
         return self.attributes.qlik_sheet_is_approved
 
     @qlik_sheet_is_approved.setter
     def qlik_sheet_is_approved(self, qlik_sheet_is_approved: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.qlik_sheet_is_approved = qlik_sheet_is_approved
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("QlikSheet", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "QlikSheet":
             raise ValueError("must be QlikSheet")
         return v
@@ -17411,14 +19116,15 @@
 
     _convience_properties: ClassVar[list[str]] = [
         "site_qualified_name",
         "project_qualified_name",
         "top_level_project_name",
         "top_level_project_qualified_name",
         "project_hierarchy",
+        "terms",
     ]
 
     @property
     def site_qualified_name(self) -> Optional[str]:
         return self.attributes.site_qualified_name
 
     @site_qualified_name.setter
@@ -17467,14 +19173,26 @@
 
     @project_hierarchy.setter
     def project_hierarchy(self, project_hierarchy: Optional[list[dict[str, str]]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.project_hierarchy = project_hierarchy
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("TableauWorkbook", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "TableauWorkbook":
             raise ValueError("must be TableauWorkbook")
         return v
@@ -17554,14 +19272,15 @@
         "tableau_datasource_field_data_type",
         "upstream_tables",
         "tableau_datasource_field_formula",
         "tableau_datasource_field_bin_size",
         "upstream_columns",
         "upstream_fields",
         "datasource_field_type",
+        "terms",
     ]
 
     @property
     def site_qualified_name(self) -> Optional[str]:
         return self.attributes.site_qualified_name
 
     @site_qualified_name.setter
@@ -17738,14 +19457,26 @@
 
     @datasource_field_type.setter
     def datasource_field_type(self, datasource_field_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.datasource_field_type = datasource_field_type
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("TableauDatasourceField", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "TableauDatasourceField":
             raise ValueError("must be TableauDatasourceField")
         return v
@@ -17847,14 +19578,15 @@
         "datasource_qualified_name",
         "project_hierarchy",
         "data_category",
         "role",
         "tableau_data_type",
         "formula",
         "upstream_fields",
+        "terms",
     ]
 
     @property
     def site_qualified_name(self) -> Optional[str]:
         return self.attributes.site_qualified_name
 
     @site_qualified_name.setter
@@ -17963,14 +19695,26 @@
 
     @upstream_fields.setter
     def upstream_fields(self, upstream_fields: Optional[list[dict[str, str]]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.upstream_fields = upstream_fields
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("TableauCalculatedField", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "TableauCalculatedField":
             raise ValueError("must be TableauCalculatedField")
         return v
@@ -18044,14 +19788,15 @@
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "site_qualified_name",
         "top_level_project_qualified_name",
         "is_top_level_project",
         "project_hierarchy",
+        "terms",
     ]
 
     @property
     def site_qualified_name(self) -> Optional[str]:
         return self.attributes.site_qualified_name
 
     @site_qualified_name.setter
@@ -18090,14 +19835,26 @@
 
     @project_hierarchy.setter
     def project_hierarchy(self, project_hierarchy: Optional[list[dict[str, str]]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.project_hierarchy = project_hierarchy
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("TableauProject", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "TableauProject":
             raise ValueError("must be TableauProject")
         return v
@@ -18168,14 +19925,15 @@
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "site_qualified_name",
         "project_qualified_name",
         "top_level_project_qualified_name",
         "project_hierarchy",
+        "terms",
     ]
 
     @property
     def site_qualified_name(self) -> Optional[str]:
         return self.attributes.site_qualified_name
 
     @site_qualified_name.setter
@@ -18214,14 +19972,26 @@
 
     @project_hierarchy.setter
     def project_hierarchy(self, project_hierarchy: Optional[list[dict[str, str]]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.project_hierarchy = project_hierarchy
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("TableauMetric", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "TableauMetric":
             raise ValueError("must be TableauMetric")
         return v
@@ -18272,15 +20042,29 @@
     """Description"""
 
     def __setattr__(self, name, value):
         if name in TableauSite._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
-    _convience_properties: ClassVar[list[str]] = []
+    _convience_properties: ClassVar[list[str]] = [
+        "terms",
+    ]
+
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
 
     type_name: str = Field("TableauSite", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "TableauSite":
             raise ValueError("must be TableauSite")
@@ -18334,14 +20118,15 @@
         "has_extracts",
         "is_certified",
         "certifier",
         "certification_note",
         "certifier_display_name",
         "upstream_tables",
         "upstream_datasources",
+        "terms",
     ]
 
     @property
     def site_qualified_name(self) -> Optional[str]:
         return self.attributes.site_qualified_name
 
     @site_qualified_name.setter
@@ -18472,14 +20257,26 @@
     def upstream_datasources(
         self, upstream_datasources: Optional[list[dict[str, str]]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.upstream_datasources = upstream_datasources
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("TableauDatasource", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "TableauDatasource":
             raise ValueError("must be TableauDatasource")
         return v
@@ -18563,14 +20360,15 @@
 
     _convience_properties: ClassVar[list[str]] = [
         "site_qualified_name",
         "project_qualified_name",
         "workbook_qualified_name",
         "top_level_project_qualified_name",
         "project_hierarchy",
+        "terms",
     ]
 
     @property
     def site_qualified_name(self) -> Optional[str]:
         return self.attributes.site_qualified_name
 
     @site_qualified_name.setter
@@ -18619,14 +20417,26 @@
 
     @project_hierarchy.setter
     def project_hierarchy(self, project_hierarchy: Optional[list[dict[str, str]]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.project_hierarchy = project_hierarchy
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("TableauDashboard", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "TableauDashboard":
             raise ValueError("must be TableauDashboard")
         return v
@@ -18691,14 +20501,15 @@
         "site_qualified_name",
         "project_qualified_name",
         "top_level_project_qualified_name",
         "project_hierarchy",
         "input_fields",
         "output_fields",
         "output_steps",
+        "terms",
     ]
 
     @property
     def site_qualified_name(self) -> Optional[str]:
         return self.attributes.site_qualified_name
 
     @site_qualified_name.setter
@@ -18767,14 +20578,26 @@
 
     @output_steps.setter
     def output_steps(self, output_steps: Optional[list[dict[str, str]]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.output_steps = output_steps
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("TableauFlow", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "TableauFlow":
             raise ValueError("must be TableauFlow")
         return v
@@ -18840,14 +20663,15 @@
 
     _convience_properties: ClassVar[list[str]] = [
         "site_qualified_name",
         "project_qualified_name",
         "top_level_project_qualified_name",
         "project_hierarchy",
         "workbook_qualified_name",
+        "terms",
     ]
 
     @property
     def site_qualified_name(self) -> Optional[str]:
         return self.attributes.site_qualified_name
 
     @site_qualified_name.setter
@@ -18896,14 +20720,26 @@
 
     @workbook_qualified_name.setter
     def workbook_qualified_name(self, workbook_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.workbook_qualified_name = workbook_qualified_name
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("TableauWorksheet", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "TableauWorksheet":
             raise ValueError("must be TableauWorksheet")
         return v
@@ -18976,14 +20812,15 @@
         "source_view_count",
         "sourcelast_updater_id",
         "source_last_accessed_at",
         "source_last_viewed_at",
         "source_content_metadata_id",
         "source_query_id",
         "model_name",
+        "terms",
     ]
 
     @property
     def folder_name(self) -> Optional[str]:
         return self.attributes.folder_name
 
     @folder_name.setter
@@ -19068,14 +20905,26 @@
 
     @model_name.setter
     def model_name(self, model_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.model_name = model_name
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("LookerLook", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "LookerLook":
             raise ValueError("must be LookerLook")
         return v
@@ -19157,14 +21006,15 @@
         "folder_name",
         "source_user_id",
         "source_view_count",
         "source_metadata_id",
         "sourcelast_updater_id",
         "source_last_accessed_at",
         "source_last_viewed_at",
+        "terms",
     ]
 
     @property
     def folder_name(self) -> Optional[str]:
         return self.attributes.folder_name
 
     @folder_name.setter
@@ -19229,14 +21079,26 @@
 
     @source_last_viewed_at.setter
     def source_last_viewed_at(self, source_last_viewed_at: Optional[datetime]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_last_viewed_at = source_last_viewed_at
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("LookerDashboard", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "LookerDashboard":
             raise ValueError("must be LookerDashboard")
         return v
@@ -19305,14 +21167,15 @@
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "source_content_metadata_id",
         "source_creator_id",
         "source_child_count",
         "source_parent_i_d",
+        "terms",
     ]
 
     @property
     def source_content_metadata_id(self) -> Optional[int]:
         return self.attributes.source_content_metadata_id
 
     @source_content_metadata_id.setter
@@ -19347,14 +21210,26 @@
 
     @source_parent_i_d.setter
     def source_parent_i_d(self, source_parent_i_d: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_parent_i_d = source_parent_i_d
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("LookerFolder", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "LookerFolder":
             raise ValueError("must be LookerFolder")
         return v
@@ -19416,14 +21291,15 @@
         "lookml_link_id",
         "merge_result_id",
         "note_text",
         "query_i_d",
         "result_maker_i_d",
         "subtitle_text",
         "look_id",
+        "terms",
     ]
 
     @property
     def lookml_link_id(self) -> Optional[str]:
         return self.attributes.lookml_link_id
 
     @lookml_link_id.setter
@@ -19488,14 +21364,26 @@
 
     @look_id.setter
     def look_id(self, look_id: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.look_id = look_id
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("LookerTile", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "LookerTile":
             raise ValueError("must be LookerTile")
         return v
@@ -19555,26 +21443,39 @@
     def __setattr__(self, name, value):
         if name in LookerModel._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "project_name",
+        "terms",
     ]
 
     @property
     def project_name(self) -> Optional[str]:
         return self.attributes.project_name
 
     @project_name.setter
     def project_name(self, project_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.project_name = project_name
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("LookerModel", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "LookerModel":
             raise ValueError("must be LookerModel")
         return v
@@ -19632,14 +21533,15 @@
 
     _convience_properties: ClassVar[list[str]] = [
         "project_name",
         "model_name",
         "source_connection_name",
         "view_name",
         "sql_table_name",
+        "terms",
     ]
 
     @property
     def project_name(self) -> Optional[str]:
         return self.attributes.project_name
 
     @project_name.setter
@@ -19684,14 +21586,26 @@
 
     @sql_table_name.setter
     def sql_table_name(self, sql_table_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sql_table_name = sql_table_name
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("LookerExplore", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "LookerExplore":
             raise ValueError("must be LookerExplore")
         return v
@@ -19745,15 +21659,29 @@
     """Description"""
 
     def __setattr__(self, name, value):
         if name in LookerProject._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
-    _convience_properties: ClassVar[list[str]] = []
+    _convience_properties: ClassVar[list[str]] = [
+        "terms",
+    ]
+
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
 
     type_name: str = Field("LookerProject", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "LookerProject":
             raise ValueError("must be LookerProject")
@@ -19807,14 +21735,15 @@
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "source_definition",
         "source_definition_database",
         "source_definition_schema",
         "fields",
+        "terms",
     ]
 
     @property
     def source_definition(self) -> Optional[str]:
         return self.attributes.source_definition
 
     @source_definition.setter
@@ -19849,14 +21778,26 @@
 
     @fields.setter
     def fields(self, fields: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.fields = fields
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("LookerQuery", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "LookerQuery":
             raise ValueError("must be LookerQuery")
         return v
@@ -19919,14 +21860,15 @@
         "project_name",
         "looker_explore_qualified_name",
         "looker_view_qualified_name",
         "model_name",
         "source_definition",
         "looker_field_data_type",
         "looker_times_used",
+        "terms",
     ]
 
     @property
     def project_name(self) -> Optional[str]:
         return self.attributes.project_name
 
     @project_name.setter
@@ -19993,14 +21935,26 @@
 
     @looker_times_used.setter
     def looker_times_used(self, looker_times_used: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.looker_times_used = looker_times_used
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("LookerField", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "LookerField":
             raise ValueError("must be LookerField")
         return v
@@ -20067,26 +22021,39 @@
     def __setattr__(self, name, value):
         if name in LookerView._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "project_name",
+        "terms",
     ]
 
     @property
     def project_name(self) -> Optional[str]:
         return self.attributes.project_name
 
     @project_name.setter
     def project_name(self, project_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.project_name = project_name
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("LookerView", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "LookerView":
             raise ValueError("must be LookerView")
         return v
@@ -20121,27 +22088,363 @@
     attributes: "LookerView.Attributes" = Field(
         None,
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
+class RedashDashboard(Redash):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in RedashDashboard._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "redash_dashboard_widget_count",
+        "terms",
+    ]
+
+    @property
+    def redash_dashboard_widget_count(self) -> Optional[int]:
+        return self.attributes.redash_dashboard_widget_count
+
+    @redash_dashboard_widget_count.setter
+    def redash_dashboard_widget_count(
+        self, redash_dashboard_widget_count: Optional[int]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.redash_dashboard_widget_count = redash_dashboard_widget_count
+
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
+    type_name: str = Field("RedashDashboard", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "RedashDashboard":
+            raise ValueError("must be RedashDashboard")
+        return v
+
+    class Attributes(Redash.Attributes):
+        redash_dashboard_widget_count: Optional[int] = Field(
+            None, description="", alias="redashDashboardWidgetCount"
+        )
+        input_to_processes: Optional[list[Process]] = Field(
+            None, description="", alias="inputToProcesses"
+        )  # relationship
+        links: Optional[list[Link]] = Field(
+            None, description="", alias="links"
+        )  # relationship
+        metrics: Optional[list[Metric]] = Field(
+            None, description="", alias="metrics"
+        )  # relationship
+        readme: Optional[Readme] = Field(
+            None, description="", alias="readme"
+        )  # relationship
+        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="meanings"
+        )  # relationship
+        output_from_processes: Optional[list[Process]] = Field(
+            None, description="", alias="outputFromProcesses"
+        )  # relationship
+
+    attributes: "RedashDashboard.Attributes" = Field(
+        None,
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class RedashQuery(Redash):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in RedashQuery._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "redash_query_s_q_l",
+        "redash_query_parameters",
+        "redash_query_schedule",
+        "redash_query_last_execution_runtime",
+        "redash_query_last_executed_at",
+        "redash_query_schedule_humanized",
+        "terms",
+    ]
+
+    @property
+    def redash_query_s_q_l(self) -> Optional[str]:
+        return self.attributes.redash_query_s_q_l
+
+    @redash_query_s_q_l.setter
+    def redash_query_s_q_l(self, redash_query_s_q_l: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.redash_query_s_q_l = redash_query_s_q_l
+
+    @property
+    def redash_query_parameters(self) -> Optional[str]:
+        return self.attributes.redash_query_parameters
+
+    @redash_query_parameters.setter
+    def redash_query_parameters(self, redash_query_parameters: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.redash_query_parameters = redash_query_parameters
+
+    @property
+    def redash_query_schedule(self) -> Optional[dict[str, str]]:
+        return self.attributes.redash_query_schedule
+
+    @redash_query_schedule.setter
+    def redash_query_schedule(self, redash_query_schedule: Optional[dict[str, str]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.redash_query_schedule = redash_query_schedule
+
+    @property
+    def redash_query_last_execution_runtime(self) -> Optional[float]:
+        return self.attributes.redash_query_last_execution_runtime
+
+    @redash_query_last_execution_runtime.setter
+    def redash_query_last_execution_runtime(
+        self, redash_query_last_execution_runtime: Optional[float]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.redash_query_last_execution_runtime = (
+            redash_query_last_execution_runtime
+        )
+
+    @property
+    def redash_query_last_executed_at(self) -> Optional[datetime]:
+        return self.attributes.redash_query_last_executed_at
+
+    @redash_query_last_executed_at.setter
+    def redash_query_last_executed_at(
+        self, redash_query_last_executed_at: Optional[datetime]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.redash_query_last_executed_at = redash_query_last_executed_at
+
+    @property
+    def redash_query_schedule_humanized(self) -> Optional[str]:
+        return self.attributes.redash_query_schedule_humanized
+
+    @redash_query_schedule_humanized.setter
+    def redash_query_schedule_humanized(
+        self, redash_query_schedule_humanized: Optional[str]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.redash_query_schedule_humanized = (
+            redash_query_schedule_humanized
+        )
+
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
+    type_name: str = Field("RedashQuery", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "RedashQuery":
+            raise ValueError("must be RedashQuery")
+        return v
+
+    class Attributes(Redash.Attributes):
+        redash_query_s_q_l: Optional[str] = Field(
+            None, description="", alias="redashQuerySQL"
+        )
+        redash_query_parameters: Optional[str] = Field(
+            None, description="", alias="redashQueryParameters"
+        )
+        redash_query_schedule: Optional[dict[str, str]] = Field(
+            None, description="", alias="redashQuerySchedule"
+        )
+        redash_query_last_execution_runtime: Optional[float] = Field(
+            None, description="", alias="redashQueryLastExecutionRuntime"
+        )
+        redash_query_last_executed_at: Optional[datetime] = Field(
+            None, description="", alias="redashQueryLastExecutedAt"
+        )
+        redash_query_schedule_humanized: Optional[str] = Field(
+            None, description="", alias="redashQueryScheduleHumanized"
+        )
+        input_to_processes: Optional[list[Process]] = Field(
+            None, description="", alias="inputToProcesses"
+        )  # relationship
+        redash_visualizations: Optional[list[RedashVisualization]] = Field(
+            None, description="", alias="redashVisualizations"
+        )  # relationship
+        links: Optional[list[Link]] = Field(
+            None, description="", alias="links"
+        )  # relationship
+        metrics: Optional[list[Metric]] = Field(
+            None, description="", alias="metrics"
+        )  # relationship
+        readme: Optional[Readme] = Field(
+            None, description="", alias="readme"
+        )  # relationship
+        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="meanings"
+        )  # relationship
+        output_from_processes: Optional[list[Process]] = Field(
+            None, description="", alias="outputFromProcesses"
+        )  # relationship
+
+    attributes: "RedashQuery.Attributes" = Field(
+        None,
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class RedashVisualization(Redash):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in RedashVisualization._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "redash_visualization_type",
+        "redash_query_name",
+        "redash_query_qualified_name",
+        "terms",
+    ]
+
+    @property
+    def redash_visualization_type(self) -> Optional[str]:
+        return self.attributes.redash_visualization_type
+
+    @redash_visualization_type.setter
+    def redash_visualization_type(self, redash_visualization_type: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.redash_visualization_type = redash_visualization_type
+
+    @property
+    def redash_query_name(self) -> Optional[str]:
+        return self.attributes.redash_query_name
+
+    @redash_query_name.setter
+    def redash_query_name(self, redash_query_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.redash_query_name = redash_query_name
+
+    @property
+    def redash_query_qualified_name(self) -> Optional[str]:
+        return self.attributes.redash_query_qualified_name
+
+    @redash_query_qualified_name.setter
+    def redash_query_qualified_name(self, redash_query_qualified_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.redash_query_qualified_name = redash_query_qualified_name
+
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
+    type_name: str = Field("RedashVisualization", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "RedashVisualization":
+            raise ValueError("must be RedashVisualization")
+        return v
+
+    class Attributes(Redash.Attributes):
+        redash_visualization_type: Optional[str] = Field(
+            None, description="", alias="redashVisualizationType"
+        )
+        redash_query_name: Optional[str] = Field(
+            None, description="", alias="redashQueryName"
+        )
+        redash_query_qualified_name: Optional[str] = Field(
+            None, description="", alias="redashQueryQualifiedName"
+        )
+        input_to_processes: Optional[list[Process]] = Field(
+            None, description="", alias="inputToProcesses"
+        )  # relationship
+        links: Optional[list[Link]] = Field(
+            None, description="", alias="links"
+        )  # relationship
+        metrics: Optional[list[Metric]] = Field(
+            None, description="", alias="metrics"
+        )  # relationship
+        readme: Optional[Readme] = Field(
+            None, description="", alias="readme"
+        )  # relationship
+        redash_query: Optional[RedashQuery] = Field(
+            None, description="", alias="redashQuery"
+        )  # relationship
+        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="meanings"
+        )  # relationship
+        output_from_processes: Optional[list[Process]] = Field(
+            None, description="", alias="outputFromProcesses"
+        )  # relationship
+
+    attributes: "RedashVisualization.Attributes" = Field(
+        None,
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
 class SalesforceObject(Salesforce):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in SalesforceObject._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "is_custom",
         "is_mergable",
         "is_queryable",
         "field_count",
+        "terms",
     ]
 
     @property
     def is_custom(self) -> Optional[bool]:
         return self.attributes.is_custom
 
     @is_custom.setter
@@ -20176,14 +22479,26 @@
 
     @field_count.setter
     def field_count(self, field_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.field_count = field_count
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("SalesforceObject", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "SalesforceObject":
             raise ValueError("must be SalesforceObject")
         return v
@@ -20249,14 +22564,15 @@
         "is_nullable",
         "precision",
         "numeric_scale",
         "is_unique",
         "picklist_values",
         "is_polymorphic_foreign_key",
         "default_value_formula",
+        "terms",
     ]
 
     @property
     def data_type(self) -> Optional[str]:
         return self.attributes.data_type
 
     @data_type.setter
@@ -20411,14 +22727,26 @@
 
     @default_value_formula.setter
     def default_value_formula(self, default_value_formula: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.default_value_formula = default_value_formula
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("SalesforceField", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "SalesforceField":
             raise ValueError("must be SalesforceField")
         return v
@@ -20494,26 +22822,39 @@
     def __setattr__(self, name, value):
         if name in SalesforceOrganization._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "source_id",
+        "terms",
     ]
 
     @property
     def source_id(self) -> Optional[str]:
         return self.attributes.source_id
 
     @source_id.setter
     def source_id(self, source_id: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_id = source_id
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("SalesforceOrganization", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "SalesforceOrganization":
             raise ValueError("must be SalesforceOrganization")
         return v
@@ -20563,14 +22904,15 @@
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "source_id",
         "dashboard_type",
         "report_count",
+        "terms",
     ]
 
     @property
     def source_id(self) -> Optional[str]:
         return self.attributes.source_id
 
     @source_id.setter
@@ -20595,14 +22937,26 @@
 
     @report_count.setter
     def report_count(self, report_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.report_count = report_count
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("SalesforceDashboard", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "SalesforceDashboard":
             raise ValueError("must be SalesforceDashboard")
         return v
@@ -20653,14 +23007,15 @@
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "source_id",
         "report_type",
         "detail_columns",
+        "terms",
     ]
 
     @property
     def source_id(self) -> Optional[str]:
         return self.attributes.source_id
 
     @source_id.setter
@@ -20685,14 +23040,26 @@
 
     @detail_columns.setter
     def detail_columns(self, detail_columns: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.detail_columns = detail_columns
 
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
     type_name: str = Field("SalesforceReport", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "SalesforceReport":
             raise ValueError("must be SalesforceReport")
         return v
@@ -20741,15 +23108,29 @@
     """Description"""
 
     def __setattr__(self, name, value):
         if name in QlikStream._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
-    _convience_properties: ClassVar[list[str]] = []
+    _convience_properties: ClassVar[list[str]] = [
+        "terms",
+    ]
+
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
 
     type_name: str = Field("QlikStream", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "QlikStream":
             raise ValueError("must be QlikStream")
@@ -20885,14 +23266,16 @@
 
 Qlik.Attributes.update_forward_refs()
 
 Tableau.Attributes.update_forward_refs()
 
 Looker.Attributes.update_forward_refs()
 
+Redash.Attributes.update_forward_refs()
+
 Salesforce.Attributes.update_forward_refs()
 
 DbtModelColumn.Attributes.update_forward_refs()
 
 DbtModel.Attributes.update_forward_refs()
 
 DbtMetric.Attributes.update_forward_refs()
@@ -21075,14 +23458,20 @@
 
 LookerQuery.Attributes.update_forward_refs()
 
 LookerField.Attributes.update_forward_refs()
 
 LookerView.Attributes.update_forward_refs()
 
+RedashDashboard.Attributes.update_forward_refs()
+
+RedashQuery.Attributes.update_forward_refs()
+
+RedashVisualization.Attributes.update_forward_refs()
+
 SalesforceObject.Attributes.update_forward_refs()
 
 SalesforceField.Attributes.update_forward_refs()
 
 SalesforceOrganization.Attributes.update_forward_refs()
 
 SalesforceDashboard.Attributes.update_forward_refs()
```

### Comparing `pyatlan-0.0.25/pyatlan/model/core.py` & `pyatlan-0.0.26/pyatlan/model/core.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.25/pyatlan/model/enums.py` & `pyatlan-0.0.26/pyatlan/model/enums.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.25/pyatlan/model/response.py` & `pyatlan-0.0.26/pyatlan/model/response.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.25/pyatlan/model/role.py` & `pyatlan-0.0.26/pyatlan/model/role.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.25/pyatlan/model/search.py` & `pyatlan-0.0.26/pyatlan/model/search.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.25/pyatlan/model/structs.py` & `pyatlan-0.0.26/pyatlan/model/structs.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.25/pyatlan/model/typedef.py` & `pyatlan-0.0.26/pyatlan/model/typedef.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.25/pyatlan/utils.py` & `pyatlan-0.0.26/pyatlan/utils.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.25/pyatlan.egg-info/PKG-INFO` & `pyatlan-0.0.26/pyatlan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatlan
-Version: 0.0.25
+Version: 0.0.26
 Summary: Atlan Python Client
 Home-page: https://github.com/atlanhq/atlan-python
 Author: Atlan Technologies Pvt Ltd
 Author-email: engineering@atlan.com
 License: Apache LICENSE 2.0
 Keywords: atlan client
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyatlan-0.0.25/pyatlan.egg-info/SOURCES.txt` & `pyatlan-0.0.26/pyatlan.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -40,12 +40,13 @@
 tests/integration/custom_metadata_test.py
 tests/integration/role_test.py
 tests/integration/test_client.py
 tests/integration/test_entity_model.py
 tests/integration/test_index_search.py
 tests/unit/__init__.py
 tests/unit/test_classification_name.py
+tests/unit/test_client.py
 tests/unit/test_glossary_term.py
 tests/unit/test_model.py
 tests/unit/test_search_model.py
 tests/unit/test_typedef_model.py
 tests/unit/test_utils.py
```

### Comparing `pyatlan-0.0.25/setup.py` & `pyatlan-0.0.26/setup.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.25/tests/integration/classification_test.py` & `pyatlan-0.0.26/tests/integration/classification_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.25/tests/integration/custom_metadata_test.py` & `pyatlan-0.0.26/tests/integration/custom_metadata_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.25/tests/integration/role_test.py` & `pyatlan-0.0.26/tests/integration/role_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.25/tests/integration/test_entity_model.py` & `pyatlan-0.0.26/tests/integration/test_entity_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.25/tests/integration/test_index_search.py` & `pyatlan-0.0.26/tests/integration/test_index_search.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.25/tests/unit/test_classification_name.py` & `pyatlan-0.0.26/tests/unit/test_classification_name.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.25/tests/unit/test_glossary_term.py` & `pyatlan-0.0.26/tests/unit/test_glossary_term.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.25/tests/unit/test_model.py` & `pyatlan-0.0.26/tests/unit/test_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,14 +128,15 @@
     "Optional[list[ColumnValueFrequencyMap]]": [ColumnValueFrequencyMap()],
     "Optional[KafkaTopicCompressionType]": KafkaTopicCompressionType.GZIP,
     "Optional[QuickSightFolderType]": QuickSightFolderType.SHARED,
     "Optional[QuickSightDatasetFieldType]": QuickSightDatasetFieldType.STRING,
     "Optional[QuickSightAnalysisStatus]": QuickSightAnalysisStatus.CREATION_FAILED,
     "Optional[QuickSightDatasetImportMode]": QuickSightDatasetImportMode.SPICE,
     "Optional[list[KafkaTopicConsumption]]": [KafkaTopicConsumption()],
+    "list[AtlasGlossaryTerm]": [AtlasGlossaryTerm()],
 }
 
 
 def load_json(filename):
     with (DATA_DIR / filename).open() as input_file:
         return json.load(input_file)
 
@@ -1317,15 +1318,15 @@
     exec(
         f"ret_value = sut.{property_name}",
         {"sut": sut, "property_name": property_name},
         local_ns,
     )
     assert attribute_value == local_ns["ret_value"]
     exec(
-        f"ret_value = sut.attributes.{property_name}",
+        f"ret_value = sut.attributes.{property_name if property_name != 'terms' else 'meanings'}",
         {"sut": sut, "property_name": property_name},
         local_ns,
     )
     assert attribute_value == local_ns["ret_value"]
 
 
 @pytest.mark.parametrize(
```

### Comparing `pyatlan-0.0.25/tests/unit/test_search_model.py` & `pyatlan-0.0.26/tests/unit/test_search_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.25/tests/unit/test_typedef_model.py` & `pyatlan-0.0.26/tests/unit/test_typedef_model.py`

 * *Files identical despite different names*

