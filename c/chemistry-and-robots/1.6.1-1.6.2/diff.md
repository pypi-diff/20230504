# Comparing `tmp/chemistry_and_robots-1.6.1.tar.gz` & `tmp/chemistry_and_robots-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chemistry_and_robots-1.6.1.tar", last modified: Fri Apr 28 12:56:56 2023, max compression
+gzip compressed data, was "chemistry_and_robots-1.6.2.tar", last modified: Thu May  4 17:18:43 2023, max compression
```

## Comparing `chemistry_and_robots-1.6.1.tar` & `chemistry_and_robots-1.6.2.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-04-28 12:56:56.481541 chemistry_and_robots-1.6.1/
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)      772 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.1/MANIFEST.in
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     8652 2023-04-28 12:56:56.481541 chemistry_and_robots-1.6.1/PKG-INFO
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     8187 2023-01-20 09:52:31.000000 chemistry_and_robots-1.6.1/README.md
-drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-04-28 12:56:56.401540 chemistry_and_robots-1.6.1/chemistry_and_robots/
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)       78 2023-04-28 12:49:16.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/__init__.py
-drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-04-28 12:56:56.411541 chemistry_and_robots-1.6.1/chemistry_and_robots/data_model/
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)      150 2022-09-02 15:03:43.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/data_model/__init__.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     8002 2023-01-20 09:52:31.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/data_model/base_ontology.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)    24268 2023-04-27 12:30:16.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/data_model/iris.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)      267 2022-09-02 15:03:43.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/data_model/ontobpr.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)    14466 2023-04-27 12:45:27.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/data_model/ontodoe.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     6132 2023-04-27 12:27:27.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/data_model/ontohplc.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     7159 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/data_model/ontolab.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)    36143 2023-04-28 12:38:36.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/data_model/ontoreaction.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)    33784 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/data_model/ontovapourtec.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     2675 2023-04-27 12:27:27.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/data_model/unit_conversion.py
-drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-04-28 12:56:56.411541 chemistry_and_robots-1.6.1/chemistry_and_robots/hardware/
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)        0 2022-09-02 15:03:43.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/hardware/__init__.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     2679 2023-01-20 09:52:31.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/hardware/hplc.py
-drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-04-28 12:56:56.421541 chemistry_and_robots-1.6.1/chemistry_and_robots/kg_operations/
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)       58 2022-09-04 20:28:19.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/kg_operations/__init__.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     3261 2023-01-20 09:52:31.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/kg_operations/dict_and_list.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)   151217 2023-04-27 14:58:00.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/kg_operations/sparql_client.py
-drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-04-28 12:56:56.421541 chemistry_and_robots-1.6.1/chemistry_and_robots/resources/
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)      585 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/resources/__init__.py
-drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-04-28 12:56:56.431541 chemistry_and_robots-1.6.1/chemistry_and_robots/resources/ontoagent/
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     1551 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/resources/ontoagent/Service__DoE.ttl
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     1516 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/resources/ontoagent/Service__Execution.ttl
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     1551 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/resources/ontoagent/Service__PostProc.ttl
-drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-04-28 12:56:56.441541 chemistry_and_robots-1.6.1/chemistry_and_robots/resources/ontology/
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)    33232 2023-04-28 12:49:54.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/resources/ontology/OntoDoE.owl
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)    21430 2023-04-28 12:50:07.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/resources/ontology/OntoGoal.owl
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)    27346 2023-04-28 12:50:01.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/resources/ontology/OntoHPLC.owl
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)    36783 2023-04-28 12:49:59.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/resources/ontology/OntoLab.owl
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)    52477 2023-04-28 12:49:57.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/resources/ontology/OntoReaction.owl
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)    62442 2023-04-28 12:50:04.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/resources/ontology/OntoVapourtec.owl
-drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-04-28 12:56:56.461541 chemistry_and_robots-1.6.1/chemistry_and_robots/resources/sample_data/
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     5426 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/resources/sample_data/doe.ttl
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     5366 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/resources/sample_data/doe_no_prior_data.ttl
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     5500 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/resources/sample_data/doe_template.ttl
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)    57959 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/resources/sample_data/dummy_lab.ttl
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     7144 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/resources/sample_data/dummy_post_proc.ttl
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)    23351 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/resources/sample_data/new_exp_data.ttl
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)    40339 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/resources/sample_data/new_exp_data_out_of_range.ttl
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)      124 2023-01-20 09:52:31.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/resources/sample_data/raw_hplc_report_txt.txt
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)      298 2023-01-20 09:52:31.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/resources/sample_data/raw_hplc_report_txt_incomplete.txt
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)      111 2023-01-20 09:52:31.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/resources/sample_data/raw_hplc_report_txt_no_product.txt
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)      416 2023-01-20 09:52:31.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/resources/sample_data/raw_hplc_report_txt_unidentified_peaks.txt
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)    25600 2023-01-20 09:52:31.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/resources/sample_data/raw_hplc_report_xls.xls
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)    25600 2023-01-20 09:52:31.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/resources/sample_data/raw_hplc_report_xls_incomplete.xls
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)    25600 2023-01-20 09:52:31.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/resources/sample_data/raw_hplc_report_xls_no_product.xls
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)    26112 2023-01-20 09:52:31.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/resources/sample_data/raw_hplc_report_xls_unidentified_peaks.xls
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)    67322 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/resources/sample_data/rxn_data.ttl
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     8080 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/resources/sample_data/rxn_queue_test.ttl
-drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-04-28 12:56:56.481541 chemistry_and_robots-1.6.1/chemistry_and_robots/tests/
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)        0 2022-09-02 15:03:43.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/tests/__init__.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)    43077 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/tests/conftest.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     4414 2022-09-02 15:03:43.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/tests/test_base_ontology.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     4720 2023-01-20 09:52:31.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/tests/test_dict_and_list.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)      663 2023-01-20 09:52:31.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/tests/test_example_triples.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)    10992 2023-01-20 09:52:31.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/tests/test_hash_eq.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     3610 2023-04-27 12:27:27.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/tests/test_hplc.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     1569 2023-04-27 12:27:27.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/tests/test_ontodoe.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)    30117 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/tests/test_single_phase.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)    90116 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.1/chemistry_and_robots/tests/test_sparql_client.py
-drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-04-28 12:56:56.411541 chemistry_and_robots-1.6.1/chemistry_and_robots.egg-info/
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     8652 2023-04-28 12:56:56.000000 chemistry_and_robots-1.6.1/chemistry_and_robots.egg-info/PKG-INFO
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     3135 2023-04-28 12:56:56.000000 chemistry_and_robots-1.6.1/chemistry_and_robots.egg-info/SOURCES.txt
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)        1 2023-04-28 12:56:56.000000 chemistry_and_robots-1.6.1/chemistry_and_robots.egg-info/dependency_links.txt
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)      157 2023-04-28 12:56:56.000000 chemistry_and_robots-1.6.1/chemistry_and_robots.egg-info/requires.txt
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)       21 2023-04-28 12:56:56.000000 chemistry_and_robots-1.6.1/chemistry_and_robots.egg-info/top_level.txt
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)       38 2023-04-28 12:56:56.481541 chemistry_and_robots-1.6.1/setup.cfg
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)      990 2023-04-28 12:49:16.000000 chemistry_and_robots-1.6.1/setup.py
+drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-05-04 17:18:43.888763 chemistry_and_robots-1.6.2/
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)      772 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.2/MANIFEST.in
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     8652 2023-05-04 17:18:43.888763 chemistry_and_robots-1.6.2/PKG-INFO
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     8187 2023-01-20 09:52:31.000000 chemistry_and_robots-1.6.2/README.md
+drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-05-04 17:18:43.838763 chemistry_and_robots-1.6.2/chemistry_and_robots/
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)       78 2023-05-04 17:10:13.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/__init__.py
+drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-05-04 17:18:43.848763 chemistry_and_robots-1.6.2/chemistry_and_robots/data_model/
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)      150 2022-09-02 15:03:43.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/data_model/__init__.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     8002 2023-01-20 09:52:31.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/data_model/base_ontology.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    24268 2023-04-28 14:15:32.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/data_model/iris.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)      267 2022-09-02 15:03:43.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/data_model/ontobpr.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    14466 2023-04-28 14:15:32.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/data_model/ontodoe.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     6132 2023-04-27 12:27:27.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/data_model/ontohplc.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     7159 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/data_model/ontolab.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    36143 2023-04-28 14:15:32.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/data_model/ontoreaction.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    33784 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/data_model/ontovapourtec.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     2675 2023-04-27 12:27:27.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/data_model/unit_conversion.py
+drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-05-04 17:18:43.848763 chemistry_and_robots-1.6.2/chemistry_and_robots/hardware/
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)        0 2022-09-02 15:03:43.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/hardware/__init__.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     2679 2023-01-20 09:52:31.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/hardware/hplc.py
+drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-05-04 17:18:43.848763 chemistry_and_robots-1.6.2/chemistry_and_robots/kg_operations/
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)       58 2022-09-04 20:28:19.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/kg_operations/__init__.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     3261 2023-01-20 09:52:31.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/kg_operations/dict_and_list.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)   151217 2023-04-28 14:15:32.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/kg_operations/sparql_client.py
+drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-05-04 17:18:43.858763 chemistry_and_robots-1.6.2/chemistry_and_robots/resources/
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)      585 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/resources/__init__.py
+drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-05-04 17:18:43.858763 chemistry_and_robots-1.6.2/chemistry_and_robots/resources/ontoagent/
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     1551 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/resources/ontoagent/Service__DoE.ttl
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     1516 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/resources/ontoagent/Service__Execution.ttl
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     1551 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/resources/ontoagent/Service__PostProc.ttl
+drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-05-04 17:18:43.858763 chemistry_and_robots-1.6.2/chemistry_and_robots/resources/ontology/
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    32981 2023-05-04 17:10:59.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/resources/ontology/OntoDoE.owl
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    21428 2023-05-04 17:11:20.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/resources/ontology/OntoGoal.owl
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    27344 2023-05-04 17:11:10.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/resources/ontology/OntoHPLC.owl
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    37208 2023-05-04 17:11:07.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/resources/ontology/OntoLab.owl
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    52475 2023-05-04 17:11:03.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/resources/ontology/OntoReaction.owl
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    62440 2023-05-04 17:11:17.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/resources/ontology/OntoVapourtec.owl
+drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-05-04 17:18:43.858763 chemistry_and_robots-1.6.2/chemistry_and_robots/resources/sample_data/
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     5426 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/resources/sample_data/doe.ttl
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     5366 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/resources/sample_data/doe_no_prior_data.ttl
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     5500 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/resources/sample_data/doe_template.ttl
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    57959 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/resources/sample_data/dummy_lab.ttl
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     7144 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/resources/sample_data/dummy_post_proc.ttl
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    23351 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/resources/sample_data/new_exp_data.ttl
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    40339 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/resources/sample_data/new_exp_data_out_of_range.ttl
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)      124 2023-01-20 09:52:31.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/resources/sample_data/raw_hplc_report_txt.txt
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)      298 2023-01-20 09:52:31.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/resources/sample_data/raw_hplc_report_txt_incomplete.txt
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)      111 2023-01-20 09:52:31.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/resources/sample_data/raw_hplc_report_txt_no_product.txt
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)      416 2023-01-20 09:52:31.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/resources/sample_data/raw_hplc_report_txt_unidentified_peaks.txt
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    25600 2023-01-20 09:52:31.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/resources/sample_data/raw_hplc_report_xls.xls
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    25600 2023-01-20 09:52:31.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/resources/sample_data/raw_hplc_report_xls_incomplete.xls
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    25600 2023-01-20 09:52:31.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/resources/sample_data/raw_hplc_report_xls_no_product.xls
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    26112 2023-01-20 09:52:31.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/resources/sample_data/raw_hplc_report_xls_unidentified_peaks.xls
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    67322 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/resources/sample_data/rxn_data.ttl
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     8080 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/resources/sample_data/rxn_queue_test.ttl
+drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-05-04 17:18:43.878763 chemistry_and_robots-1.6.2/chemistry_and_robots/tests/
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)        0 2022-09-02 15:03:43.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/tests/__init__.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    43077 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/tests/conftest.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     4414 2022-09-02 15:03:43.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/tests/test_base_ontology.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     4720 2023-01-20 09:52:31.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/tests/test_dict_and_list.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)      663 2023-01-20 09:52:31.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/tests/test_example_triples.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    10992 2023-01-20 09:52:31.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/tests/test_hash_eq.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     3610 2023-04-27 12:27:27.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/tests/test_hplc.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     1569 2023-04-27 12:27:27.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/tests/test_ontodoe.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    30117 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/tests/test_single_phase.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    90116 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.2/chemistry_and_robots/tests/test_sparql_client.py
+drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-05-04 17:18:43.838763 chemistry_and_robots-1.6.2/chemistry_and_robots.egg-info/
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     8652 2023-05-04 17:18:43.000000 chemistry_and_robots-1.6.2/chemistry_and_robots.egg-info/PKG-INFO
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     3135 2023-05-04 17:18:43.000000 chemistry_and_robots-1.6.2/chemistry_and_robots.egg-info/SOURCES.txt
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)        1 2023-05-04 17:18:43.000000 chemistry_and_robots-1.6.2/chemistry_and_robots.egg-info/dependency_links.txt
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)      157 2023-05-04 17:18:43.000000 chemistry_and_robots-1.6.2/chemistry_and_robots.egg-info/requires.txt
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)       21 2023-05-04 17:18:43.000000 chemistry_and_robots-1.6.2/chemistry_and_robots.egg-info/top_level.txt
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)       38 2023-05-04 17:18:43.888763 chemistry_and_robots-1.6.2/setup.cfg
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)      990 2023-05-04 17:10:13.000000 chemistry_and_robots-1.6.2/setup.py
```

### Comparing `chemistry_and_robots-1.6.1/MANIFEST.in` & `chemistry_and_robots-1.6.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.6.1/PKG-INFO` & `chemistry_and_robots-1.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chemistry_and_robots
-Version: 1.6.1
+Version: 1.6.2
 Summary: chemistryandrobots contains dataclasses and sparql queries for concepts related to chemistry_and_robots as part of The World Avatar project.
 Home-page: https://github.com/cambridge-cares/TheWorldAvatar/tree/main/Agents/utils/chemistry_and_robots
 Author: Jiaru Bai
 Author-email: jb2197@cam.ac.uk
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `chemistry_and_robots-1.6.1/README.md` & `chemistry_and_robots-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots/data_model/base_ontology.py` & `chemistry_and_robots-1.6.2/chemistry_and_robots/data_model/base_ontology.py`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots/data_model/iris.py` & `chemistry_and_robots-1.6.2/chemistry_and_robots/data_model/iris.py`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots/data_model/ontodoe.py` & `chemistry_and_robots-1.6.2/chemistry_and_robots/data_model/ontodoe.py`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots/data_model/ontohplc.py` & `chemistry_and_robots-1.6.2/chemistry_and_robots/data_model/ontohplc.py`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots/data_model/ontolab.py` & `chemistry_and_robots-1.6.2/chemistry_and_robots/data_model/ontolab.py`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots/data_model/ontoreaction.py` & `chemistry_and_robots-1.6.2/chemistry_and_robots/data_model/ontoreaction.py`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots/data_model/ontovapourtec.py` & `chemistry_and_robots-1.6.2/chemistry_and_robots/data_model/ontovapourtec.py`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots/data_model/unit_conversion.py` & `chemistry_and_robots-1.6.2/chemistry_and_robots/data_model/unit_conversion.py`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots/hardware/hplc.py` & `chemistry_and_robots-1.6.2/chemistry_and_robots/hardware/hplc.py`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots/kg_operations/dict_and_list.py` & `chemistry_and_robots-1.6.2/chemistry_and_robots/kg_operations/dict_and_list.py`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots/kg_operations/sparql_client.py` & `chemistry_and_robots-1.6.2/chemistry_and_robots/kg_operations/sparql_client.py`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots/resources/__init__.py` & `chemistry_and_robots-1.6.2/chemistry_and_robots/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots/resources/ontoagent/Service__DoE.ttl` & `chemistry_and_robots-1.6.2/chemistry_and_robots/resources/ontoagent/Service__DoE.ttl`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots/resources/ontoagent/Service__Execution.ttl` & `chemistry_and_robots-1.6.2/chemistry_and_robots/resources/ontoagent/Service__Execution.ttl`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots/resources/ontoagent/Service__PostProc.ttl` & `chemistry_and_robots-1.6.2/chemistry_and_robots/resources/ontoagent/Service__PostProc.ttl`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots/resources/ontology/OntoDoE.owl` & `chemistry_and_robots-1.6.2/chemistry_and_robots/resources/ontology/OntoDoE.owl`

 * *Files 0% similar despite different names*

#### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots/resources/ontology/OntoDoE.owl` & `chemistry_and_robots-1.6.2/chemistry_and_robots/resources/ontology/OntoDoE.owl`

```diff
@@ -1,13 +1,13 @@
 <?xml version="1.0" encoding="utf-8"?>
 <rdf:RDF xmlns="https://www.theworldavatar.com/kg/ontodoe/" xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#" xmlns:owl="http://www.w3.org/2002/07/owl#" xmlns:xml="http://www.w3.org/XML/1998/namespace" xmlns:xsd="http://www.w3.org/2001/XMLSchema#" xmlns:rdfs="http://www.w3.org/2000/01/rdf-schema#" xmlns:dc="http://purl.org/dc/elements/1.1/" xmlns:ontodoe="https://www.theworldavatar.com/kg/ontodoe/" xml:base="https://www.theworldavatar.com/kg/ontodoe/">
   <owl:Ontology rdf:about="https://www.theworldavatar.com/kg/ontodoe/">
-    <dc:date rdf:datatype="http://www.w3.org/2001/XMLSchema#string">28 April 2023</dc:date>
+    <dc:date rdf:datatype="http://www.w3.org/2001/XMLSchema#string">04 May 2023</dc:date>
     <rdfs:comment rdf:datatype="http://www.w3.org/2001/XMLSchema#string">An ontology developed for design of experiment.</rdfs:comment>
-    <owl:versionInfo rdf:datatype="http://www.w3.org/2001/XMLSchema#string">1.10</owl:versionInfo>
+    <owl:versionInfo rdf:datatype="http://www.w3.org/2001/XMLSchema#string">1.11</owl:versionInfo>
     <gitCommitHash rdf:datatype="http://www.w3.org/2001/XMLSchema#string">c0599beca8df55873a1ab061dee64e52c510c6a0</gitCommitHash>
   </owl:Ontology>
   <!-- 
     ///////////////////////////////////////////////////////////////////////////////////////
     //
     // Object Properties
     //
@@ -61,15 +61,15 @@
     <rdfs:range rdf:resource="https://www.theworldavatar.com/kg/ontoreaction/ReactionExperiment"/>
     <rdfs:comment rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A relation between a design of experiment exercise and the new experiment it defines.</rdfs:comment>
     <rdfs:isDefinedBy rdf:datatype="http://www.w3.org/2001/XMLSchema#string">https://www.theworldavatar.com/kg/ontodoe/</rdfs:isDefinedBy>
   </owl:ObjectProperty>
   <!-- https://www.theworldavatar.com/kg/ontodoe/refersToExperiment -->
   <owl:ObjectProperty rdf:about="https://www.theworldavatar.com/kg/ontodoe/refersToExperiment">
     <rdfs:domain rdf:resource="https://www.theworldavatar.com/kg/ontodoe/HistoricalData"/>
-    <rdfs:range rdf:resource="http://www.theworldavatar.com/ontology/ontoreaction/OntoReaction.owl#ReactionExperiment"/>
+    <rdfs:range rdf:resource="https://www.theworldavatar.com/kg/ontoreaction/ReactionExperiment"/>
     <rdfs:comment rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A relation between previous experiment records/future experiment conditions and the reaction experiment it refers to.</rdfs:comment>
     <rdfs:isDefinedBy rdf:datatype="http://www.w3.org/2001/XMLSchema#string">https://www.theworldavatar.com/kg/ontodoe/</rdfs:isDefinedBy>
   </owl:ObjectProperty>
   <!-- https://www.theworldavatar.com/kg/ontodoe/refersToQuantity -->
   <owl:ObjectProperty rdf:about="https://www.theworldavatar.com/kg/ontodoe/refersToQuantity">
     <rdfs:domain>
       <owl:Class>
@@ -196,16 +196,14 @@
     //
     // Classes
     //
     ///////////////////////////////////////////////////////////////////////////////////////
      -->
   <!-- http://www.ontology-of-units-of-measure.org/resource/om-2/Quantity -->
   <owl:Class rdf:about="http://www.ontology-of-units-of-measure.org/resource/om-2/Quantity"/>
-  <!-- http://www.theworldavatar.com/ontology/ontoreaction/OntoReaction.owl#ReactionExperiment -->
-  <owl:Class rdf:about="http://www.theworldavatar.com/ontology/ontoreaction/OntoReaction.owl#ReactionExperiment"/>
   <!-- https://www.theworldavatar.com/kg/ontodoe/CategoricalVariable -->
   <owl:Class rdf:about="https://www.theworldavatar.com/kg/ontodoe/CategoricalVariable">
     <rdfs:subClassOf rdf:resource="https://www.theworldavatar.com/kg/ontodoe/DesignVariable"/>
     <rdfs:subClassOf>
       <owl:Restriction>
         <owl:onProperty rdf:resource="https://www.theworldavatar.com/kg/ontodoe/refersToQuantity"/>
         <owl:qualifiedCardinality rdf:datatype="http://www.w3.org/2001/XMLSchema#nonNegativeInteger">1</owl:qualifiedCardinality>
```

### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots/resources/ontology/OntoGoal.owl` & `chemistry_and_robots-1.6.2/chemistry_and_robots/resources/ontology/OntoGoal.owl`

 * *Files 1% similar despite different names*

#### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots/resources/ontology/OntoGoal.owl` & `chemistry_and_robots-1.6.2/chemistry_and_robots/resources/ontology/OntoGoal.owl`

```diff
@@ -1,11 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
 <rdf:RDF xmlns="https://www.theworldavatar.com/kg/ontogoal/" xmlns:ontogoal="https://www.theworldavatar.com/kg/ontogoal/" xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#" xmlns:owl="http://www.w3.org/2002/07/owl#" xmlns:xml="http://www.w3.org/XML/1998/namespace" xmlns:xsd="http://www.w3.org/2001/XMLSchema#" xmlns:rdfs="http://www.w3.org/2000/01/rdf-schema#" xmlns:dc="http://purl.org/dc/elements/1.1/" xml:base="https://www.theworldavatar.com/kg/ontogoal/">
   <owl:Ontology rdf:about="https://www.theworldavatar.com/kg/ontogoal/">
-    <dc:date rdf:datatype="http://www.w3.org/2001/XMLSchema#string">28 April 2023</dc:date>
+    <dc:date rdf:datatype="http://www.w3.org/2001/XMLSchema#string">04 May 2023</dc:date>
     <rdfs:comment rdf:datatype="http://www.w3.org/2001/XMLSchema#string">An ontology developed for goal-based agent operation.</rdfs:comment>
     <owl:versionInfo rdf:datatype="http://www.w3.org/2001/XMLSchema#string">1.3</owl:versionInfo>
     <gitCommitHash rdf:datatype="http://www.w3.org/2001/XMLSchema#string">c0599beca8df55873a1ab061dee64e52c510c6a0</gitCommitHash>
   </owl:Ontology>
   <!-- 
     ///////////////////////////////////////////////////////////////////////////////////////
     //
```

### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots/resources/ontology/OntoHPLC.owl` & `chemistry_and_robots-1.6.2/chemistry_and_robots/resources/ontology/OntoHPLC.owl`

 * *Files 1% similar despite different names*

#### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots/resources/ontology/OntoHPLC.owl` & `chemistry_and_robots-1.6.2/chemistry_and_robots/resources/ontology/OntoHPLC.owl`

```diff
@@ -1,11 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
 <rdf:RDF xmlns="https://www.theworldavatar.com/kg/ontohplc/" xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#" xmlns:owl="http://www.w3.org/2002/07/owl#" xmlns:xml="http://www.w3.org/XML/1998/namespace" xmlns:ontohplc="https://www.theworldavatar.com/kg/ontohplc/" xmlns:xsd="http://www.w3.org/2001/XMLSchema#" xmlns:rdfs="http://www.w3.org/2000/01/rdf-schema#" xmlns:dc="http://purl.org/dc/elements/1.1/" xml:base="https://www.theworldavatar.com/kg/ontohplc/">
   <owl:Ontology rdf:about="https://www.theworldavatar.com/kg/ontohplc/">
-    <dc:date rdf:datatype="http://www.w3.org/2001/XMLSchema#string">28 April 2023</dc:date>
+    <dc:date rdf:datatype="http://www.w3.org/2001/XMLSchema#string">04 May 2023</dc:date>
     <rdfs:comment rdf:datatype="http://www.w3.org/2001/XMLSchema#string">OntoHPLC is an ontology developed for expressing a high performance liquid chromatography.</rdfs:comment>
     <owl:versionInfo rdf:datatype="http://www.w3.org/2001/XMLSchema#string">1.8</owl:versionInfo>
     <gitCommitHash rdf:datatype="http://www.w3.org/2001/XMLSchema#string">c0599beca8df55873a1ab061dee64e52c510c6a0</gitCommitHash>
   </owl:Ontology>
   <!-- 
     ///////////////////////////////////////////////////////////////////////////////////////
     //
```

### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots/resources/ontology/OntoLab.owl` & `chemistry_and_robots-1.6.2/chemistry_and_robots/resources/ontology/OntoLab.owl`

 * *Files 1% similar despite different names*

#### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots/resources/ontology/OntoLab.owl` & `chemistry_and_robots-1.6.2/chemistry_and_robots/resources/ontology/OntoLab.owl`

```diff
@@ -1,13 +1,13 @@
 <?xml version="1.0" encoding="utf-8"?>
 <rdf:RDF xmlns="https://www.theworldavatar.com/kg/ontolab/" xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#" xmlns:owl="http://www.w3.org/2002/07/owl#" xmlns:xml="http://www.w3.org/XML/1998/namespace" xmlns:xsd="http://www.w3.org/2001/XMLSchema#" xmlns:rdfs="http://www.w3.org/2000/01/rdf-schema#" xmlns:ontolab="https://www.theworldavatar.com/kg/ontolab/" xmlns:dc="http://purl.org/dc/elements/1.1/" xml:base="https://www.theworldavatar.com/kg/ontolab/">
   <owl:Ontology rdf:about="https://www.theworldavatar.com/kg/ontolab/">
-    <dc:date rdf:datatype="http://www.w3.org/2001/XMLSchema#string">28 April 2023</dc:date>
+    <dc:date rdf:datatype="http://www.w3.org/2001/XMLSchema#string">04 May 2023</dc:date>
     <rdfs:comment rdf:datatype="http://www.w3.org/2001/XMLSchema#string">OntoLab is an ontology developed for expressing facilities in a research lab.</rdfs:comment>
-    <owl:versionInfo rdf:datatype="http://www.w3.org/2001/XMLSchema#string">1.9</owl:versionInfo>
+    <owl:versionInfo rdf:datatype="http://www.w3.org/2001/XMLSchema#string">1.10</owl:versionInfo>
     <gitCommitHash rdf:datatype="http://www.w3.org/2001/XMLSchema#string">c0599beca8df55873a1ab061dee64e52c510c6a0</gitCommitHash>
   </owl:Ontology>
   <!-- 
     ///////////////////////////////////////////////////////////////////////////////////////
     //
     // Object Properties
     //
@@ -178,22 +178,27 @@
   <owl:Class rdf:about="http://www.theworldavatar.com/ontology/ontoagent/MSM.owl#Service"/>
   <!-- http://www.theworldavatar.com/ontology/ontocape/chemical_process_system/CPS_behavior/behavior.owl#MaterialAmount -->
   <owl:Class rdf:about="http://www.theworldavatar.com/ontology/ontocape/chemical_process_system/CPS_behavior/behavior.owl#MaterialAmount"/>
   <!-- https://saref.etsi.org/core/Device -->
   <owl:Class rdf:about="https://saref.etsi.org/core/Device"/>
   <!-- https://saref.etsi.org/core/State -->
   <owl:Class rdf:about="https://saref.etsi.org/core/State"/>
+  <!-- https://w3id.org/bot#Element -->
+  <owl:Class rdf:about="https://w3id.org/bot#Element"/>
+  <!-- https://www.theworldavatar.com/kg/ontobim/Facility -->
+  <owl:Class rdf:about="https://www.theworldavatar.com/kg/ontobim/Facility"/>
   <!-- https://www.theworldavatar.com/kg/ontolab/ChemicalAmount -->
   <owl:Class rdf:about="https://www.theworldavatar.com/kg/ontolab/ChemicalAmount">
     <rdfs:subClassOf rdf:resource="http://www.theworldavatar.com/ontology/ontocape/chemical_process_system/CPS_behavior/behavior.owl#MaterialAmount"/>
     <rdfs:comment rdf:datatype="http://www.w3.org/2001/XMLSchema#string">The concrete realisation of chemical amount in the physical world, e.g., a liquid holdup in a vessel.</rdfs:comment>
     <rdfs:isDefinedBy rdf:datatype="http://www.w3.org/2001/XMLSchema#string">https://www.theworldavatar.com/kg/ontolab/</rdfs:isDefinedBy>
   </owl:Class>
   <!-- https://www.theworldavatar.com/kg/ontolab/ChemicalContainer -->
   <owl:Class rdf:about="https://www.theworldavatar.com/kg/ontolab/ChemicalContainer">
+    <rdfs:subClassOf rdf:resource="https://w3id.org/bot#Element"/>
     <rdfs:subClassOf>
       <owl:Restriction>
         <owl:onProperty rdf:resource="https://www.theworldavatar.com/kg/ontolab/hasFillLevel"/>
         <owl:qualifiedCardinality rdf:datatype="http://www.w3.org/2001/XMLSchema#nonNegativeInteger">1</owl:qualifiedCardinality>
         <owl:onClass rdf:resource="http://www.ontology-of-units-of-measure.org/resource/om-2/Volume"/>
       </owl:Restriction>
     </rdfs:subClassOf>
@@ -309,14 +314,15 @@
       </owl:Restriction>
     </rdfs:subClassOf>
     <rdfs:comment rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Equipment used for laboratory experiments. [https://www.wikidata.org/wiki/Q834028]</rdfs:comment>
     <rdfs:isDefinedBy rdf:datatype="http://www.w3.org/2001/XMLSchema#string">https://www.theworldavatar.com/kg/ontolab/</rdfs:isDefinedBy>
   </owl:Class>
   <!-- https://www.theworldavatar.com/kg/ontolab/Laboratory -->
   <owl:Class rdf:about="https://www.theworldavatar.com/kg/ontolab/Laboratory">
+    <rdfs:subClassOf rdf:resource="https://www.theworldavatar.com/kg/ontobim/Facility"/>
     <rdfs:comment rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Facility that provides controlled conditions in which scientific or technological research, experiments, and measurement may be performed. [https://www.wikidata.org/wiki/Q483242]</rdfs:comment>
     <rdfs:isDefinedBy rdf:datatype="http://www.w3.org/2001/XMLSchema#string">https://www.theworldavatar.com/kg/ontolab/</rdfs:isDefinedBy>
   </owl:Class>
   <!-- https://www.theworldavatar.com/kg/ontolab/LithiumBattery -->
   <owl:Class rdf:about="https://www.theworldavatar.com/kg/ontolab/LithiumBattery">
     <rdfs:subClassOf rdf:resource="https://www.theworldavatar.com/kg/ontolab/PowerSupply"/>
     <rdfs:comment rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Power supply through a lithium battery.</rdfs:comment>
```

### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots/resources/ontology/OntoReaction.owl` & `chemistry_and_robots-1.6.2/chemistry_and_robots/resources/ontology/OntoReaction.owl`

 * *Files 0% similar despite different names*

#### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots/resources/ontology/OntoReaction.owl` & `chemistry_and_robots-1.6.2/chemistry_and_robots/resources/ontology/OntoReaction.owl`

```diff
@@ -1,11 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
 <rdf:RDF xmlns="https://www.theworldavatar.com/kg/ontoreaction/" xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#" xmlns:owl="http://www.w3.org/2002/07/owl#" xmlns:xml="http://www.w3.org/XML/1998/namespace" xmlns:xsd="http://www.w3.org/2001/XMLSchema#" xmlns:ontoreaction="https://www.theworldavatar.com/kg/ontoreaction/" xmlns:rdfs="http://www.w3.org/2000/01/rdf-schema#" xmlns:dc="http://purl.org/dc/elements/1.1/" xml:base="https://www.theworldavatar.com/kg/ontoreaction/">
   <owl:Ontology rdf:about="https://www.theworldavatar.com/kg/ontoreaction/">
-    <dc:date rdf:datatype="http://www.w3.org/2001/XMLSchema#string">28 April 2023</dc:date>
+    <dc:date rdf:datatype="http://www.w3.org/2001/XMLSchema#string">04 May 2023</dc:date>
     <rdfs:comment rdf:datatype="http://www.w3.org/2001/XMLSchema#string">An ontology developed for describing reaction experiment.</rdfs:comment>
     <owl:versionInfo rdf:datatype="http://www.w3.org/2001/XMLSchema#string">1.10</owl:versionInfo>
     <gitCommitHash rdf:datatype="http://www.w3.org/2001/XMLSchema#string">c0599beca8df55873a1ab061dee64e52c510c6a0</gitCommitHash>
   </owl:Ontology>
   <!-- 
     ///////////////////////////////////////////////////////////////////////////////////////
     //
```

### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots/resources/ontology/OntoVapourtec.owl` & `chemistry_and_robots-1.6.2/chemistry_and_robots/resources/ontology/OntoVapourtec.owl`

 * *Files 0% similar despite different names*

#### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots/resources/ontology/OntoVapourtec.owl` & `chemistry_and_robots-1.6.2/chemistry_and_robots/resources/ontology/OntoVapourtec.owl`

```diff
@@ -1,11 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
 <rdf:RDF xmlns="https://www.theworldavatar.com/kg/ontovapourtec/" xmlns:ontovapourtec="https://www.theworldavatar.com/kg/ontovapourtec/" xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#" xmlns:owl="http://www.w3.org/2002/07/owl#" xmlns:xml="http://www.w3.org/XML/1998/namespace" xmlns:xsd="http://www.w3.org/2001/XMLSchema#" xmlns:rdfs="http://www.w3.org/2000/01/rdf-schema#" xmlns:dc="http://purl.org/dc/elements/1.1/" xml:base="https://www.theworldavatar.com/kg/ontovapourtec/">
   <owl:Ontology rdf:about="https://www.theworldavatar.com/kg/ontovapourtec/">
-    <dc:date rdf:datatype="http://www.w3.org/2001/XMLSchema#string">28 April 2023</dc:date>
+    <dc:date rdf:datatype="http://www.w3.org/2001/XMLSchema#string">04 May 2023</dc:date>
     <rdfs:comment rdf:datatype="http://www.w3.org/2001/XMLSchema#string">OntoVapourtec is an ontology developed for expressing a Vapourtec experiment module.</rdfs:comment>
     <owl:versionInfo rdf:datatype="http://www.w3.org/2001/XMLSchema#string">1.9</owl:versionInfo>
     <gitCommitHash rdf:datatype="http://www.w3.org/2001/XMLSchema#string">c0599beca8df55873a1ab061dee64e52c510c6a0</gitCommitHash>
   </owl:Ontology>
   <!-- 
     ///////////////////////////////////////////////////////////////////////////////////////
     //
```

### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots/resources/sample_data/doe.ttl` & `chemistry_and_robots-1.6.2/chemistry_and_robots/resources/sample_data/doe.ttl`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots/resources/sample_data/doe_no_prior_data.ttl` & `chemistry_and_robots-1.6.2/chemistry_and_robots/resources/sample_data/doe_no_prior_data.ttl`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots/resources/sample_data/doe_template.ttl` & `chemistry_and_robots-1.6.2/chemistry_and_robots/resources/sample_data/doe_template.ttl`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots/resources/sample_data/dummy_lab.ttl` & `chemistry_and_robots-1.6.2/chemistry_and_robots/resources/sample_data/dummy_lab.ttl`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots/resources/sample_data/dummy_post_proc.ttl` & `chemistry_and_robots-1.6.2/chemistry_and_robots/resources/sample_data/dummy_post_proc.ttl`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots/resources/sample_data/new_exp_data.ttl` & `chemistry_and_robots-1.6.2/chemistry_and_robots/resources/sample_data/new_exp_data.ttl`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots/resources/sample_data/new_exp_data_out_of_range.ttl` & `chemistry_and_robots-1.6.2/chemistry_and_robots/resources/sample_data/new_exp_data_out_of_range.ttl`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots/resources/sample_data/raw_hplc_report_xls.xls` & `chemistry_and_robots-1.6.2/chemistry_and_robots/resources/sample_data/raw_hplc_report_xls.xls`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots/resources/sample_data/raw_hplc_report_xls_incomplete.xls` & `chemistry_and_robots-1.6.2/chemistry_and_robots/resources/sample_data/raw_hplc_report_xls_incomplete.xls`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots/resources/sample_data/raw_hplc_report_xls_no_product.xls` & `chemistry_and_robots-1.6.2/chemistry_and_robots/resources/sample_data/raw_hplc_report_xls_no_product.xls`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots/resources/sample_data/raw_hplc_report_xls_unidentified_peaks.xls` & `chemistry_and_robots-1.6.2/chemistry_and_robots/resources/sample_data/raw_hplc_report_xls_unidentified_peaks.xls`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots/resources/sample_data/rxn_data.ttl` & `chemistry_and_robots-1.6.2/chemistry_and_robots/resources/sample_data/rxn_data.ttl`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots/resources/sample_data/rxn_queue_test.ttl` & `chemistry_and_robots-1.6.2/chemistry_and_robots/resources/sample_data/rxn_queue_test.ttl`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots/tests/conftest.py` & `chemistry_and_robots-1.6.2/chemistry_and_robots/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots/tests/test_base_ontology.py` & `chemistry_and_robots-1.6.2/chemistry_and_robots/tests/test_base_ontology.py`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots/tests/test_dict_and_list.py` & `chemistry_and_robots-1.6.2/chemistry_and_robots/tests/test_dict_and_list.py`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots/tests/test_example_triples.py` & `chemistry_and_robots-1.6.2/chemistry_and_robots/tests/test_example_triples.py`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots/tests/test_hash_eq.py` & `chemistry_and_robots-1.6.2/chemistry_and_robots/tests/test_hash_eq.py`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots/tests/test_hplc.py` & `chemistry_and_robots-1.6.2/chemistry_and_robots/tests/test_hplc.py`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots/tests/test_ontodoe.py` & `chemistry_and_robots-1.6.2/chemistry_and_robots/tests/test_ontodoe.py`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots/tests/test_single_phase.py` & `chemistry_and_robots-1.6.2/chemistry_and_robots/tests/test_single_phase.py`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots/tests/test_sparql_client.py` & `chemistry_and_robots-1.6.2/chemistry_and_robots/tests/test_sparql_client.py`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots.egg-info/PKG-INFO` & `chemistry_and_robots-1.6.2/chemistry_and_robots.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chemistry-and-robots
-Version: 1.6.1
+Version: 1.6.2
 Summary: chemistryandrobots contains dataclasses and sparql queries for concepts related to chemistry_and_robots as part of The World Avatar project.
 Home-page: https://github.com/cambridge-cares/TheWorldAvatar/tree/main/Agents/utils/chemistry_and_robots
 Author: Jiaru Bai
 Author-email: jb2197@cam.ac.uk
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `chemistry_and_robots-1.6.1/chemistry_and_robots.egg-info/SOURCES.txt` & `chemistry_and_robots-1.6.2/chemistry_and_robots.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.6.1/setup.py` & `chemistry_and_robots-1.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name='chemistry_and_robots',
-    version='1.6.1',
+    version='1.6.2',
     author='Jiaru Bai',
     author_email='jb2197@cam.ac.uk',
     license='MIT',
     python_requires='>=3.8',
     description="chemistryandrobots contains dataclasses and sparql queries for concepts related to chemistry_and_robots as part of The World Avatar project.",
     url="https://github.com/cambridge-cares/TheWorldAvatar/tree/main/Agents/utils/chemistry_and_robots",
     long_description=open('README.md').read(),
```

