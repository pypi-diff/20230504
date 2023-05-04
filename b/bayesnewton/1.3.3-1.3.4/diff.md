# Comparing `tmp/bayesnewton-1.3.3.tar.gz` & `tmp/bayesnewton-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bayesnewton-1.3.3.tar", last modified: Tue May  2 20:28:16 2023, max compression
+gzip compressed data, was "bayesnewton-1.3.4.tar", last modified: Thu May  4 15:34:21 2023, max compression
```

## Comparing `bayesnewton-1.3.3.tar` & `bayesnewton-1.3.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 wwilkinson   (501) staff       (20)        0 2023-05-02 20:28:16.177220 bayesnewton-1.3.3/
--rw-r--r--   0 wwilkinson   (501) staff       (20)    11357 2021-11-10 15:34:42.000000 bayesnewton-1.3.3/LICENSE
--rw-r--r--   0 wwilkinson   (501) staff       (20)      170 2023-05-02 20:28:16.177089 bayesnewton-1.3.3/PKG-INFO
--rw-r--r--   0 wwilkinson   (501) staff       (20)     8385 2022-11-29 10:26:07.000000 bayesnewton-1.3.3/README.md
-drwxr-xr-x   0 wwilkinson   (501) staff       (20)        0 2023-05-02 20:28:16.174918 bayesnewton-1.3.3/bayesnewton/
--rw-r--r--   0 wwilkinson   (501) staff       (20)      211 2021-11-10 15:34:42.000000 bayesnewton-1.3.3/bayesnewton/__init__.py
--rw-r--r--   0 wwilkinson   (501) staff       (20)    59304 2023-02-17 12:56:03.000000 bayesnewton-1.3.3/bayesnewton/basemodels.py
--rw-r--r--   0 wwilkinson   (501) staff       (20)    19067 2022-11-07 13:19:06.000000 bayesnewton-1.3.3/bayesnewton/cubature.py
--rw-r--r--   0 wwilkinson   (501) staff       (20)    43632 2023-02-17 12:56:03.000000 bayesnewton-1.3.3/bayesnewton/inference.py
--rw-r--r--   0 wwilkinson   (501) staff       (20)    74634 2023-02-17 12:56:03.000000 bayesnewton-1.3.3/bayesnewton/kernels.py
--rw-r--r--   0 wwilkinson   (501) staff       (20)   106886 2023-03-06 14:54:44.000000 bayesnewton-1.3.3/bayesnewton/likelihoods.py
--rw-r--r--   0 wwilkinson   (501) staff       (20)    39746 2022-11-18 14:50:56.000000 bayesnewton-1.3.3/bayesnewton/models.py
--rw-r--r--   0 wwilkinson   (501) staff       (20)    43162 2023-05-02 20:15:25.000000 bayesnewton-1.3.3/bayesnewton/ops.py
--rw-r--r--   0 wwilkinson   (501) staff       (20)    25027 2023-02-17 12:56:03.000000 bayesnewton-1.3.3/bayesnewton/utils.py
-drwxr-xr-x   0 wwilkinson   (501) staff       (20)        0 2023-05-02 20:28:16.175405 bayesnewton-1.3.3/bayesnewton.egg-info/
--rw-r--r--   0 wwilkinson   (501) staff       (20)      170 2023-05-02 20:28:16.000000 bayesnewton-1.3.3/bayesnewton.egg-info/PKG-INFO
--rw-r--r--   0 wwilkinson   (501) staff       (20)      668 2023-05-02 20:28:16.000000 bayesnewton-1.3.3/bayesnewton.egg-info/SOURCES.txt
--rw-r--r--   0 wwilkinson   (501) staff       (20)        1 2023-05-02 20:28:16.000000 bayesnewton-1.3.3/bayesnewton.egg-info/dependency_links.txt
--rw-r--r--   0 wwilkinson   (501) staff       (20)       12 2023-05-02 20:28:16.000000 bayesnewton-1.3.3/bayesnewton.egg-info/top_level.txt
--rw-r--r--   0 wwilkinson   (501) staff       (20)       38 2023-05-02 20:28:16.177256 bayesnewton-1.3.3/setup.cfg
--rw-r--r--   0 wwilkinson   (501) staff       (20)      261 2023-05-02 20:15:46.000000 bayesnewton-1.3.3/setup.py
-drwxr-xr-x   0 wwilkinson   (501) staff       (20)        0 2023-05-02 20:28:16.176910 bayesnewton-1.3.3/tests/
--rw-r--r--   0 wwilkinson   (501) staff       (20)     4347 2021-11-10 15:34:42.000000 bayesnewton-1.3.3/tests/test_gp_vs_markovgp_class.py
--rw-r--r--   0 wwilkinson   (501) staff       (20)     5121 2021-11-10 15:34:42.000000 bayesnewton-1.3.3/tests/test_gp_vs_markovgp_reg.py
--rw-r--r--   0 wwilkinson   (501) staff       (20)     7116 2021-11-10 15:34:42.000000 bayesnewton-1.3.3/tests/test_gp_vs_markovgp_spacetime.py
--rw-r--r--   0 wwilkinson   (501) staff       (20)    12690 2021-11-10 15:34:42.000000 bayesnewton-1.3.3/tests/test_sparsemarkov.py
--rw-r--r--   0 wwilkinson   (501) staff       (20)     2115 2021-11-10 15:34:42.000000 bayesnewton-1.3.3/tests/test_vs_exact_marg_lik.py
--rw-r--r--   0 wwilkinson   (501) staff       (20)     5792 2021-11-10 15:34:42.000000 bayesnewton-1.3.3/tests/test_vs_gpflow_class.py
--rw-r--r--   0 wwilkinson   (501) staff       (20)     6586 2021-11-10 15:34:42.000000 bayesnewton-1.3.3/tests/test_vs_gpflow_reg.py
--rw-r--r--   0 wwilkinson   (501) staff       (20)     8557 2022-11-29 10:25:32.000000 bayesnewton-1.3.3/tests/test_vs_gpflow_shutters.py
--rw-r--r--   0 wwilkinson   (501) staff       (20)    10118 2021-11-10 15:34:42.000000 bayesnewton-1.3.3/tests/test_vs_gpflow_spacetime.py
+drwxr-xr-x   0 wwilkinson   (501) staff       (20)        0 2023-05-04 15:34:21.905675 bayesnewton-1.3.4/
+-rw-r--r--   0 wwilkinson   (501) staff       (20)    11357 2021-11-10 15:34:42.000000 bayesnewton-1.3.4/LICENSE
+-rw-r--r--   0 wwilkinson   (501) staff       (20)      170 2023-05-04 15:34:21.905534 bayesnewton-1.3.4/PKG-INFO
+-rw-r--r--   0 wwilkinson   (501) staff       (20)     8385 2022-11-29 10:26:07.000000 bayesnewton-1.3.4/README.md
+drwxr-xr-x   0 wwilkinson   (501) staff       (20)        0 2023-05-04 15:34:21.903059 bayesnewton-1.3.4/bayesnewton/
+-rw-r--r--   0 wwilkinson   (501) staff       (20)      211 2021-11-10 15:34:42.000000 bayesnewton-1.3.4/bayesnewton/__init__.py
+-rw-r--r--   0 wwilkinson   (501) staff       (20)    59304 2023-02-17 12:56:03.000000 bayesnewton-1.3.4/bayesnewton/basemodels.py
+-rw-r--r--   0 wwilkinson   (501) staff       (20)    19067 2022-11-07 13:19:06.000000 bayesnewton-1.3.4/bayesnewton/cubature.py
+-rw-r--r--   0 wwilkinson   (501) staff       (20)    43632 2023-02-17 12:56:03.000000 bayesnewton-1.3.4/bayesnewton/inference.py
+-rw-r--r--   0 wwilkinson   (501) staff       (20)    74634 2023-02-17 12:56:03.000000 bayesnewton-1.3.4/bayesnewton/kernels.py
+-rw-r--r--   0 wwilkinson   (501) staff       (20)   106886 2023-03-06 14:54:44.000000 bayesnewton-1.3.4/bayesnewton/likelihoods.py
+-rw-r--r--   0 wwilkinson   (501) staff       (20)    39746 2022-11-18 14:50:56.000000 bayesnewton-1.3.4/bayesnewton/models.py
+-rw-r--r--   0 wwilkinson   (501) staff       (20)    43172 2023-05-04 15:33:09.000000 bayesnewton-1.3.4/bayesnewton/ops.py
+-rw-r--r--   0 wwilkinson   (501) staff       (20)    25027 2023-02-17 12:56:03.000000 bayesnewton-1.3.4/bayesnewton/utils.py
+drwxr-xr-x   0 wwilkinson   (501) staff       (20)        0 2023-05-04 15:34:21.903785 bayesnewton-1.3.4/bayesnewton.egg-info/
+-rw-r--r--   0 wwilkinson   (501) staff       (20)      170 2023-05-04 15:34:21.000000 bayesnewton-1.3.4/bayesnewton.egg-info/PKG-INFO
+-rw-r--r--   0 wwilkinson   (501) staff       (20)      668 2023-05-04 15:34:21.000000 bayesnewton-1.3.4/bayesnewton.egg-info/SOURCES.txt
+-rw-r--r--   0 wwilkinson   (501) staff       (20)        1 2023-05-04 15:34:21.000000 bayesnewton-1.3.4/bayesnewton.egg-info/dependency_links.txt
+-rw-r--r--   0 wwilkinson   (501) staff       (20)       12 2023-05-04 15:34:21.000000 bayesnewton-1.3.4/bayesnewton.egg-info/top_level.txt
+-rw-r--r--   0 wwilkinson   (501) staff       (20)       38 2023-05-04 15:34:21.905711 bayesnewton-1.3.4/setup.cfg
+-rw-r--r--   0 wwilkinson   (501) staff       (20)      261 2023-05-04 15:33:18.000000 bayesnewton-1.3.4/setup.py
+drwxr-xr-x   0 wwilkinson   (501) staff       (20)        0 2023-05-04 15:34:21.905359 bayesnewton-1.3.4/tests/
+-rw-r--r--   0 wwilkinson   (501) staff       (20)     4347 2021-11-10 15:34:42.000000 bayesnewton-1.3.4/tests/test_gp_vs_markovgp_class.py
+-rw-r--r--   0 wwilkinson   (501) staff       (20)     5121 2021-11-10 15:34:42.000000 bayesnewton-1.3.4/tests/test_gp_vs_markovgp_reg.py
+-rw-r--r--   0 wwilkinson   (501) staff       (20)     7116 2021-11-10 15:34:42.000000 bayesnewton-1.3.4/tests/test_gp_vs_markovgp_spacetime.py
+-rw-r--r--   0 wwilkinson   (501) staff       (20)    12690 2021-11-10 15:34:42.000000 bayesnewton-1.3.4/tests/test_sparsemarkov.py
+-rw-r--r--   0 wwilkinson   (501) staff       (20)     2115 2021-11-10 15:34:42.000000 bayesnewton-1.3.4/tests/test_vs_exact_marg_lik.py
+-rw-r--r--   0 wwilkinson   (501) staff       (20)     5792 2021-11-10 15:34:42.000000 bayesnewton-1.3.4/tests/test_vs_gpflow_class.py
+-rw-r--r--   0 wwilkinson   (501) staff       (20)     6586 2021-11-10 15:34:42.000000 bayesnewton-1.3.4/tests/test_vs_gpflow_reg.py
+-rw-r--r--   0 wwilkinson   (501) staff       (20)     8557 2022-11-29 10:25:32.000000 bayesnewton-1.3.4/tests/test_vs_gpflow_shutters.py
+-rw-r--r--   0 wwilkinson   (501) staff       (20)    10118 2021-11-10 15:34:42.000000 bayesnewton-1.3.4/tests/test_vs_gpflow_spacetime.py
```

### Comparing `bayesnewton-1.3.3/LICENSE` & `bayesnewton-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bayesnewton-1.3.3/README.md` & `bayesnewton-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `bayesnewton-1.3.3/bayesnewton/basemodels.py` & `bayesnewton-1.3.4/bayesnewton/basemodels.py`

 * *Files identical despite different names*

### Comparing `bayesnewton-1.3.3/bayesnewton/cubature.py` & `bayesnewton-1.3.4/bayesnewton/cubature.py`

 * *Files identical despite different names*

### Comparing `bayesnewton-1.3.3/bayesnewton/inference.py` & `bayesnewton-1.3.4/bayesnewton/inference.py`

 * *Files identical despite different names*

### Comparing `bayesnewton-1.3.3/bayesnewton/kernels.py` & `bayesnewton-1.3.4/bayesnewton/kernels.py`

 * *Files identical despite different names*

### Comparing `bayesnewton-1.3.3/bayesnewton/likelihoods.py` & `bayesnewton-1.3.4/bayesnewton/likelihoods.py`

 * *Files identical despite different names*

### Comparing `bayesnewton-1.3.3/bayesnewton/models.py` & `bayesnewton-1.3.4/bayesnewton/models.py`

 * *Files identical despite different names*

### Comparing `bayesnewton-1.3.3/bayesnewton/ops.py` & `bayesnewton-1.3.4/bayesnewton/ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -565,15 +565,15 @@
     return AA, b, C, J, eta
 
 
 def _parallel_kf_mf(As, Qs, H, ys, noise_covs, m0, P0, masks, block_index):
 
     @vmap
     def build_block_diag(P_blocks):
-        P = Pzeros.at[0].add(P_blocks.flatten())
+        P = Pzeros.at[block_index].add(P_blocks.flatten())
         return P
 
     def build_mean(m):
         return m.reshape(num_time_steps, state_dim, 1)
 
     num_time_steps = As.shape[0]
     num_latents = As.shape[1]
```

### Comparing `bayesnewton-1.3.3/bayesnewton/utils.py` & `bayesnewton-1.3.4/bayesnewton/utils.py`

 * *Files identical despite different names*

### Comparing `bayesnewton-1.3.3/bayesnewton.egg-info/SOURCES.txt` & `bayesnewton-1.3.4/bayesnewton.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bayesnewton-1.3.3/tests/test_gp_vs_markovgp_class.py` & `bayesnewton-1.3.4/tests/test_gp_vs_markovgp_class.py`

 * *Files identical despite different names*

### Comparing `bayesnewton-1.3.3/tests/test_gp_vs_markovgp_reg.py` & `bayesnewton-1.3.4/tests/test_gp_vs_markovgp_reg.py`

 * *Files identical despite different names*

### Comparing `bayesnewton-1.3.3/tests/test_gp_vs_markovgp_spacetime.py` & `bayesnewton-1.3.4/tests/test_gp_vs_markovgp_spacetime.py`

 * *Files identical despite different names*

### Comparing `bayesnewton-1.3.3/tests/test_sparsemarkov.py` & `bayesnewton-1.3.4/tests/test_sparsemarkov.py`

 * *Files identical despite different names*

### Comparing `bayesnewton-1.3.3/tests/test_vs_exact_marg_lik.py` & `bayesnewton-1.3.4/tests/test_vs_exact_marg_lik.py`

 * *Files identical despite different names*

### Comparing `bayesnewton-1.3.3/tests/test_vs_gpflow_class.py` & `bayesnewton-1.3.4/tests/test_vs_gpflow_class.py`

 * *Files identical despite different names*

### Comparing `bayesnewton-1.3.3/tests/test_vs_gpflow_reg.py` & `bayesnewton-1.3.4/tests/test_vs_gpflow_reg.py`

 * *Files identical despite different names*

### Comparing `bayesnewton-1.3.3/tests/test_vs_gpflow_shutters.py` & `bayesnewton-1.3.4/tests/test_vs_gpflow_shutters.py`

 * *Files identical despite different names*

### Comparing `bayesnewton-1.3.3/tests/test_vs_gpflow_spacetime.py` & `bayesnewton-1.3.4/tests/test_vs_gpflow_spacetime.py`

 * *Files identical despite different names*

