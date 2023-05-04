# Comparing `tmp/ner4opt-1.0.0.tar.gz` & `tmp/ner4opt-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ner4opt-1.0.0.tar", last modified: Wed May  3 19:03:30 2023, max compression
+gzip compressed data, was "ner4opt-1.0.1.tar", last modified: Thu May  4 00:16:29 2023, max compression
```

## Comparing `ner4opt-1.0.0.tar` & `ner4opt-1.0.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 a715824  (337160431) staff       (20)        0 2023-05-03 19:03:30.905713 ner4opt-1.0.0/
--rw-r--r--   0 a715824  (337160431) staff       (20)      175 2023-05-03 11:54:59.000000 ner4opt-1.0.0/CHANGELOG.md
--rw-r--r--   0 a715824  (337160431) staff       (20)     1056 2023-05-03 12:26:33.000000 ner4opt-1.0.0/LICENSE
--rw-r--r--   0 a715824  (337160431) staff       (20)      139 2023-05-03 13:55:11.000000 ner4opt-1.0.0/MANIFEST.in
--rw-r--r--   0 a715824  (337160431) staff       (20)     3277 2023-05-03 19:03:30.905413 ner4opt-1.0.0/PKG-INFO
--rw-r--r--   0 a715824  (337160431) staff       (20)     2289 2023-05-03 11:54:59.000000 ner4opt-1.0.0/README.md
-drwxr-xr-x   0 a715824  (337160431) staff       (20)        0 2023-05-03 19:03:30.850368 ner4opt-1.0.0/models/
--rw-r--r--   0 a715824  (337160431) staff       (20)     6148 2023-05-03 16:50:34.000000 ner4opt-1.0.0/models/.DS_Store
--rw-r--r--   0 a715824  (337160431) staff       (20)     1469 2023-05-03 11:54:59.000000 ner4opt-1.0.0/models/README.md
--rw-r--r--   0 a715824  (337160431) staff       (20)  6424278 2023-05-03 11:54:59.000000 ner4opt-1.0.0/models/hybrid.pkl
--rw-r--r--   0 a715824  (337160431) staff       (20)  7962982 2023-05-03 11:54:59.000000 ner4opt-1.0.0/models/lexical.pkl
--rw-r--r--   0 a715824  (337160431) staff       (20)  8152086 2023-05-03 11:54:59.000000 ner4opt-1.0.0/models/lexical_plus.pkl
-drwxr-xr-x   0 a715824  (337160431) staff       (20)        0 2023-05-03 19:03:30.875866 ner4opt-1.0.0/models/training/
--rw-r--r--   0 a715824  (337160431) staff       (20)     1314 2023-05-03 18:50:43.000000 ner4opt-1.0.0/models/training/README.md
-drwxr-xr-x   0 a715824  (337160431) staff       (20)        0 2023-05-03 19:03:30.876895 ner4opt-1.0.0/models/training/data/
--rw-r--r--   0 a715824  (337160431) staff       (20)     1191 2023-05-03 11:54:59.000000 ner4opt-1.0.0/models/training/data/README.md
-drwxr-xr-x   0 a715824  (337160431) staff       (20)        0 2023-05-03 19:03:30.877785 ner4opt-1.0.0/models/training/logs/
--rw-r--r--   0 a715824  (337160431) staff       (20)    20771 2023-05-03 11:54:59.000000 ner4opt-1.0.0/models/training/logs/hybrid_log.txt
-drwxr-xr-x   0 a715824  (337160431) staff       (20)        0 2023-05-03 19:03:30.881995 ner4opt-1.0.0/models/training/nl4opt_utils/
--rw-r--r--   0 a715824  (337160431) staff       (20)      338 2023-05-03 11:54:59.000000 ner4opt-1.0.0/models/training/nl4opt_utils/README.md
--rw-r--r--   0 a715824  (337160431) staff       (20)        0 2023-05-03 11:54:59.000000 ner4opt-1.0.0/models/training/nl4opt_utils/__init__.py
--rw-r--r--   0 a715824  (337160431) staff       (20)     4665 2023-05-03 11:54:59.000000 ner4opt-1.0.0/models/training/nl4opt_utils/metric.py
--rw-r--r--   0 a715824  (337160431) staff       (20)     3841 2023-05-03 11:54:59.000000 ner4opt-1.0.0/models/training/nl4opt_utils/reader.py
--rw-r--r--   0 a715824  (337160431) staff       (20)     3002 2023-05-03 11:54:59.000000 ner4opt-1.0.0/models/training/nl4opt_utils/reader_utils.py
--rw-r--r--   0 a715824  (337160431) staff       (20)     8571 2023-05-03 11:54:59.000000 ner4opt-1.0.0/models/training/nl4opt_utils/utils.py
-drwxr-xr-x   0 a715824  (337160431) staff       (20)        0 2023-05-03 19:03:30.884438 ner4opt-1.0.0/models/training/notebooks/
--rw-r--r--   0 a715824  (337160431) staff       (20)      541 2023-05-03 11:54:59.000000 ner4opt-1.0.0/models/training/notebooks/README.md
--rw-r--r--   0 a715824  (337160431) staff       (20)     8812 2023-05-03 11:54:59.000000 ner4opt-1.0.0/models/training/notebooks/data_augmentation.ipynb
--rw-r--r--   0 a715824  (337160431) staff       (20)     2334 2023-05-03 11:54:59.000000 ner4opt-1.0.0/models/training/notebooks/entity_gazetteers.ipynb
--rw-r--r--   0 a715824  (337160431) staff       (20)    10760 2023-05-03 11:54:59.000000 ner4opt-1.0.0/models/training/train_and_evaluate_hybrid_model.py
-drwxr-xr-x   0 a715824  (337160431) staff       (20)        0 2023-05-03 19:03:30.891034 ner4opt-1.0.0/ner4opt/
--rw-r--r--   0 a715824  (337160431) staff       (20)      298 2023-05-03 18:18:31.000000 ner4opt-1.0.0/ner4opt/__init__.py
--rw-r--r--   0 a715824  (337160431) staff       (20)       45 2023-05-03 11:54:59.000000 ner4opt-1.0.0/ner4opt/_version.py
--rw-r--r--   0 a715824  (337160431) staff       (20)     4874 2023-05-03 17:57:26.000000 ner4opt-1.0.0/ner4opt/constants.py
--rw-r--r--   0 a715824  (337160431) staff       (20)    22255 2023-05-03 11:54:59.000000 ner4opt-1.0.0/ner4opt/featurizer.py
--rw-r--r--   0 a715824  (337160431) staff       (20)     8807 2023-05-03 11:54:59.000000 ner4opt-1.0.0/ner4opt/ner4opt.py
--rw-r--r--   0 a715824  (337160431) staff       (20)       87 2023-05-03 11:54:59.000000 ner4opt-1.0.0/ner4opt/setup_nltk.py
--rw-r--r--   0 a715824  (337160431) staff       (20)      896 2023-05-03 18:21:46.000000 ner4opt-1.0.0/ner4opt/setup_spacy.py
--rw-r--r--   0 a715824  (337160431) staff       (20)    10012 2023-05-03 11:54:59.000000 ner4opt-1.0.0/ner4opt/utils.py
-drwxr-xr-x   0 a715824  (337160431) staff       (20)        0 2023-05-03 19:03:30.896012 ner4opt-1.0.0/ner4opt.egg-info/
--rw-r--r--   0 a715824  (337160431) staff       (20)     3277 2023-05-03 19:03:30.000000 ner4opt-1.0.0/ner4opt.egg-info/PKG-INFO
--rw-r--r--   0 a715824  (337160431) staff       (20)     1281 2023-05-03 19:03:30.000000 ner4opt-1.0.0/ner4opt.egg-info/SOURCES.txt
--rw-r--r--   0 a715824  (337160431) staff       (20)        1 2023-05-03 19:03:30.000000 ner4opt-1.0.0/ner4opt.egg-info/dependency_links.txt
--rw-r--r--   0 a715824  (337160431) staff       (20)      134 2023-05-03 19:03:30.000000 ner4opt-1.0.0/ner4opt.egg-info/requires.txt
--rw-r--r--   0 a715824  (337160431) staff       (20)       21 2023-05-03 19:03:30.000000 ner4opt-1.0.0/ner4opt.egg-info/top_level.txt
--rw-r--r--   0 a715824  (337160431) staff       (20)      134 2023-05-03 16:38:48.000000 ner4opt-1.0.0/requirements.txt
--rw-r--r--   0 a715824  (337160431) staff       (20)       38 2023-05-03 19:03:30.905814 ner4opt-1.0.0/setup.cfg
--rw-r--r--   0 a715824  (337160431) staff       (20)      886 2023-05-03 16:39:19.000000 ner4opt-1.0.0/setup.py
-drwxr-xr-x   0 a715824  (337160431) staff       (20)        0 2023-05-03 19:03:30.901177 ner4opt-1.0.0/tests/
--rw-r--r--   0 a715824  (337160431) staff       (20)     6148 2023-05-03 18:25:50.000000 ner4opt-1.0.0/tests/.DS_Store
--rw-r--r--   0 a715824  (337160431) staff       (20)        0 2023-05-03 11:54:59.000000 ner4opt-1.0.0/tests/__init__.py
-drwxr-xr-x   0 a715824  (337160431) staff       (20)        0 2023-05-03 19:03:30.904800 ner4opt-1.0.0/tests/fixtures/
--rw-r--r--   0 a715824  (337160431) staff       (20)      593 2023-05-03 11:54:59.000000 ner4opt-1.0.0/tests/fixtures/example_problem.txt
--rw-r--r--   0 a715824  (337160431) staff       (20)     1652 2023-05-03 11:54:59.000000 ner4opt-1.0.0/tests/fixtures/hybrid_result.json
--rw-r--r--   0 a715824  (337160431) staff       (20)     1654 2023-05-03 11:54:59.000000 ner4opt-1.0.0/tests/fixtures/lexical_plus_result.json
--rw-r--r--   0 a715824  (337160431) staff       (20)     1643 2023-05-03 11:54:59.000000 ner4opt-1.0.0/tests/fixtures/lexical_result.json
--rw-r--r--   0 a715824  (337160431) staff       (20)     1652 2023-05-03 11:54:59.000000 ner4opt-1.0.0/tests/fixtures/semantic_result.json
--rw-r--r--   0 a715824  (337160431) staff       (20)     2427 2023-05-03 11:54:59.000000 ner4opt-1.0.0/tests/test_features.py
--rw-r--r--   0 a715824  (337160431) staff       (20)     3169 2023-05-03 11:54:59.000000 ner4opt-1.0.0/tests/test_ner4opt.py
--rw-r--r--   0 a715824  (337160431) staff       (20)     3104 2023-05-03 11:54:59.000000 ner4opt-1.0.0/tests/test_utils.py
+drwxr-xr-x   0 a715824  (337160431) staff       (20)        0 2023-05-04 00:16:29.084807 ner4opt-1.0.1/
+-rw-r--r--   0 a715824  (337160431) staff       (20)      175 2023-05-03 11:54:59.000000 ner4opt-1.0.1/CHANGELOG.md
+-rw-r--r--   0 a715824  (337160431) staff       (20)     1056 2023-05-03 12:26:33.000000 ner4opt-1.0.1/LICENSE
+-rw-r--r--   0 a715824  (337160431) staff       (20)      139 2023-05-03 13:55:11.000000 ner4opt-1.0.1/MANIFEST.in
+-rw-r--r--   0 a715824  (337160431) staff       (20)     3277 2023-05-04 00:16:29.084503 ner4opt-1.0.1/PKG-INFO
+-rw-r--r--   0 a715824  (337160431) staff       (20)     2289 2023-05-03 11:54:59.000000 ner4opt-1.0.1/README.md
+drwxr-xr-x   0 a715824  (337160431) staff       (20)        0 2023-05-04 00:16:29.035171 ner4opt-1.0.1/models/
+-rw-r--r--   0 a715824  (337160431) staff       (20)     6148 2023-05-03 16:50:34.000000 ner4opt-1.0.1/models/.DS_Store
+-rw-r--r--   0 a715824  (337160431) staff       (20)     1469 2023-05-03 11:54:59.000000 ner4opt-1.0.1/models/README.md
+-rw-r--r--   0 a715824  (337160431) staff       (20)  6424278 2023-05-03 11:54:59.000000 ner4opt-1.0.1/models/hybrid.pkl
+-rw-r--r--   0 a715824  (337160431) staff       (20)  7962982 2023-05-03 11:54:59.000000 ner4opt-1.0.1/models/lexical.pkl
+-rw-r--r--   0 a715824  (337160431) staff       (20)  8152086 2023-05-03 11:54:59.000000 ner4opt-1.0.1/models/lexical_plus.pkl
+drwxr-xr-x   0 a715824  (337160431) staff       (20)        0 2023-05-04 00:16:29.060713 ner4opt-1.0.1/models/training/
+-rw-r--r--   0 a715824  (337160431) staff       (20)     1314 2023-05-03 18:50:43.000000 ner4opt-1.0.1/models/training/README.md
+drwxr-xr-x   0 a715824  (337160431) staff       (20)        0 2023-05-04 00:16:29.061594 ner4opt-1.0.1/models/training/data/
+-rw-r--r--   0 a715824  (337160431) staff       (20)     1191 2023-05-03 11:54:59.000000 ner4opt-1.0.1/models/training/data/README.md
+drwxr-xr-x   0 a715824  (337160431) staff       (20)        0 2023-05-04 00:16:29.062434 ner4opt-1.0.1/models/training/logs/
+-rw-r--r--   0 a715824  (337160431) staff       (20)    20771 2023-05-03 11:54:59.000000 ner4opt-1.0.1/models/training/logs/hybrid_log.txt
+drwxr-xr-x   0 a715824  (337160431) staff       (20)        0 2023-05-04 00:16:29.066917 ner4opt-1.0.1/models/training/nl4opt_utils/
+-rw-r--r--   0 a715824  (337160431) staff       (20)      338 2023-05-03 11:54:59.000000 ner4opt-1.0.1/models/training/nl4opt_utils/README.md
+-rw-r--r--   0 a715824  (337160431) staff       (20)        0 2023-05-03 11:54:59.000000 ner4opt-1.0.1/models/training/nl4opt_utils/__init__.py
+-rw-r--r--   0 a715824  (337160431) staff       (20)     4665 2023-05-03 11:54:59.000000 ner4opt-1.0.1/models/training/nl4opt_utils/metric.py
+-rw-r--r--   0 a715824  (337160431) staff       (20)     3841 2023-05-03 11:54:59.000000 ner4opt-1.0.1/models/training/nl4opt_utils/reader.py
+-rw-r--r--   0 a715824  (337160431) staff       (20)     3002 2023-05-03 11:54:59.000000 ner4opt-1.0.1/models/training/nl4opt_utils/reader_utils.py
+-rw-r--r--   0 a715824  (337160431) staff       (20)     8571 2023-05-03 11:54:59.000000 ner4opt-1.0.1/models/training/nl4opt_utils/utils.py
+drwxr-xr-x   0 a715824  (337160431) staff       (20)        0 2023-05-04 00:16:29.068898 ner4opt-1.0.1/models/training/notebooks/
+-rw-r--r--   0 a715824  (337160431) staff       (20)      541 2023-05-03 11:54:59.000000 ner4opt-1.0.1/models/training/notebooks/README.md
+-rw-r--r--   0 a715824  (337160431) staff       (20)     8812 2023-05-03 11:54:59.000000 ner4opt-1.0.1/models/training/notebooks/data_augmentation.ipynb
+-rw-r--r--   0 a715824  (337160431) staff       (20)     2334 2023-05-03 11:54:59.000000 ner4opt-1.0.1/models/training/notebooks/entity_gazetteers.ipynb
+-rw-r--r--   0 a715824  (337160431) staff       (20)    10760 2023-05-03 11:54:59.000000 ner4opt-1.0.1/models/training/train_and_evaluate_hybrid_model.py
+drwxr-xr-x   0 a715824  (337160431) staff       (20)        0 2023-05-04 00:16:29.075133 ner4opt-1.0.1/ner4opt/
+-rw-r--r--   0 a715824  (337160431) staff       (20)      298 2023-05-03 18:18:31.000000 ner4opt-1.0.1/ner4opt/__init__.py
+-rw-r--r--   0 a715824  (337160431) staff       (20)       45 2023-05-04 00:09:23.000000 ner4opt-1.0.1/ner4opt/_version.py
+-rw-r--r--   0 a715824  (337160431) staff       (20)     4874 2023-05-03 17:57:26.000000 ner4opt-1.0.1/ner4opt/constants.py
+-rw-r--r--   0 a715824  (337160431) staff       (20)    22255 2023-05-03 11:54:59.000000 ner4opt-1.0.1/ner4opt/featurizer.py
+-rw-r--r--   0 a715824  (337160431) staff       (20)     9352 2023-05-04 00:03:24.000000 ner4opt-1.0.1/ner4opt/ner4opt.py
+-rw-r--r--   0 a715824  (337160431) staff       (20)       87 2023-05-03 11:54:59.000000 ner4opt-1.0.1/ner4opt/setup_nltk.py
+-rw-r--r--   0 a715824  (337160431) staff       (20)      896 2023-05-03 18:21:46.000000 ner4opt-1.0.1/ner4opt/setup_spacy.py
+-rw-r--r--   0 a715824  (337160431) staff       (20)    10104 2023-05-03 23:33:02.000000 ner4opt-1.0.1/ner4opt/utils.py
+drwxr-xr-x   0 a715824  (337160431) staff       (20)        0 2023-05-04 00:16:29.078308 ner4opt-1.0.1/ner4opt.egg-info/
+-rw-r--r--   0 a715824  (337160431) staff       (20)     3277 2023-05-04 00:16:28.000000 ner4opt-1.0.1/ner4opt.egg-info/PKG-INFO
+-rw-r--r--   0 a715824  (337160431) staff       (20)     1281 2023-05-04 00:16:28.000000 ner4opt-1.0.1/ner4opt.egg-info/SOURCES.txt
+-rw-r--r--   0 a715824  (337160431) staff       (20)        1 2023-05-04 00:16:28.000000 ner4opt-1.0.1/ner4opt.egg-info/dependency_links.txt
+-rw-r--r--   0 a715824  (337160431) staff       (20)      134 2023-05-04 00:16:28.000000 ner4opt-1.0.1/ner4opt.egg-info/requires.txt
+-rw-r--r--   0 a715824  (337160431) staff       (20)       21 2023-05-04 00:16:28.000000 ner4opt-1.0.1/ner4opt.egg-info/top_level.txt
+-rw-r--r--   0 a715824  (337160431) staff       (20)      134 2023-05-03 16:38:48.000000 ner4opt-1.0.1/requirements.txt
+-rw-r--r--   0 a715824  (337160431) staff       (20)       38 2023-05-04 00:16:29.084915 ner4opt-1.0.1/setup.cfg
+-rw-r--r--   0 a715824  (337160431) staff       (20)      886 2023-05-03 16:39:19.000000 ner4opt-1.0.1/setup.py
+drwxr-xr-x   0 a715824  (337160431) staff       (20)        0 2023-05-04 00:16:29.080997 ner4opt-1.0.1/tests/
+-rw-r--r--   0 a715824  (337160431) staff       (20)     6148 2023-05-04 00:14:47.000000 ner4opt-1.0.1/tests/.DS_Store
+-rw-r--r--   0 a715824  (337160431) staff       (20)        0 2023-05-03 11:54:59.000000 ner4opt-1.0.1/tests/__init__.py
+drwxr-xr-x   0 a715824  (337160431) staff       (20)        0 2023-05-04 00:16:29.083954 ner4opt-1.0.1/tests/fixtures/
+-rw-r--r--   0 a715824  (337160431) staff       (20)      593 2023-05-03 11:54:59.000000 ner4opt-1.0.1/tests/fixtures/example_problem.txt
+-rw-r--r--   0 a715824  (337160431) staff       (20)     1652 2023-05-03 11:54:59.000000 ner4opt-1.0.1/tests/fixtures/hybrid_result.json
+-rw-r--r--   0 a715824  (337160431) staff       (20)     1654 2023-05-03 11:54:59.000000 ner4opt-1.0.1/tests/fixtures/lexical_plus_result.json
+-rw-r--r--   0 a715824  (337160431) staff       (20)     1643 2023-05-03 11:54:59.000000 ner4opt-1.0.1/tests/fixtures/lexical_result.json
+-rw-r--r--   0 a715824  (337160431) staff       (20)     1652 2023-05-03 11:54:59.000000 ner4opt-1.0.1/tests/fixtures/semantic_result.json
+-rw-r--r--   0 a715824  (337160431) staff       (20)     2427 2023-05-03 11:54:59.000000 ner4opt-1.0.1/tests/test_features.py
+-rw-r--r--   0 a715824  (337160431) staff       (20)     3169 2023-05-03 11:54:59.000000 ner4opt-1.0.1/tests/test_ner4opt.py
+-rw-r--r--   0 a715824  (337160431) staff       (20)     3104 2023-05-03 11:54:59.000000 ner4opt-1.0.1/tests/test_utils.py
```

### Comparing `ner4opt-1.0.0/LICENSE` & `ner4opt-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ner4opt-1.0.0/PKG-INFO` & `ner4opt-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ner4opt
-Version: 1.0.0
+Version: 1.0.1
 Summary: NER4OPT Library
 Home-page: https://github.com/skadio/ner4opt
 License: UNKNOWN
 Project-URL: Source, https://github.com/skadio/ner4opt
 Description: # Named Entity Recognition for Optimization (Ner4Opt) Library
         
         Given an optimization problem in natural language, the Ner4Opt library extracts **six named entities**:
```

### Comparing `ner4opt-1.0.0/README.md` & `ner4opt-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ner4opt-1.0.0/models/.DS_Store` & `ner4opt-1.0.1/models/.DS_Store`

 * *Files identical despite different names*

### Comparing `ner4opt-1.0.0/models/README.md` & `ner4opt-1.0.1/models/README.md`

 * *Files identical despite different names*

### Comparing `ner4opt-1.0.0/models/hybrid.pkl` & `ner4opt-1.0.1/models/hybrid.pkl`

 * *Files identical despite different names*

### Comparing `ner4opt-1.0.0/models/lexical.pkl` & `ner4opt-1.0.1/models/lexical.pkl`

 * *Files identical despite different names*

### Comparing `ner4opt-1.0.0/models/lexical_plus.pkl` & `ner4opt-1.0.1/models/lexical_plus.pkl`

 * *Files identical despite different names*

### Comparing `ner4opt-1.0.0/models/training/README.md` & `ner4opt-1.0.1/models/training/README.md`

 * *Files identical despite different names*

### Comparing `ner4opt-1.0.0/models/training/data/README.md` & `ner4opt-1.0.1/models/training/data/README.md`

 * *Files identical despite different names*

### Comparing `ner4opt-1.0.0/models/training/logs/hybrid_log.txt` & `ner4opt-1.0.1/models/training/logs/hybrid_log.txt`

 * *Files identical despite different names*

### Comparing `ner4opt-1.0.0/models/training/nl4opt_utils/metric.py` & `ner4opt-1.0.1/models/training/nl4opt_utils/metric.py`

 * *Files identical despite different names*

### Comparing `ner4opt-1.0.0/models/training/nl4opt_utils/reader.py` & `ner4opt-1.0.1/models/training/nl4opt_utils/reader.py`

 * *Files identical despite different names*

### Comparing `ner4opt-1.0.0/models/training/nl4opt_utils/reader_utils.py` & `ner4opt-1.0.1/models/training/nl4opt_utils/reader_utils.py`

 * *Files identical despite different names*

### Comparing `ner4opt-1.0.0/models/training/nl4opt_utils/utils.py` & `ner4opt-1.0.1/models/training/nl4opt_utils/utils.py`

 * *Files identical despite different names*

### Comparing `ner4opt-1.0.0/models/training/notebooks/README.md` & `ner4opt-1.0.1/models/training/notebooks/README.md`

 * *Files identical despite different names*

### Comparing `ner4opt-1.0.0/models/training/notebooks/data_augmentation.ipynb` & `ner4opt-1.0.1/models/training/notebooks/data_augmentation.ipynb`

 * *Files identical despite different names*

### Comparing `ner4opt-1.0.0/models/training/notebooks/entity_gazetteers.ipynb` & `ner4opt-1.0.1/models/training/notebooks/entity_gazetteers.ipynb`

 * *Files identical despite different names*

### Comparing `ner4opt-1.0.0/models/training/train_and_evaluate_hybrid_model.py` & `ner4opt-1.0.1/models/training/train_and_evaluate_hybrid_model.py`

 * *Files identical despite different names*

### Comparing `ner4opt-1.0.0/ner4opt/constants.py` & `ner4opt-1.0.1/ner4opt/constants.py`

 * *Files identical despite different names*

### Comparing `ner4opt-1.0.0/ner4opt/featurizer.py` & `ner4opt-1.0.1/ner4opt/featurizer.py`

 * *Files identical despite different names*

### Comparing `ner4opt-1.0.0/ner4opt/ner4opt.py` & `ner4opt-1.0.1/ner4opt/ner4opt.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,16 @@
     Attributes
     -------
     model (str) : Specifies the model to use for extracting the entities.
                   Options include `lexical`, `lexical_plus`, `semantic` and `hybrid`
                   Default is `hybrid`
     use_gpu (bool) : Specifies the model to use gpu while calculating transformer based features.
                      Default is False
+    use_multiprocessing (bool) : Specifies the model to use multiprocessing while calculating transformer based features.
+                                 Default is False
 
     Methods
     -------
     get_entities()
 
     Attributes
     -------
@@ -91,15 +93,15 @@
 
     Help
     ----
     >>> from ner4opt import Ner4Opt
     >>> Ner4Opt.__doc__
     """
 
-    def __init__(self, model: str = Constants.HYBRID, use_gpu: bool = False):
+    def __init__(self, model: str = Constants.HYBRID, use_gpu: bool = False, use_multiprocessing: bool = False):
         """Init Ner4Opt class."""
 
         _root_directory = pathlib.Path(__file__).parent.parent
 
         self._lexical_crf_model_path = os.path.join(_root_directory, Constants.MODELS_DIRECTORY,
                                                     Constants.LEXICAL_CRF_MODEL_NAME)
         self._lexical_plus_crf_model_path = os.path.join(_root_directory, Constants.MODELS_DIRECTORY,
@@ -116,18 +118,22 @@
             self._crf_model = joblib.load(self._lexical_crf_model_path)
 
         elif self._model == Constants.LEXICAL_PLUS:
             self._crf_model = joblib.load(self._lexical_plus_crf_model_path)
 
         elif self._model == Constants.SEMANTIC:
             # Model to extract semantic features
-            self._semantic_feature_extractor = load_torch_model(Constants.SEMANTIC_MODEL_ROBERTA_V1, use_gpu=use_gpu)
+            self._semantic_feature_extractor = load_torch_model(Constants.SEMANTIC_MODEL_ROBERTA_V1,
+                                                                use_gpu=use_gpu,
+                                                                use_multiprocessing=use_multiprocessing)
 
         elif self._model == Constants.HYBRID:
-            self._semantic_feature_extractor = load_torch_model(Constants.SEMANTIC_MODEL_ROBERTA_V2, use_gpu=use_gpu)
+            self._semantic_feature_extractor = load_torch_model(Constants.SEMANTIC_MODEL_ROBERTA_V2,
+                                                                use_gpu=use_gpu,
+                                                                use_multiprocessing=use_multiprocessing)
             # Our best model combines both semantic and lexical features
             self._crf_model = joblib.load(self._hybrid_crf_model_path)
 
         else:
             raise ValueError(
                 "Invalid Model {} passed. Model name should be one of the following lexical, lexical_plus, semantic or hybrid"
                 .format(self._model))
```

### Comparing `ner4opt-1.0.0/ner4opt/setup_spacy.py` & `ner4opt-1.0.1/ner4opt/setup_spacy.py`

 * *Files identical despite different names*

### Comparing `ner4opt-1.0.0/ner4opt/utils.py` & `ner4opt-1.0.1/ner4opt/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         for token_idx in range(chunk.start, chunk.end):
 
             connected_chunks[token_idx] = [chunk.start, chunk.end]
 
     return connected_chunks
 
 
-def load_torch_model(model_name: str, use_gpu: bool = False):
+def load_torch_model(model_name: str, use_gpu: bool = False, use_multiprocessing: bool = False):
     """Load Torch model."""
 
     model_args = NERArgs()
     model_args.use_early_stopping = True
     model_args.early_stopping_delta = 0.01
     model_args.early_stopping_metric = "eval_loss"
     model_args.early_stopping_metric_minimize = False
@@ -130,14 +130,15 @@
     model_args.weight_decay = 0.01
     model_args.max_seq_length = 512
     model_args.learning_rate = 4e-5
     model_args.train_batch_size = 1
     model_args.eval_batch_size = 1
     model_args.manual_seed = 123456789
     model_args.use_cuda = use_gpu
+    model_args.use_multiprocessing = use_multiprocessing
     model_args.force_download = True
 
     model = NERModel("roberta", model_name, labels=Constants.LABELS, use_cuda=use_gpu, args=model_args)
 
     return model
```

### Comparing `ner4opt-1.0.0/ner4opt.egg-info/PKG-INFO` & `ner4opt-1.0.1/ner4opt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ner4opt
-Version: 1.0.0
+Version: 1.0.1
 Summary: NER4OPT Library
 Home-page: https://github.com/skadio/ner4opt
 License: UNKNOWN
 Project-URL: Source, https://github.com/skadio/ner4opt
 Description: # Named Entity Recognition for Optimization (Ner4Opt) Library
         
         Given an optimization problem in natural language, the Ner4Opt library extracts **six named entities**:
```

### Comparing `ner4opt-1.0.0/ner4opt.egg-info/SOURCES.txt` & `ner4opt-1.0.1/ner4opt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ner4opt-1.0.0/setup.py` & `ner4opt-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `ner4opt-1.0.0/tests/.DS_Store` & `ner4opt-1.0.1/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `ner4opt-1.0.0/tests/fixtures/example_problem.txt` & `ner4opt-1.0.1/tests/fixtures/example_problem.txt`

 * *Files identical despite different names*

### Comparing `ner4opt-1.0.0/tests/fixtures/hybrid_result.json` & `ner4opt-1.0.1/tests/fixtures/hybrid_result.json`

 * *Files identical despite different names*

### Comparing `ner4opt-1.0.0/tests/fixtures/lexical_plus_result.json` & `ner4opt-1.0.1/tests/fixtures/lexical_plus_result.json`

 * *Files identical despite different names*

### Comparing `ner4opt-1.0.0/tests/fixtures/lexical_result.json` & `ner4opt-1.0.1/tests/fixtures/lexical_result.json`

 * *Files identical despite different names*

### Comparing `ner4opt-1.0.0/tests/fixtures/semantic_result.json` & `ner4opt-1.0.1/tests/fixtures/semantic_result.json`

 * *Files identical despite different names*

### Comparing `ner4opt-1.0.0/tests/test_features.py` & `ner4opt-1.0.1/tests/test_features.py`

 * *Files identical despite different names*

### Comparing `ner4opt-1.0.0/tests/test_ner4opt.py` & `ner4opt-1.0.1/tests/test_ner4opt.py`

 * *Files identical despite different names*

### Comparing `ner4opt-1.0.0/tests/test_utils.py` & `ner4opt-1.0.1/tests/test_utils.py`

 * *Files identical despite different names*

