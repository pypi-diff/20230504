# Comparing `tmp/CoLT5-attention-0.5.1.tar.gz` & `tmp/CoLT5-attention-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CoLT5-attention-0.5.1.tar", last modified: Thu May  4 01:43:15 2023, max compression
+gzip compressed data, was "CoLT5-attention-0.5.2.tar", last modified: Thu May  4 01:44:00 2023, max compression
```

## Comparing `CoLT5-attention-0.5.1.tar` & `CoLT5-attention-0.5.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:43:15.519557 CoLT5-attention-0.5.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:43:15.519557 CoLT5-attention-0.5.1/CoLT5_attention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-04 01:43:15.000000 CoLT5-attention-0.5.1/CoLT5_attention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-04 01:43:15.000000 CoLT5-attention-0.5.1/CoLT5_attention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 01:43:15.000000 CoLT5-attention-0.5.1/CoLT5_attention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-04 01:43:15.000000 CoLT5-attention-0.5.1/CoLT5_attention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-04 01:43:15.000000 CoLT5-attention-0.5.1/CoLT5_attention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-04 01:43:03.000000 CoLT5-attention-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-04 01:43:15.519557 CoLT5-attention-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9745 2023-05-04 01:43:03.000000 CoLT5-attention-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:43:15.519557 CoLT5-attention-0.5.1/colt5_attention/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-04 01:43:03.000000 CoLT5-attention-0.5.1/colt5_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-04 01:43:03.000000 CoLT5-attention-0.5.1/colt5_attention/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-04 01:43:03.000000 CoLT5-attention-0.5.1/colt5_attention/coor_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-04 01:43:03.000000 CoLT5-attention-0.5.1/colt5_attention/sinkhorn.py
--rw-r--r--   0 runner    (1001) docker     (123)    34323 2023-05-04 01:43:03.000000 CoLT5-attention-0.5.1/colt5_attention/transformer_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-05-04 01:43:03.000000 CoLT5-attention-0.5.1/colt5_attention/triton_coor_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 01:43:15.519557 CoLT5-attention-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-04 01:43:03.000000 CoLT5-attention-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:44:00.600881 CoLT5-attention-0.5.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:44:00.600881 CoLT5-attention-0.5.2/CoLT5_attention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-04 01:44:00.000000 CoLT5-attention-0.5.2/CoLT5_attention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-04 01:44:00.000000 CoLT5-attention-0.5.2/CoLT5_attention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 01:44:00.000000 CoLT5-attention-0.5.2/CoLT5_attention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-04 01:44:00.000000 CoLT5-attention-0.5.2/CoLT5_attention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-04 01:44:00.000000 CoLT5-attention-0.5.2/CoLT5_attention.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-04 01:43:49.000000 CoLT5-attention-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-04 01:44:00.600881 CoLT5-attention-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9745 2023-05-04 01:43:49.000000 CoLT5-attention-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:44:00.600881 CoLT5-attention-0.5.2/colt5_attention/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-04 01:43:49.000000 CoLT5-attention-0.5.2/colt5_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-04 01:43:49.000000 CoLT5-attention-0.5.2/colt5_attention/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-04 01:43:49.000000 CoLT5-attention-0.5.2/colt5_attention/coor_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-04 01:43:49.000000 CoLT5-attention-0.5.2/colt5_attention/sinkhorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34323 2023-05-04 01:43:49.000000 CoLT5-attention-0.5.2/colt5_attention/transformer_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-05-04 01:43:49.000000 CoLT5-attention-0.5.2/colt5_attention/triton_coor_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 01:44:00.600881 CoLT5-attention-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-04 01:43:49.000000 CoLT5-attention-0.5.2/setup.py
```

### Comparing `CoLT5-attention-0.5.1/CoLT5_attention.egg-info/PKG-INFO` & `CoLT5-attention-0.5.2/CoLT5_attention.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.5.1
+Version: 0.5.2
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.5.1/LICENSE` & `CoLT5-attention-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.5.1/PKG-INFO` & `CoLT5-attention-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.5.1
+Version: 0.5.2
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.5.1/README.md` & `CoLT5-attention-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.5.1/colt5_attention/attend.py` & `CoLT5-attention-0.5.2/colt5_attention/attend.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.5.1/colt5_attention/coor_descent.py` & `CoLT5-attention-0.5.2/colt5_attention/coor_descent.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.5.1/colt5_attention/sinkhorn.py` & `CoLT5-attention-0.5.2/colt5_attention/sinkhorn.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.5.1/colt5_attention/transformer_block.py` & `CoLT5-attention-0.5.2/colt5_attention/transformer_block.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.5.1/colt5_attention/triton_coor_descent.py` & `CoLT5-attention-0.5.2/colt5_attention/triton_coor_descent.py`

 * *Files 0% similar despite different names*

```diff
@@ -364,15 +364,15 @@
 
         n_rows, n_cols = grad_probs.shape
 
         BLOCK_SIZE = triton.next_power_of_2(n_cols)
         num_warps = calc_num_warps(BLOCK_SIZE)
 
         dx = torch.empty_like(grad_probs)
-        dk = torch.zeros_like(k)
+        dk = torch.empty_like(k)
 
         mask_int = mask.int()
 
         coor_descent_kernel_backward[(n_rows,)](
             dx,
             dk,
             x,
```

### Comparing `CoLT5-attention-0.5.1/setup.py` & `CoLT5-attention-0.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'CoLT5-attention',
   packages = find_packages(),
-  version = '0.5.1',
+  version = '0.5.2',
   license='MIT',
   description = 'Conditionally Routed Attention',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/CoLT5-attention',
   keywords = [
```

