# Comparing `tmp/EA_framework-2.2.2.tar.gz` & `tmp/EA_framework-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EA_framework-2.2.2.tar", last modified: Thu May  4 18:57:05 2023, max compression
+gzip compressed data, was "EA_framework-2.2.3.tar", last modified: Thu May  4 19:00:01 2023, max compression
```

## Comparing `EA_framework-2.2.2.tar` & `EA_framework-2.2.3.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxrwxr-x   0 dimi      (1000) dimi      (1000)        0 2023-05-04 18:57:05.598565 EA_framework-2.2.2/
--rw-rw-r--   0 dimi      (1000) dimi      (1000)     1060 2022-05-16 23:00:20.000000 EA_framework-2.2.2/LICENSE
--rw-rw-r--   0 dimi      (1000) dimi      (1000)     1684 2023-05-04 18:57:05.598565 EA_framework-2.2.2/PKG-INFO
--rw-rw-r--   0 dimi      (1000) dimi      (1000)     6948 2023-05-04 18:52:34.000000 EA_framework-2.2.2/README.md
--rw-rw-r--   0 dimi      (1000) dimi      (1000)      689 2023-05-04 18:56:53.000000 EA_framework-2.2.2/pyproject.toml
--rw-rw-r--   0 dimi      (1000) dimi      (1000)       38 2023-05-04 18:57:05.598565 EA_framework-2.2.2/setup.cfg
-drwxrwxr-x   0 dimi      (1000) dimi      (1000)        0 2023-05-04 18:57:05.594565 EA_framework-2.2.2/src/
-drwxrwxr-x   0 dimi      (1000) dimi      (1000)        0 2023-05-04 18:57:05.594565 EA_framework-2.2.2/src/EA_framework.egg-info/
--rw-rw-r--   0 dimi      (1000) dimi      (1000)     1684 2023-05-04 18:57:05.000000 EA_framework-2.2.2/src/EA_framework.egg-info/PKG-INFO
--rw-rw-r--   0 dimi      (1000) dimi      (1000)     1014 2023-05-04 18:57:05.000000 EA_framework-2.2.2/src/EA_framework.egg-info/SOURCES.txt
--rw-rw-r--   0 dimi      (1000) dimi      (1000)        1 2023-05-04 18:57:05.000000 EA_framework-2.2.2/src/EA_framework.egg-info/dependency_links.txt
--rw-rw-r--   0 dimi      (1000) dimi      (1000)      114 2023-05-04 18:57:05.000000 EA_framework-2.2.2/src/EA_framework.egg-info/top_level.txt
-drwxrwxr-x   0 dimi      (1000) dimi      (1000)        0 2023-05-04 18:57:05.594565 EA_framework-2.2.2/src/EA_multiproc/
--rw-rw-r--   0 dimi      (1000) dimi      (1000)     7202 2022-11-22 12:22:09.000000 EA_framework-2.2.2/src/EA_multiproc/EA_mixed.py
--rw-rw-r--   0 dimi      (1000) dimi      (1000)     6248 2022-12-10 10:56:47.000000 EA_framework-2.2.2/src/EA_multiproc/EA_pool.py
--rw-rw-r--   0 dimi      (1000) dimi      (1000)     1668 2022-12-10 10:47:46.000000 EA_framework-2.2.2/src/EA_multiproc/Eval_multiproc.py
--rw-rw-r--   0 dimi      (1000) dimi      (1000)     2513 2022-12-10 10:19:55.000000 EA_framework-2.2.2/src/EA_multiproc/Mut_multiproc.py
--rw-rw-r--   0 dimi      (1000) dimi      (1000)     3390 2022-12-10 10:14:53.000000 EA_framework-2.2.2/src/EA_multiproc/Pop_multiproc.py
--rw-rw-r--   0 dimi      (1000) dimi      (1000)     1421 2022-11-22 11:12:24.000000 EA_framework-2.2.2/src/EA_multiproc/Rec_multiproc.py
--rw-rw-r--   0 dimi      (1000) dimi      (1000)      968 2022-12-10 10:22:30.000000 EA_framework-2.2.2/src/EA_multiproc/Sel_multiproc.py
--rw-rw-r--   0 dimi      (1000) dimi      (1000)        0 2022-11-21 21:59:04.000000 EA_framework-2.2.2/src/EA_multiproc/__init__.py
-drwxrwxr-x   0 dimi      (1000) dimi      (1000)        0 2023-05-04 18:57:05.598565 EA_framework-2.2.2/src/EA_sequential/
--rw-rw-r--   0 dimi      (1000) dimi      (1000)      112 2022-11-21 22:11:30.000000 EA_framework-2.2.2/src/EA_sequential/Crossover.py
--rw-rw-r--   0 dimi      (1000) dimi      (1000)     5342 2022-12-10 10:51:03.000000 EA_framework-2.2.2/src/EA_sequential/EA.py
--rw-rw-r--   0 dimi      (1000) dimi      (1000)     2999 2022-11-21 22:11:30.000000 EA_framework-2.2.2/src/EA_sequential/Evaluation.py
--rw-rw-r--   0 dimi      (1000) dimi      (1000)     2337 2022-11-22 11:00:14.000000 EA_framework-2.2.2/src/EA_sequential/Mutation.py
--rw-rw-r--   0 dimi      (1000) dimi      (1000)     2612 2022-11-21 21:40:17.000000 EA_framework-2.2.2/src/EA_sequential/Population.py
--rw-rw-r--   0 dimi      (1000) dimi      (1000)     4372 2022-11-21 22:11:30.000000 EA_framework-2.2.2/src/EA_sequential/Recombination.py
--rw-rw-r--   0 dimi      (1000) dimi      (1000)     1723 2022-11-21 22:11:30.000000 EA_framework-2.2.2/src/EA_sequential/Selection.py
--rw-rw-r--   0 dimi      (1000) dimi      (1000)        0 2022-05-12 11:14:40.000000 EA_framework-2.2.2/src/EA_sequential/__init__.py
-drwxrwxr-x   0 dimi      (1000) dimi      (1000)        0 2023-05-04 18:57:05.598565 EA_framework-2.2.2/src/EA_torch/
--rw-rw-r--   0 dimi      (1000) dimi      (1000)     2130 2022-10-21 20:14:36.000000 EA_framework-2.2.2/src/EA_torch/EA_torch.py
--rw-rw-r--   0 dimi      (1000) dimi      (1000)     1846 2022-10-21 16:37:06.000000 EA_framework-2.2.2/src/EA_torch/Evaluation_torch.py
--rw-rw-r--   0 dimi      (1000) dimi      (1000)     1297 2022-10-21 20:20:13.000000 EA_framework-2.2.2/src/EA_torch/Mutation_torch.py
--rw-rw-r--   0 dimi      (1000) dimi      (1000)     2526 2022-10-21 16:48:08.000000 EA_framework-2.2.2/src/EA_torch/Population_torch.py
--rw-rw-r--   0 dimi      (1000) dimi      (1000)     3387 2022-11-21 22:11:30.000000 EA_framework-2.2.2/src/EA_torch/Recombination_torch.py
--rw-rw-r--   0 dimi      (1000) dimi      (1000)     1714 2022-10-21 16:12:18.000000 EA_framework-2.2.2/src/EA_torch/Selection_torch.py
--rw-rw-r--   0 dimi      (1000) dimi      (1000)        0 2022-10-21 16:52:04.000000 EA_framework-2.2.2/src/EA_torch/__init__.py
--rw-rw-r--   0 dimi      (1000) dimi      (1000)      525 2022-11-21 22:11:30.000000 EA_framework-2.2.2/src/discrete_test.py
--rw-rw-r--   0 dimi      (1000) dimi      (1000)     7119 2022-11-21 22:11:30.000000 EA_framework-2.2.2/src/main_ea.py
--rw-rw-r--   0 dimi      (1000) dimi      (1000)     2186 2022-11-22 13:08:58.000000 EA_framework-2.2.2/src/mixed_test.py
--rw-rw-r--   0 dimi      (1000) dimi      (1000)     2661 2022-12-10 10:58:58.000000 EA_framework-2.2.2/src/multiprocess_comparison.py
--rw-rw-r--   0 dimi      (1000) dimi      (1000)     2492 2022-11-21 22:11:30.000000 EA_framework-2.2.2/src/pytorch_test.py
+drwxrwxr-x   0 dimi      (1000) dimi      (1000)        0 2023-05-04 19:00:01.925317 EA_framework-2.2.3/
+-rw-rw-r--   0 dimi      (1000) dimi      (1000)     1060 2022-05-16 23:00:20.000000 EA_framework-2.2.3/LICENSE
+-rw-rw-r--   0 dimi      (1000) dimi      (1000)       17 2023-05-04 18:59:24.000000 EA_framework-2.2.3/MANIFEST.in
+-rw-rw-r--   0 dimi      (1000) dimi      (1000)     8674 2023-05-04 19:00:01.925317 EA_framework-2.2.3/PKG-INFO
+-rw-rw-r--   0 dimi      (1000) dimi      (1000)     6948 2023-05-04 18:52:34.000000 EA_framework-2.2.3/README.md
+-rw-rw-r--   0 dimi      (1000) dimi      (1000)      710 2023-05-04 18:59:49.000000 EA_framework-2.2.3/pyproject.toml
+-rw-rw-r--   0 dimi      (1000) dimi      (1000)       38 2023-05-04 19:00:01.925317 EA_framework-2.2.3/setup.cfg
+drwxrwxr-x   0 dimi      (1000) dimi      (1000)        0 2023-05-04 19:00:01.921317 EA_framework-2.2.3/src/
+drwxrwxr-x   0 dimi      (1000) dimi      (1000)        0 2023-05-04 19:00:01.925317 EA_framework-2.2.3/src/EA_framework.egg-info/
+-rw-rw-r--   0 dimi      (1000) dimi      (1000)     8674 2023-05-04 19:00:01.000000 EA_framework-2.2.3/src/EA_framework.egg-info/PKG-INFO
+-rw-rw-r--   0 dimi      (1000) dimi      (1000)     1026 2023-05-04 19:00:01.000000 EA_framework-2.2.3/src/EA_framework.egg-info/SOURCES.txt
+-rw-rw-r--   0 dimi      (1000) dimi      (1000)        1 2023-05-04 19:00:01.000000 EA_framework-2.2.3/src/EA_framework.egg-info/dependency_links.txt
+-rw-rw-r--   0 dimi      (1000) dimi      (1000)      114 2023-05-04 19:00:01.000000 EA_framework-2.2.3/src/EA_framework.egg-info/top_level.txt
+drwxrwxr-x   0 dimi      (1000) dimi      (1000)        0 2023-05-04 19:00:01.925317 EA_framework-2.2.3/src/EA_multiproc/
+-rw-rw-r--   0 dimi      (1000) dimi      (1000)     7202 2022-11-22 12:22:09.000000 EA_framework-2.2.3/src/EA_multiproc/EA_mixed.py
+-rw-rw-r--   0 dimi      (1000) dimi      (1000)     6248 2022-12-10 10:56:47.000000 EA_framework-2.2.3/src/EA_multiproc/EA_pool.py
+-rw-rw-r--   0 dimi      (1000) dimi      (1000)     1668 2022-12-10 10:47:46.000000 EA_framework-2.2.3/src/EA_multiproc/Eval_multiproc.py
+-rw-rw-r--   0 dimi      (1000) dimi      (1000)     2513 2022-12-10 10:19:55.000000 EA_framework-2.2.3/src/EA_multiproc/Mut_multiproc.py
+-rw-rw-r--   0 dimi      (1000) dimi      (1000)     3390 2022-12-10 10:14:53.000000 EA_framework-2.2.3/src/EA_multiproc/Pop_multiproc.py
+-rw-rw-r--   0 dimi      (1000) dimi      (1000)     1421 2022-11-22 11:12:24.000000 EA_framework-2.2.3/src/EA_multiproc/Rec_multiproc.py
+-rw-rw-r--   0 dimi      (1000) dimi      (1000)      968 2022-12-10 10:22:30.000000 EA_framework-2.2.3/src/EA_multiproc/Sel_multiproc.py
+-rw-rw-r--   0 dimi      (1000) dimi      (1000)        0 2022-11-21 21:59:04.000000 EA_framework-2.2.3/src/EA_multiproc/__init__.py
+drwxrwxr-x   0 dimi      (1000) dimi      (1000)        0 2023-05-04 19:00:01.925317 EA_framework-2.2.3/src/EA_sequential/
+-rw-rw-r--   0 dimi      (1000) dimi      (1000)      112 2022-11-21 22:11:30.000000 EA_framework-2.2.3/src/EA_sequential/Crossover.py
+-rw-rw-r--   0 dimi      (1000) dimi      (1000)     5342 2022-12-10 10:51:03.000000 EA_framework-2.2.3/src/EA_sequential/EA.py
+-rw-rw-r--   0 dimi      (1000) dimi      (1000)     2999 2022-11-21 22:11:30.000000 EA_framework-2.2.3/src/EA_sequential/Evaluation.py
+-rw-rw-r--   0 dimi      (1000) dimi      (1000)     2337 2022-11-22 11:00:14.000000 EA_framework-2.2.3/src/EA_sequential/Mutation.py
+-rw-rw-r--   0 dimi      (1000) dimi      (1000)     2612 2022-11-21 21:40:17.000000 EA_framework-2.2.3/src/EA_sequential/Population.py
+-rw-rw-r--   0 dimi      (1000) dimi      (1000)     4372 2022-11-21 22:11:30.000000 EA_framework-2.2.3/src/EA_sequential/Recombination.py
+-rw-rw-r--   0 dimi      (1000) dimi      (1000)     1723 2022-11-21 22:11:30.000000 EA_framework-2.2.3/src/EA_sequential/Selection.py
+-rw-rw-r--   0 dimi      (1000) dimi      (1000)        0 2022-05-12 11:14:40.000000 EA_framework-2.2.3/src/EA_sequential/__init__.py
+drwxrwxr-x   0 dimi      (1000) dimi      (1000)        0 2023-05-04 19:00:01.925317 EA_framework-2.2.3/src/EA_torch/
+-rw-rw-r--   0 dimi      (1000) dimi      (1000)     2130 2022-10-21 20:14:36.000000 EA_framework-2.2.3/src/EA_torch/EA_torch.py
+-rw-rw-r--   0 dimi      (1000) dimi      (1000)     1846 2022-10-21 16:37:06.000000 EA_framework-2.2.3/src/EA_torch/Evaluation_torch.py
+-rw-rw-r--   0 dimi      (1000) dimi      (1000)     1297 2022-10-21 20:20:13.000000 EA_framework-2.2.3/src/EA_torch/Mutation_torch.py
+-rw-rw-r--   0 dimi      (1000) dimi      (1000)     2526 2022-10-21 16:48:08.000000 EA_framework-2.2.3/src/EA_torch/Population_torch.py
+-rw-rw-r--   0 dimi      (1000) dimi      (1000)     3387 2022-11-21 22:11:30.000000 EA_framework-2.2.3/src/EA_torch/Recombination_torch.py
+-rw-rw-r--   0 dimi      (1000) dimi      (1000)     1714 2022-10-21 16:12:18.000000 EA_framework-2.2.3/src/EA_torch/Selection_torch.py
+-rw-rw-r--   0 dimi      (1000) dimi      (1000)        0 2022-10-21 16:52:04.000000 EA_framework-2.2.3/src/EA_torch/__init__.py
+-rw-rw-r--   0 dimi      (1000) dimi      (1000)      525 2022-11-21 22:11:30.000000 EA_framework-2.2.3/src/discrete_test.py
+-rw-rw-r--   0 dimi      (1000) dimi      (1000)     7119 2022-11-21 22:11:30.000000 EA_framework-2.2.3/src/main_ea.py
+-rw-rw-r--   0 dimi      (1000) dimi      (1000)     2186 2022-11-22 13:08:58.000000 EA_framework-2.2.3/src/mixed_test.py
+-rw-rw-r--   0 dimi      (1000) dimi      (1000)     2661 2022-12-10 10:58:58.000000 EA_framework-2.2.3/src/multiprocess_comparison.py
+-rw-rw-r--   0 dimi      (1000) dimi      (1000)     2492 2022-11-21 22:11:30.000000 EA_framework-2.2.3/src/pytorch_test.py
```

### Comparing `EA_framework-2.2.2/LICENSE` & `EA_framework-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `EA_framework-2.2.2/README.md` & `EA_framework-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `EA_framework-2.2.2/pyproject.toml` & `EA_framework-2.2.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "EA_framework"
-version = "2.2.2"
+version = "2.2.3"
 authors = [
   { name="Dimitrios Ieronymakis", email="dimitris.ieronymakis@gmail.com" },
 ]
 description = "A framework for applying evolutionary algorithms to generic optimization problems."
+readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `EA_framework-2.2.2/src/EA_framework.egg-info/SOURCES.txt` & `EA_framework-2.2.3/src/EA_framework.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE
+MANIFEST.in
 README.md
 pyproject.toml
 src/discrete_test.py
 src/main_ea.py
 src/mixed_test.py
 src/multiprocess_comparison.py
 src/pytorch_test.py
```

### Comparing `EA_framework-2.2.2/src/EA_multiproc/EA_mixed.py` & `EA_framework-2.2.3/src/EA_multiproc/EA_mixed.py`

 * *Files identical despite different names*

### Comparing `EA_framework-2.2.2/src/EA_multiproc/EA_pool.py` & `EA_framework-2.2.3/src/EA_multiproc/EA_pool.py`

 * *Files identical despite different names*

### Comparing `EA_framework-2.2.2/src/EA_multiproc/Eval_multiproc.py` & `EA_framework-2.2.3/src/EA_multiproc/Eval_multiproc.py`

 * *Files identical despite different names*

### Comparing `EA_framework-2.2.2/src/EA_multiproc/Mut_multiproc.py` & `EA_framework-2.2.3/src/EA_multiproc/Mut_multiproc.py`

 * *Files identical despite different names*

### Comparing `EA_framework-2.2.2/src/EA_multiproc/Pop_multiproc.py` & `EA_framework-2.2.3/src/EA_multiproc/Pop_multiproc.py`

 * *Files identical despite different names*

### Comparing `EA_framework-2.2.2/src/EA_multiproc/Rec_multiproc.py` & `EA_framework-2.2.3/src/EA_multiproc/Rec_multiproc.py`

 * *Files identical despite different names*

### Comparing `EA_framework-2.2.2/src/EA_multiproc/Sel_multiproc.py` & `EA_framework-2.2.3/src/EA_multiproc/Sel_multiproc.py`

 * *Files identical despite different names*

### Comparing `EA_framework-2.2.2/src/EA_sequential/EA.py` & `EA_framework-2.2.3/src/EA_sequential/EA.py`

 * *Files identical despite different names*

### Comparing `EA_framework-2.2.2/src/EA_sequential/Evaluation.py` & `EA_framework-2.2.3/src/EA_sequential/Evaluation.py`

 * *Files identical despite different names*

### Comparing `EA_framework-2.2.2/src/EA_sequential/Mutation.py` & `EA_framework-2.2.3/src/EA_sequential/Mutation.py`

 * *Files identical despite different names*

### Comparing `EA_framework-2.2.2/src/EA_sequential/Population.py` & `EA_framework-2.2.3/src/EA_sequential/Population.py`

 * *Files identical despite different names*

### Comparing `EA_framework-2.2.2/src/EA_sequential/Recombination.py` & `EA_framework-2.2.3/src/EA_sequential/Recombination.py`

 * *Files identical despite different names*

### Comparing `EA_framework-2.2.2/src/EA_sequential/Selection.py` & `EA_framework-2.2.3/src/EA_sequential/Selection.py`

 * *Files identical despite different names*

### Comparing `EA_framework-2.2.2/src/EA_torch/EA_torch.py` & `EA_framework-2.2.3/src/EA_torch/EA_torch.py`

 * *Files identical despite different names*

### Comparing `EA_framework-2.2.2/src/EA_torch/Evaluation_torch.py` & `EA_framework-2.2.3/src/EA_torch/Evaluation_torch.py`

 * *Files identical despite different names*

### Comparing `EA_framework-2.2.2/src/EA_torch/Mutation_torch.py` & `EA_framework-2.2.3/src/EA_torch/Mutation_torch.py`

 * *Files identical despite different names*

### Comparing `EA_framework-2.2.2/src/EA_torch/Population_torch.py` & `EA_framework-2.2.3/src/EA_torch/Population_torch.py`

 * *Files identical despite different names*

### Comparing `EA_framework-2.2.2/src/EA_torch/Recombination_torch.py` & `EA_framework-2.2.3/src/EA_torch/Recombination_torch.py`

 * *Files identical despite different names*

### Comparing `EA_framework-2.2.2/src/EA_torch/Selection_torch.py` & `EA_framework-2.2.3/src/EA_torch/Selection_torch.py`

 * *Files identical despite different names*

### Comparing `EA_framework-2.2.2/src/discrete_test.py` & `EA_framework-2.2.3/src/discrete_test.py`

 * *Files identical despite different names*

### Comparing `EA_framework-2.2.2/src/main_ea.py` & `EA_framework-2.2.3/src/main_ea.py`

 * *Files identical despite different names*

### Comparing `EA_framework-2.2.2/src/mixed_test.py` & `EA_framework-2.2.3/src/mixed_test.py`

 * *Files identical despite different names*

### Comparing `EA_framework-2.2.2/src/multiprocess_comparison.py` & `EA_framework-2.2.3/src/multiprocess_comparison.py`

 * *Files identical despite different names*

### Comparing `EA_framework-2.2.2/src/pytorch_test.py` & `EA_framework-2.2.3/src/pytorch_test.py`

 * *Files identical despite different names*

