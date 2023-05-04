# Comparing `tmp/text2term-2.2.0.tar.gz` & `tmp/text2term-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text2term-2.2.0.tar", last modified: Tue May  2 13:43:38 2023, max compression
+gzip compressed data, was "text2term-2.3.0.tar", last modified: Thu May  4 15:09:44 2023, max compression
```

## Comparing `text2term-2.2.0.tar` & `text2term-2.3.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-05-02 13:43:38.272933 text2term-2.2.0/
--rw-r--r--   0 jason      (501) staff       (20)     1117 2022-08-03 13:24:07.000000 text2term-2.2.0/LICENSE
--rw-r--r--   0 jason      (501) staff       (20)    14370 2023-05-02 13:43:38.272744 text2term-2.2.0/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)    13612 2023-04-25 19:02:20.000000 text2term-2.2.0/README.md
--rw-r--r--   0 jason      (501) staff       (20)       38 2023-05-02 13:43:38.272975 text2term-2.2.0/setup.cfg
--rw-r--r--   0 jason      (501) staff       (20)     1162 2023-03-27 17:45:54.000000 text2term-2.2.0/setup.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-05-02 13:43:38.269621 text2term-2.2.0/test/
--rw-r--r--   0 jason      (501) staff       (20)     1435 2023-04-25 18:43:12.000000 text2term-2.2.0/test/test-pypi.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-05-02 13:43:38.271887 text2term-2.2.0/text2term/
--rw-r--r--   0 jason      (501) staff       (20)      406 2023-05-02 13:41:43.000000 text2term-2.2.0/text2term/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)     4540 2023-04-25 19:04:10.000000 text2term-2.2.0/text2term/__main__.py
--rw-r--r--   0 jason      (501) staff       (20)     4416 2022-08-03 13:24:07.000000 text2term-2.2.0/text2term/bioportal_mapper.py
--rw-r--r--   0 jason      (501) staff       (20)       17 2023-04-17 18:05:11.000000 text2term-2.2.0/text2term/config.py
--rw-r--r--   0 jason      (501) staff       (20)      469 2022-09-26 14:42:08.000000 text2term-2.2.0/text2term/mapper.py
--rw-r--r--   0 jason      (501) staff       (20)     6692 2023-03-27 17:45:54.000000 text2term-2.2.0/text2term/onto_utils.py
--rw-r--r--   0 jason      (501) staff       (20)     5540 2023-03-27 17:45:54.000000 text2term-2.2.0/text2term/preprocess.py
--rw-r--r--   0 jason      (501) staff       (20)     5403 2023-02-09 15:42:55.000000 text2term-2.2.0/text2term/syntactic_mapper.py
--rw-r--r--   0 jason      (501) staff       (20)    13355 2023-05-02 13:41:43.000000 text2term-2.2.0/text2term/t2t.py
--rw-r--r--   0 jason      (501) staff       (20)      741 2023-02-24 16:05:08.000000 text2term-2.2.0/text2term/tagged_terms.py
--rw-r--r--   0 jason      (501) staff       (20)     2479 2023-04-18 15:25:34.000000 text2term-2.2.0/text2term/term.py
--rw-r--r--   0 jason      (501) staff       (20)    16757 2023-05-02 13:41:43.000000 text2term-2.2.0/text2term/term_collector.py
--rw-r--r--   0 jason      (501) staff       (20)     2697 2022-08-03 13:24:07.000000 text2term-2.2.0/text2term/term_graph.py
--rw-r--r--   0 jason      (501) staff       (20)     2991 2023-01-20 15:17:36.000000 text2term-2.2.0/text2term/term_graph_generator.py
--rw-r--r--   0 jason      (501) staff       (20)     2158 2023-04-11 13:56:32.000000 text2term-2.2.0/text2term/term_mapping.py
--rw-r--r--   0 jason      (501) staff       (20)     5108 2022-11-15 20:43:11.000000 text2term-2.2.0/text2term/tfidf_mapper.py
--rw-r--r--   0 jason      (501) staff       (20)     4098 2023-02-09 15:42:55.000000 text2term-2.2.0/text2term/zooma_mapper.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-05-02 13:43:38.272562 text2term-2.2.0/text2term.egg-info/
--rw-r--r--   0 jason      (501) staff       (20)    14370 2023-05-02 13:43:38.000000 text2term-2.2.0/text2term.egg-info/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)      625 2023-05-02 13:43:38.000000 text2term-2.2.0/text2term.egg-info/SOURCES.txt
--rw-r--r--   0 jason      (501) staff       (20)        1 2023-05-02 13:43:38.000000 text2term-2.2.0/text2term.egg-info/dependency_links.txt
--rw-r--r--   0 jason      (501) staff       (20)      248 2023-05-02 13:43:38.000000 text2term-2.2.0/text2term.egg-info/requires.txt
--rw-r--r--   0 jason      (501) staff       (20)       10 2023-05-02 13:43:38.000000 text2term-2.2.0/text2term.egg-info/top_level.txt
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-05-04 15:09:44.164136 text2term-2.3.0/
+-rw-r--r--   0 jason      (501) staff       (20)     1117 2022-08-03 13:24:07.000000 text2term-2.3.0/LICENSE
+-rw-r--r--   0 jason      (501) staff       (20)    14914 2023-05-04 15:09:44.163948 text2term-2.3.0/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)    14156 2023-05-04 15:09:10.000000 text2term-2.3.0/README.md
+-rw-r--r--   0 jason      (501) staff       (20)       38 2023-05-04 15:09:44.164179 text2term-2.3.0/setup.cfg
+-rw-r--r--   0 jason      (501) staff       (20)     1162 2023-03-27 17:45:54.000000 text2term-2.3.0/setup.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-05-04 15:09:44.160366 text2term-2.3.0/test/
+-rw-r--r--   0 jason      (501) staff       (20)     1435 2023-04-25 18:43:12.000000 text2term-2.3.0/test/test-pypi.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-05-04 15:09:44.163001 text2term-2.3.0/text2term/
+-rw-r--r--   0 jason      (501) staff       (20)      427 2023-05-04 15:09:10.000000 text2term-2.3.0/text2term/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)     4540 2023-04-25 19:04:10.000000 text2term-2.3.0/text2term/__main__.py
+-rw-r--r--   0 jason      (501) staff       (20)     4416 2022-08-03 13:24:07.000000 text2term-2.3.0/text2term/bioportal_mapper.py
+-rw-r--r--   0 jason      (501) staff       (20)       17 2023-05-04 15:09:10.000000 text2term-2.3.0/text2term/config.py
+-rw-r--r--   0 jason      (501) staff       (20)      469 2022-09-26 14:42:08.000000 text2term-2.3.0/text2term/mapper.py
+-rw-r--r--   0 jason      (501) staff       (20)     3649 2023-05-04 15:09:10.000000 text2term-2.3.0/text2term/onto_cache.py
+-rw-r--r--   0 jason      (501) staff       (20)     6692 2023-03-27 17:45:54.000000 text2term-2.3.0/text2term/onto_utils.py
+-rw-r--r--   0 jason      (501) staff       (20)     5540 2023-03-27 17:45:54.000000 text2term-2.3.0/text2term/preprocess.py
+-rw-r--r--   0 jason      (501) staff       (20)     5403 2023-02-09 15:42:55.000000 text2term-2.3.0/text2term/syntactic_mapper.py
+-rw-r--r--   0 jason      (501) staff       (20)    12516 2023-05-04 15:09:10.000000 text2term-2.3.0/text2term/t2t.py
+-rw-r--r--   0 jason      (501) staff       (20)      741 2023-02-24 16:05:08.000000 text2term-2.3.0/text2term/tagged_terms.py
+-rw-r--r--   0 jason      (501) staff       (20)     2479 2023-04-18 15:25:34.000000 text2term-2.3.0/text2term/term.py
+-rw-r--r--   0 jason      (501) staff       (20)    17050 2023-05-04 15:09:10.000000 text2term-2.3.0/text2term/term_collector.py
+-rw-r--r--   0 jason      (501) staff       (20)     2697 2022-08-03 13:24:07.000000 text2term-2.3.0/text2term/term_graph.py
+-rw-r--r--   0 jason      (501) staff       (20)     2991 2023-01-20 15:17:36.000000 text2term-2.3.0/text2term/term_graph_generator.py
+-rw-r--r--   0 jason      (501) staff       (20)     2158 2023-04-11 13:56:32.000000 text2term-2.3.0/text2term/term_mapping.py
+-rw-r--r--   0 jason      (501) staff       (20)     5108 2022-11-15 20:43:11.000000 text2term-2.3.0/text2term/tfidf_mapper.py
+-rw-r--r--   0 jason      (501) staff       (20)     4098 2023-02-09 15:42:55.000000 text2term-2.3.0/text2term/zooma_mapper.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-05-04 15:09:44.163758 text2term-2.3.0/text2term.egg-info/
+-rw-r--r--   0 jason      (501) staff       (20)    14914 2023-05-04 15:09:44.000000 text2term-2.3.0/text2term.egg-info/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)      649 2023-05-04 15:09:44.000000 text2term-2.3.0/text2term.egg-info/SOURCES.txt
+-rw-r--r--   0 jason      (501) staff       (20)        1 2023-05-04 15:09:44.000000 text2term-2.3.0/text2term.egg-info/dependency_links.txt
+-rw-r--r--   0 jason      (501) staff       (20)      248 2023-05-04 15:09:44.000000 text2term-2.3.0/text2term.egg-info/requires.txt
+-rw-r--r--   0 jason      (501) staff       (20)       10 2023-05-04 15:09:44.000000 text2term-2.3.0/text2term.egg-info/top_level.txt
```

### Comparing `text2term-2.2.0/LICENSE` & `text2term-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `text2term-2.2.0/PKG-INFO` & `text2term-2.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2term
-Version: 2.2.0
+Version: 2.3.0
 Summary: A tool for mapping free-text descriptions of (biomedical) entities to controlled terms in ontologies
 Home-page: https://github.com/ccb-hms/ontology-mapper
 Author: Center for Computational Biomedicine, Harvard Medical School
 Author-email: rafael_goncalves@hms.harvard.edu
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -124,14 +124,15 @@
 For `map_tagged_terms`, everything is the same as `map_terms` except the first argument is either a dictionary of terms to a list of tags, or a list of TaggedTerm objects (see below). Currently, the tags do not affect the mapping in any way, but they are added to the output dataframe at the end of the process.
 
 All other arguments are the same, and have the same functionality:
 
 `target_ontology` : str
     Path or URL of 'target' ontology to map the source terms to. When the chosen mapper is BioPortal or Zooma,
     provide a comma-separated list of ontology acronyms (eg 'EFO,HPO') or write 'all' to search all ontologies
+    As of version 2.3.0, passing a recognized acronym to `target_ontology` will generate the download link automatically. This is done using the `bioregistry` python package.
 
 `base_iris` : tuple
     Map only to ontology terms whose IRIs start with one of the strings given in this tuple, for example:
     ('http://www.ebi.ac.uk/efo','http://purl.obolibrary.org/obo/HP')
 
 `source_terms_ids` : tuple
     Collection of identifiers for the given source terms
@@ -172,26 +173,27 @@
 
 `df` : Data frame containing the generated ontology mappings
 
 ### Ontology Caching
 As of version 1.1.0, users can cache ontologies that they want to use regularly or quickly. Programmatically, there are two steps to using the cache: creating the cache, then accessing it. First, the user can cache ontologies using either of two functions:
 
 ```python
-cache_ontology(ontology_url, ontology_acronym, base_iris=())
+cache_ontology(ontology_url, ontology_acronym="", base_iris=())
 ```
 
 ```python
 cache_ontology_set(ontology_registry_path)
 ```
 
-The first of these will cache a single ontology from a URL or file path, with it being referenced by an acronym that will be used to reference it later. An example can be found above.
+The first of these will cache a single ontology from a URL or file path, with it being referenced by an acronym that will be used to reference it later. If no acronym is given, it will use the URL as the cache name. An example can be found above.
 The second function allows the user to cache several ontologies at once by referencing a CSV file of the format:
 `acronym,version,url`. An example is provided in `resources/ontologies.csv`
 
 Once an ontology has been cached by either function, it is stored in a cache folder locally, and thus can be referenced even in different Python instances.
+As of version 2.3.0, the `cache_ontology` function also returns an object that can be used to call any of the `map` functions, as well as `clear_cache` and `cache_exists`. These have the same arguments, except `ontology_target` is not specified and there is no `use_cache` option, as it is always True.
 
 NOTE: Due to how ontologies are processed in memory, `cache_ontology_set` must be used to cache multiple ontologies in a single Python instance. If `cache_ontology` is used multiple times in one instance, the behavior is undefined and may cause visible or invisible errors.
 
 After an ontology is cached, the user can access the cache by using the assigned acronym in the place of `target_ontology` and setting the `use_cache` flag to `True`.
 To clear the cache, one can call:
 `clear_cache(ontology_acronym='')`
 If no arguments are specified, the entire cache will be cleared. Otherwise, only the ontology with the given acronym will be cleared.
```

### Comparing `text2term-2.2.0/README.md` & `text2term-2.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -105,14 +105,15 @@
 For `map_tagged_terms`, everything is the same as `map_terms` except the first argument is either a dictionary of terms to a list of tags, or a list of TaggedTerm objects (see below). Currently, the tags do not affect the mapping in any way, but they are added to the output dataframe at the end of the process.
 
 All other arguments are the same, and have the same functionality:
 
 `target_ontology` : str
     Path or URL of 'target' ontology to map the source terms to. When the chosen mapper is BioPortal or Zooma,
     provide a comma-separated list of ontology acronyms (eg 'EFO,HPO') or write 'all' to search all ontologies
+    As of version 2.3.0, passing a recognized acronym to `target_ontology` will generate the download link automatically. This is done using the `bioregistry` python package.
 
 `base_iris` : tuple
     Map only to ontology terms whose IRIs start with one of the strings given in this tuple, for example:
     ('http://www.ebi.ac.uk/efo','http://purl.obolibrary.org/obo/HP')
 
 `source_terms_ids` : tuple
     Collection of identifiers for the given source terms
@@ -153,26 +154,27 @@
 
 `df` : Data frame containing the generated ontology mappings
 
 ### Ontology Caching
 As of version 1.1.0, users can cache ontologies that they want to use regularly or quickly. Programmatically, there are two steps to using the cache: creating the cache, then accessing it. First, the user can cache ontologies using either of two functions:
 
 ```python
-cache_ontology(ontology_url, ontology_acronym, base_iris=())
+cache_ontology(ontology_url, ontology_acronym="", base_iris=())
 ```
 
 ```python
 cache_ontology_set(ontology_registry_path)
 ```
 
-The first of these will cache a single ontology from a URL or file path, with it being referenced by an acronym that will be used to reference it later. An example can be found above.
+The first of these will cache a single ontology from a URL or file path, with it being referenced by an acronym that will be used to reference it later. If no acronym is given, it will use the URL as the cache name. An example can be found above.
 The second function allows the user to cache several ontologies at once by referencing a CSV file of the format:
 `acronym,version,url`. An example is provided in `resources/ontologies.csv`
 
 Once an ontology has been cached by either function, it is stored in a cache folder locally, and thus can be referenced even in different Python instances.
+As of version 2.3.0, the `cache_ontology` function also returns an object that can be used to call any of the `map` functions, as well as `clear_cache` and `cache_exists`. These have the same arguments, except `ontology_target` is not specified and there is no `use_cache` option, as it is always True.
 
 NOTE: Due to how ontologies are processed in memory, `cache_ontology_set` must be used to cache multiple ontologies in a single Python instance. If `cache_ontology` is used multiple times in one instance, the behavior is undefined and may cause visible or invisible errors.
 
 After an ontology is cached, the user can access the cache by using the assigned acronym in the place of `target_ontology` and setting the `use_cache` flag to `True`.
 To clear the cache, one can call:
 `clear_cache(ontology_acronym='')`
 If no arguments are specified, the entire cache will be cleared. Otherwise, only the ontology with the given acronym will be cleared.
```

### Comparing `text2term-2.2.0/setup.py` & `text2term-2.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `text2term-2.2.0/test/test-pypi.py` & `text2term-2.3.0/test/test-pypi.py`

 * *Files identical despite different names*

### Comparing `text2term-2.2.0/text2term/__main__.py` & `text2term-2.3.0/text2term/__main__.py`

 * *Files identical despite different names*

### Comparing `text2term-2.2.0/text2term/bioportal_mapper.py` & `text2term-2.3.0/text2term/bioportal_mapper.py`

 * *Files identical despite different names*

### Comparing `text2term-2.2.0/text2term/onto_utils.py` & `text2term-2.3.0/text2term/onto_utils.py`

 * *Files identical despite different names*

### Comparing `text2term-2.2.0/text2term/preprocess.py` & `text2term-2.3.0/text2term/preprocess.py`

 * *Files identical despite different names*

### Comparing `text2term-2.2.0/text2term/syntactic_mapper.py` & `text2term-2.3.0/text2term/syntactic_mapper.py`

 * *Files identical despite different names*

### Comparing `text2term-2.2.0/text2term/t2t.py` & `text2term-2.3.0/text2term/t2t.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-"""Provides Text2Term class"""
 import os
 import sys
 import json
 import pickle
 import time
 import datetime
 import owlready2
 import pandas as pd
-from shutil import rmtree
 from text2term import onto_utils
 from text2term.mapper import Mapper
+from text2term import onto_cache
 from text2term.term_collector import OntologyTermCollector
 from text2term.term_graph_generator import TermGraphGenerator
 from text2term.bioportal_mapper import BioPortalAnnotatorMapper
 from text2term.syntactic_mapper import SyntacticMapper
 from text2term.tfidf_mapper import TFIDFMapper
 from text2term.zooma_mapper import ZoomaMapper
 from text2term.config import VERSION
@@ -104,15 +103,15 @@
             df.loc[df['Source Term'] == key, "Tags"] = to_store
     else: 
         for term in tagged_terms_dict:
             to_store = ','.join(term.get_tags())
             df.loc[df['Source Term'] == term.get_term(), "Tags"] = to_store
 
     if save_mappings:
-        _save_mappings(df, output_file, min_score, mapper, target_ontology, base_iris, excl_deprecated, max_mappings)
+        _save_mappings(df, output_file, min_score, mapper, target_ontology, base_iris, excl_deprecated, max_mappings, term_type)
     return df
 
 """
 Maps the terms in the given list to the specified target ontology.
 
 Parameters
 ----------
@@ -159,59 +158,32 @@
         output_file = "t2t-mappings-" + timestamp + ".csv"
     if mapper in {Mapper.ZOOMA, Mapper.BIOPORTAL}:
         target_terms = '' if target_ontology.lower() == 'all' else target_ontology
     else:
         target_terms = _load_ontology(target_ontology, base_iris, excl_deprecated, use_cache, term_type)
     mappings_df = _do_mapping(source_terms, source_terms_ids, target_terms, mapper, max_mappings, min_score)
     if save_mappings:
-        _save_mappings(mappings_df, output_file, min_score, mapper, target_ontology, base_iris, excl_deprecated, max_mappings)
+        _save_mappings(mappings_df, output_file, min_score, mapper, target_ontology, base_iris, excl_deprecated, max_mappings, term_type)
     if save_graphs:
         _save_graphs(target_terms, output_file)
     return mappings_df
 
-"""
-CACHING FUNCTIONS -- Public
-"""
-# Caches many ontologies from a csv
-def cache_ontology_set(ontology_registry_path):
-    registry = pd.read_csv(ontology_registry_path)
-    for index, row in registry.iterrows():
-        try:
-            cache_ontology(row.url, row.acronym)
-        except Exception as err:
-            sys.stderr.write("Could not cache ontology", row.acronym, "due to error:", err)
-        owlready2.default_world.ontologies.clear()
-
 # Caches a single ontology
-def cache_ontology(ontology_url, ontology_acronym, base_iris=()):
+def cache_ontology(ontology_url, ontology_acronym="", base_iris=()):
+    if ontology_acronym == "":
+        ontology_acronym = ontology_url
     ontology_terms = _load_ontology(ontology_url, base_iris, exclude_deprecated=False, term_type='both')
     cache_dir = "cache/" + ontology_acronym + "/"
     if not os.path.exists(cache_dir):
         os.makedirs(cache_dir)
 
     _serialize_ontology(ontology_terms, ontology_acronym, cache_dir)
     _save_graphs(ontology_terms, output_file=cache_dir + ontology_acronym)
     ontology_terms.clear()
-
-# Will check if an acronym exists in the cache
-def cache_exists(ontology_acronym=''):
-    return os.path.exists("cache/" + ontology_acronym)
-
-# Clears the cache
-def clear_cache(ontology_acronym=''):
-    cache_dir = "cache/" 
-    if ontology_acronym != '':
-        cache_dir = os.path.join(cache_dir, ontology_acronym)
-    # Is equivalent to: rm -r cache_dir
-    try:
-        rmtree(cache_dir)
-        sys.stderr.write("Cache has been cleared successfully")
-    except OSError as error:
-        sys.stderr.write("Cache cannot be removed:")
-        sys.stderr.write(error)
+    return onto_cache.OntologyCache(ontology_acronym)
 
 """
 PRIVATE/HELPER FUNCTIONS
 """
 def _serialize_ontology(ontology_terms, ontology_acronym, cache_dir):
     start = time.time()
     with open(cache_dir + ontology_acronym + "-term-details.pickle", 'wb+') as out_file:
@@ -256,26 +228,27 @@
         return term_mapper.map(source_terms, source_term_ids, ontologies=ontology_terms, max_mappings=max_mappings)
     elif mapper in {Mapper.LEVENSHTEIN, Mapper.JARO, Mapper.JARO_WINKLER, Mapper.INDEL, Mapper.FUZZY, Mapper.JACCARD}:
         term_mapper = SyntacticMapper(ontology_terms)
         return term_mapper.map(source_terms, source_term_ids, mapper, max_mappings=max_mappings)
     else:
         raise ValueError("Unsupported mapper: " + mapper)
 
-def _save_mappings(mappings, output_file, min_score, mapper, target_ontology, base_iris, excl_deprecated, max_mappings):
+def _save_mappings(mappings, output_file, min_score, mapper, target_ontology, base_iris, excl_deprecated, max_mappings, term_type):
     if os.path.dirname(output_file):  # create output directories if needed
         os.makedirs(os.path.dirname(output_file), exist_ok=True)
     with open(output_file, "a") as f:
         f.write("# Date and time run: %s\n" % datetime.datetime.now())
         f.write("# Target Ontology: %s\n" % target_ontology)
         f.write("# Text2term version: %s\n" % VERSION)
         f.write("# Minimum Score: %.2f\n" % min_score)
         f.write("# Mapper: %s\n" % mapper.value)
         f.write("# Base IRIs: %s\n" % (base_iris,))
         f.write("# Max Mappings: %d\n" % max_mappings)
-        f.write("# Depricated Terms ")
+        f.write("# Term Type: %s\n" % term_type)
+        f.write("# Deprecated Terms ")
         f.write("Excluded\n" if excl_deprecated else "Included\n")
     mappings.to_csv(output_file, index=False, mode='a')
 
 def _save_graphs(terms, output_file):
     term_graphs = TermGraphGenerator(terms).graphs_dicts()
     with open(output_file + "-term-graphs.json", 'w') as json_file:
         json.dump(term_graphs, json_file, indent=2)
```

### Comparing `text2term-2.2.0/text2term/tagged_terms.py` & `text2term-2.3.0/text2term/tagged_terms.py`

 * *Files identical despite different names*

### Comparing `text2term-2.2.0/text2term/term.py` & `text2term-2.3.0/text2term/term.py`

 * *Files identical despite different names*

### Comparing `text2term-2.2.0/text2term/term_collector.py` & `text2term-2.3.0/text2term/term_collector.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Provides OntologyTermCollector class"""
 
 from owlready2 import *
 from text2term import onto_utils
 from text2term.term import OntologyTerm
 import logging
+import bioregistry
 
-options = ['classes', 'properties', 'both']
 
 class OntologyTermCollector:
 
     def __init__(self, log_level=logging.INFO):
         self.logger = onto_utils.get_logger(__name__, level=log_level)
 
     def get_ontology_terms(self, ontology_iri, base_iris=(), use_reasoning=False, exclude_deprecated=False, term_type="classes"):
@@ -171,31 +171,33 @@
             label_from_iri = onto_utils.label_from_iri(ontology_term.iri)
             self.logger.debug("...ontology term %s has no labels (rdfs:label or skos:prefLabel). "
                               "Using a label based on the term IRI: %s", ontology_term.iri, label_from_iri)
             labels.add(label_from_iri)
         self.logger.debug("...collected %i labels and synonyms for %s", len(labels), ontology_term)
         return labels
 
-    def _get_synonyms(self, ontology_term):
+    def _get_synonyms(self, ontology_term, include_broad_synonyms=False):
         """
         Collect the synonyms of the given ontology term
         :param ontology_term: Ontology term
+        :param include_broad_synonyms: true if broad (i.e. more generic) synonyms should be included, false otherwise
         :return: Collection of synonyms of the ontology term
         """
         synonyms = set()
         for synonym in self._get_obo_exact_synonyms(ontology_term):
             synonyms.add(synonym)
         for synonym in self._get_obo_related_synonyms(ontology_term):
             synonyms.add(synonym)
-        for synonym in self._get_obo_broad_synonyms(ontology_term):
-            synonyms.add(synonym)
         for nci_synonym in self._get_nci_synonyms(ontology_term):
             synonyms.add(nci_synonym)
         for efo_alt_term in self._get_efo_alt_terms(ontology_term):
             synonyms.add(efo_alt_term)
+        if include_broad_synonyms:
+            for synonym in self._get_obo_broad_synonyms(ontology_term):
+                synonyms.add(synonym)
         self.logger.debug("...collected %i synonyms for %s", len(synonyms), ontology_term)
         return synonyms
 
     def _get_rdfs_labels(self, ontology_term):
         """
         Collect labels of the given term that are specified using the standard rdfs:label annotation property
         :param ontology_term: Ontology term to collect labels from
@@ -332,14 +334,17 @@
         """
         Load the ontology at the specified IRI.
         :param ontology_iri: IRI of the ontology (e.g., path of ontology document in the local file system, URL)
         :return: Ontology document
         """
         self.logger.info("Loading ontology %s...", ontology_iri)
         start = time.time()
+        owl_link = bioregistry.get_owl_download(ontology_iri)
+        if owl_link != None:
+            ontology_iri = owl_link
         ontology = get_ontology(ontology_iri).load()
         end = time.time()
         self._log_ontology_metrics(ontology)
         self.logger.info("...done (ontology loading time: %.2fs)", end - start)
         return ontology
 
     def _classify_ontology(self, ontology):
```

### Comparing `text2term-2.2.0/text2term/term_graph.py` & `text2term-2.3.0/text2term/term_graph.py`

 * *Files identical despite different names*

### Comparing `text2term-2.2.0/text2term/term_graph_generator.py` & `text2term-2.3.0/text2term/term_graph_generator.py`

 * *Files identical despite different names*

### Comparing `text2term-2.2.0/text2term/term_mapping.py` & `text2term-2.3.0/text2term/term_mapping.py`

 * *Files identical despite different names*

### Comparing `text2term-2.2.0/text2term/tfidf_mapper.py` & `text2term-2.3.0/text2term/tfidf_mapper.py`

 * *Files identical despite different names*

### Comparing `text2term-2.2.0/text2term/zooma_mapper.py` & `text2term-2.3.0/text2term/zooma_mapper.py`

 * *Files identical despite different names*

### Comparing `text2term-2.2.0/text2term.egg-info/PKG-INFO` & `text2term-2.3.0/text2term.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2term
-Version: 2.2.0
+Version: 2.3.0
 Summary: A tool for mapping free-text descriptions of (biomedical) entities to controlled terms in ontologies
 Home-page: https://github.com/ccb-hms/ontology-mapper
 Author: Center for Computational Biomedicine, Harvard Medical School
 Author-email: rafael_goncalves@hms.harvard.edu
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -124,14 +124,15 @@
 For `map_tagged_terms`, everything is the same as `map_terms` except the first argument is either a dictionary of terms to a list of tags, or a list of TaggedTerm objects (see below). Currently, the tags do not affect the mapping in any way, but they are added to the output dataframe at the end of the process.
 
 All other arguments are the same, and have the same functionality:
 
 `target_ontology` : str
     Path or URL of 'target' ontology to map the source terms to. When the chosen mapper is BioPortal or Zooma,
     provide a comma-separated list of ontology acronyms (eg 'EFO,HPO') or write 'all' to search all ontologies
+    As of version 2.3.0, passing a recognized acronym to `target_ontology` will generate the download link automatically. This is done using the `bioregistry` python package.
 
 `base_iris` : tuple
     Map only to ontology terms whose IRIs start with one of the strings given in this tuple, for example:
     ('http://www.ebi.ac.uk/efo','http://purl.obolibrary.org/obo/HP')
 
 `source_terms_ids` : tuple
     Collection of identifiers for the given source terms
@@ -172,26 +173,27 @@
 
 `df` : Data frame containing the generated ontology mappings
 
 ### Ontology Caching
 As of version 1.1.0, users can cache ontologies that they want to use regularly or quickly. Programmatically, there are two steps to using the cache: creating the cache, then accessing it. First, the user can cache ontologies using either of two functions:
 
 ```python
-cache_ontology(ontology_url, ontology_acronym, base_iris=())
+cache_ontology(ontology_url, ontology_acronym="", base_iris=())
 ```
 
 ```python
 cache_ontology_set(ontology_registry_path)
 ```
 
-The first of these will cache a single ontology from a URL or file path, with it being referenced by an acronym that will be used to reference it later. An example can be found above.
+The first of these will cache a single ontology from a URL or file path, with it being referenced by an acronym that will be used to reference it later. If no acronym is given, it will use the URL as the cache name. An example can be found above.
 The second function allows the user to cache several ontologies at once by referencing a CSV file of the format:
 `acronym,version,url`. An example is provided in `resources/ontologies.csv`
 
 Once an ontology has been cached by either function, it is stored in a cache folder locally, and thus can be referenced even in different Python instances.
+As of version 2.3.0, the `cache_ontology` function also returns an object that can be used to call any of the `map` functions, as well as `clear_cache` and `cache_exists`. These have the same arguments, except `ontology_target` is not specified and there is no `use_cache` option, as it is always True.
 
 NOTE: Due to how ontologies are processed in memory, `cache_ontology_set` must be used to cache multiple ontologies in a single Python instance. If `cache_ontology` is used multiple times in one instance, the behavior is undefined and may cause visible or invisible errors.
 
 After an ontology is cached, the user can access the cache by using the assigned acronym in the place of `target_ontology` and setting the `use_cache` flag to `True`.
 To clear the cache, one can call:
 `clear_cache(ontology_acronym='')`
 If no arguments are specified, the entire cache will be cleared. Otherwise, only the ontology with the given acronym will be cleared.
```

### Comparing `text2term-2.2.0/text2term.egg-info/SOURCES.txt` & `text2term-2.3.0/text2term.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 setup.py
 test/test-pypi.py
 text2term/__init__.py
 text2term/__main__.py
 text2term/bioportal_mapper.py
 text2term/config.py
 text2term/mapper.py
+text2term/onto_cache.py
 text2term/onto_utils.py
 text2term/preprocess.py
 text2term/syntactic_mapper.py
 text2term/t2t.py
 text2term/tagged_terms.py
 text2term/term.py
 text2term/term_collector.py
```

