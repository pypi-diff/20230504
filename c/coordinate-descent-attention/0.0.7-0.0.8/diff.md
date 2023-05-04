# Comparing `tmp/coordinate-descent-attention-0.0.7.tar.gz` & `tmp/coordinate-descent-attention-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coordinate-descent-attention-0.0.7.tar", last modified: Thu May  4 00:19:33 2023, max compression
+gzip compressed data, was "coordinate-descent-attention-0.0.8.tar", last modified: Thu May  4 02:39:36 2023, max compression
```

## Comparing `coordinate-descent-attention-0.0.7.tar` & `coordinate-descent-attention-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:19:33.260179 coordinate-descent-attention-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-04 00:19:19.000000 coordinate-descent-attention-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-04 00:19:33.260179 coordinate-descent-attention-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-04 00:19:19.000000 coordinate-descent-attention-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:19:33.256179 coordinate-descent-attention-0.0.7/coordinate_descent_attention/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-04 00:19:19.000000 coordinate-descent-attention-0.0.7/coordinate_descent_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-04 00:19:19.000000 coordinate-descent-attention-0.0.7/coordinate_descent_attention/autoregressive_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-05-04 00:19:19.000000 coordinate-descent-attention-0.0.7/coordinate_descent_attention/coordinate_descent_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:19:33.260179 coordinate-descent-attention-0.0.7/coordinate_descent_attention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-04 00:19:33.000000 coordinate-descent-attention-0.0.7/coordinate_descent_attention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-04 00:19:33.000000 coordinate-descent-attention-0.0.7/coordinate_descent_attention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 00:19:33.000000 coordinate-descent-attention-0.0.7/coordinate_descent_attention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-04 00:19:33.000000 coordinate-descent-attention-0.0.7/coordinate_descent_attention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-04 00:19:33.000000 coordinate-descent-attention-0.0.7/coordinate_descent_attention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 00:19:33.260179 coordinate-descent-attention-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-04 00:19:19.000000 coordinate-descent-attention-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:39:36.315890 coordinate-descent-attention-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-04 02:39:20.000000 coordinate-descent-attention-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-04 02:39:36.315890 coordinate-descent-attention-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-05-04 02:39:20.000000 coordinate-descent-attention-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:39:36.315890 coordinate-descent-attention-0.0.8/coordinate_descent_attention/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-04 02:39:20.000000 coordinate-descent-attention-0.0.8/coordinate_descent_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-04 02:39:20.000000 coordinate-descent-attention-0.0.8/coordinate_descent_attention/autoregressive_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-05-04 02:39:20.000000 coordinate-descent-attention-0.0.8/coordinate_descent_attention/coordinate_descent_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:39:36.315890 coordinate-descent-attention-0.0.8/coordinate_descent_attention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-04 02:39:36.000000 coordinate-descent-attention-0.0.8/coordinate_descent_attention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-04 02:39:36.000000 coordinate-descent-attention-0.0.8/coordinate_descent_attention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 02:39:36.000000 coordinate-descent-attention-0.0.8/coordinate_descent_attention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-04 02:39:36.000000 coordinate-descent-attention-0.0.8/coordinate_descent_attention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-04 02:39:36.000000 coordinate-descent-attention-0.0.8/coordinate_descent_attention.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 02:39:36.315890 coordinate-descent-attention-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-04 02:39:20.000000 coordinate-descent-attention-0.0.8/setup.py
```

### Comparing `coordinate-descent-attention-0.0.7/LICENSE` & `coordinate-descent-attention-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `coordinate-descent-attention-0.0.7/PKG-INFO` & `coordinate-descent-attention-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coordinate-descent-attention
-Version: 0.0.7
+Version: 0.0.8
 Summary: Coordinate Descent Attention - Pytorch
 Home-page: https://github.com/lucidrains/coodinate-descent-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,attention mechanism
 Classifier: Development Status :: 4 - Beta
```

### Comparing `coordinate-descent-attention-0.0.7/README.md` & `coordinate-descent-attention-0.0.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 logits = model(x)
 ```
 
 ## Todo
 
 - [x] let the network control sparsity k
 - [ ] ablate with topk attention, make sure it isn't because of hard attention
+- [ ] try coordinate descent with a few set sparsity levels for the hidden layer of the feedforward
 
 ## Citations
 
 ```bibtex
 @article{Wright2015CoordinateDA,
     title   = {Coordinate descent algorithms},
     author  = {Stephen J. Wright},
```

#### html2text {}

```diff
@@ -14,17 +14,19 @@
 descent-attention ``` ## Usage ```python import torch from
 coordinate_descent_attention import Transformer model = Transformer( num_tokens
 = 256, dim = 512, depth = 2, seq_len = 2048, dim_head = 64, heads = 8,
 use_coor_descent = True # set to True to switch from softmax to coordinate
 descent on qk similarity matrix ).cuda() x = torch.randint(0, 256, (1,
 2048)).cuda() logits = model(x) ``` ## Todo - [x] let the network control
 sparsity k - [ ] ablate with topk attention, make sure it isn't because of hard
-attention ## Citations ```bibtex @article{Wright2015CoordinateDA, title =
-{Coordinate descent algorithms}, author = {Stephen J. Wright}, journal =
-{Mathematical Programming}, year = {2015}, volume = {151}, pages = {3-34} } ```
-```bibtex @inproceedings{Gupta2021MemoryefficientTV, title = {Memory-efficient
-Transformers via Top-k Attention}, author = {Ankit Gupta and Guy Dar and Shaya
-Goodman and David Ciprut and Jonathan Berant}, booktitle = {SUSTAINLP}, year =
-{2021} } ``` ```bibtex @article{Zhao2019ExplicitST, title = {Explicit Sparse
-Transformer: Concentrated Attention Through Explicit Selection}, author =
-{Guangxiang Zhao and Junyang Lin and Zhiyuan Zhang and Xuancheng Ren and Qi Su
-and Xu Sun}, journal = {ArXiv}, year = {2019}, volume = {abs/1912.11637} } ```
+attention - [ ] try coordinate descent with a few set sparsity levels for the
+hidden layer of the feedforward ## Citations ```bibtex @article
+{Wright2015CoordinateDA, title = {Coordinate descent algorithms}, author =
+{Stephen J. Wright}, journal = {Mathematical Programming}, year = {2015},
+volume = {151}, pages = {3-34} } ``` ```bibtex @inproceedings
+{Gupta2021MemoryefficientTV, title = {Memory-efficient Transformers via Top-
+k Attention}, author = {Ankit Gupta and Guy Dar and Shaya Goodman and David
+Ciprut and Jonathan Berant}, booktitle = {SUSTAINLP}, year = {2021} } ```
+```bibtex @article{Zhao2019ExplicitST, title = {Explicit Sparse Transformer:
+Concentrated Attention Through Explicit Selection}, author = {Guangxiang Zhao
+and Junyang Lin and Zhiyuan Zhang and Xuancheng Ren and Qi Su and Xu Sun},
+journal = {ArXiv}, year = {2019}, volume = {abs/1912.11637} } ```
```

### Comparing `coordinate-descent-attention-0.0.7/coordinate_descent_attention/autoregressive_wrapper.py` & `coordinate-descent-attention-0.0.8/coordinate_descent_attention/autoregressive_wrapper.py`

 * *Files identical despite different names*

### Comparing `coordinate-descent-attention-0.0.7/coordinate_descent_attention/coordinate_descent_attention.py` & `coordinate-descent-attention-0.0.8/coordinate_descent_attention/coordinate_descent_attention.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,16 +47,14 @@
 
         self.use_coor_descent = use_coor_descent
 
         self.coor_descent_iters = coor_descent_iters
         self.coor_descent_sparsity_k = coor_descent_sparsity_k
         self.coor_descent_eps = coor_descent_eps
 
-        self.coor_descent_fn = coor_descent if learned_sparsity_k else triton_coor_descent
-
         self.to_learned_k = None
         if learned_sparsity_k:
             self.to_learned_k = nn.Linear(dim, heads)
             nn.init.constant_(self.to_learned_k.bias, -10)
 
         self.norm = nn.LayerNorm(dim)
 
@@ -97,15 +95,15 @@
                 sparsity_k = self.to_learned_k(x).sigmoid() * (self.coor_descent_sparsity_k - 1) + 1
                 sparsity_k = rearrange(sparsity_k, 'b i h -> (b h i)')
             else:
                 sparsity_k = torch.ones(i, device = device, dtype = dtype) * self.coor_descent_sparsity_k
 
             causal_mask = repeat(causal_mask, 'i j -> b h i j', b = sim.shape[0], h = sim.shape[1])
 
-            attn = self.coor_descent_fn(
+            attn = triton_coor_descent(
                 sim,
                 n_iters = self.coor_descent_iters,
                 k = sparsity_k,
                 eps = self.coor_descent_eps,
                 mask = ~causal_mask
             )
```

### Comparing `coordinate-descent-attention-0.0.7/coordinate_descent_attention.egg-info/PKG-INFO` & `coordinate-descent-attention-0.0.8/coordinate_descent_attention.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coordinate-descent-attention
-Version: 0.0.7
+Version: 0.0.8
 Summary: Coordinate Descent Attention - Pytorch
 Home-page: https://github.com/lucidrains/coodinate-descent-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,attention mechanism
 Classifier: Development Status :: 4 - Beta
```

### Comparing `coordinate-descent-attention-0.0.7/setup.py` & `coordinate-descent-attention-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'coordinate-descent-attention',
   packages = find_packages(exclude=[]),
-  version = '0.0.7',
+  version = '0.0.8',
   license='MIT',
   description = 'Coordinate Descent Attention - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/coodinate-descent-attention',
   keywords = [
     'artificial intelligence',
     'deep learning',
     'attention mechanism'
   ],
   install_requires=[
     'einops>=0.6.1',
     'torch>=1.6',
-    'colt5-attention>=0.5.0'
+    'colt5-attention>=0.5.2'
   ],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Topic :: Scientific/Engineering :: Artificial Intelligence',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3.6',
```

