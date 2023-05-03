# Comparing `tmp/coordinate-descent-attention-0.0.4.tar.gz` & `tmp/coordinate-descent-attention-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coordinate-descent-attention-0.0.4.tar", last modified: Wed Apr  5 21:15:14 2023, max compression
+gzip compressed data, was "coordinate-descent-attention-0.0.5.tar", last modified: Wed May  3 23:36:19 2023, max compression
```

## Comparing `coordinate-descent-attention-0.0.4.tar` & `coordinate-descent-attention-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 21:15:14.299418 coordinate-descent-attention-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-05 21:15:00.000000 coordinate-descent-attention-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-05 21:15:14.295418 coordinate-descent-attention-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-05 21:15:00.000000 coordinate-descent-attention-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 21:15:14.295418 coordinate-descent-attention-0.0.4/coordinate_descent_attention/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-05 21:15:00.000000 coordinate-descent-attention-0.0.4/coordinate_descent_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-05 21:15:00.000000 coordinate-descent-attention-0.0.4/coordinate_descent_attention/autoregressive_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-04-05 21:15:00.000000 coordinate-descent-attention-0.0.4/coordinate_descent_attention/coordinate_descent_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 21:15:14.295418 coordinate-descent-attention-0.0.4/coordinate_descent_attention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-05 21:15:14.000000 coordinate-descent-attention-0.0.4/coordinate_descent_attention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-05 21:15:14.000000 coordinate-descent-attention-0.0.4/coordinate_descent_attention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 21:15:14.000000 coordinate-descent-attention-0.0.4/coordinate_descent_attention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-05 21:15:14.000000 coordinate-descent-attention-0.0.4/coordinate_descent_attention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-05 21:15:14.000000 coordinate-descent-attention-0.0.4/coordinate_descent_attention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 21:15:14.299418 coordinate-descent-attention-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-05 21:15:00.000000 coordinate-descent-attention-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:36:19.159078 coordinate-descent-attention-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-03 23:36:06.000000 coordinate-descent-attention-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-03 23:36:19.159078 coordinate-descent-attention-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-05-03 23:36:06.000000 coordinate-descent-attention-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:36:19.159078 coordinate-descent-attention-0.0.5/coordinate_descent_attention/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-03 23:36:06.000000 coordinate-descent-attention-0.0.5/coordinate_descent_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-03 23:36:06.000000 coordinate-descent-attention-0.0.5/coordinate_descent_attention/autoregressive_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-05-03 23:36:06.000000 coordinate-descent-attention-0.0.5/coordinate_descent_attention/coordinate_descent_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:36:19.159078 coordinate-descent-attention-0.0.5/coordinate_descent_attention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-03 23:36:19.000000 coordinate-descent-attention-0.0.5/coordinate_descent_attention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-03 23:36:19.000000 coordinate-descent-attention-0.0.5/coordinate_descent_attention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 23:36:19.000000 coordinate-descent-attention-0.0.5/coordinate_descent_attention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-03 23:36:19.000000 coordinate-descent-attention-0.0.5/coordinate_descent_attention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-03 23:36:19.000000 coordinate-descent-attention-0.0.5/coordinate_descent_attention.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 23:36:19.159078 coordinate-descent-attention-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-03 23:36:06.000000 coordinate-descent-attention-0.0.5/setup.py
```

### Comparing `coordinate-descent-attention-0.0.4/LICENSE` & `coordinate-descent-attention-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `coordinate-descent-attention-0.0.4/PKG-INFO` & `coordinate-descent-attention-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coordinate-descent-attention
-Version: 0.0.4
+Version: 0.0.5
 Summary: Coordinate Descent Attention - Pytorch
 Home-page: https://github.com/lucidrains/coodinate-descent-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,attention mechanism
 Classifier: Development Status :: 4 - Beta
```

### Comparing `coordinate-descent-attention-0.0.4/README.md` & `coordinate-descent-attention-0.0.5/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -2,14 +2,20 @@
 
 Implementation of an Attention layer where each head can attend to more than just one token, using coordinate descent to pick topk. Perhaps the number of tokens to attend to can even be learned.
 
 In the case that experiments above fail, will use the repo for a few other ideas, among them getting coordinate descent routing working for autoregressive transformers.
 
 <a href="https://api.wandb.ai/links/lucidrains/7amjt5kw">Ongoing experiments</a>
 
+Update: I don't think the improvements are worth it. The memory usage becomes impractical as the number of iterations goes up as well. I'll keep playing around with topk attention though, because it bothers me that softmax becomes a bottleneck for the tokens far in the future, especially as sequence lengths go above 8k
+
+## Appreciation
+
+- <a href="https://stability.ai/">StabilityAI</a> for the sponsorship to carry out independent research
+
 ## Install
 
 ```bash
 $ pip install coordinate-descent-attention
 ```
 
 ## Usage
@@ -31,16 +37,16 @@
 x = torch.randint(0, 256, (1, 2048)).cuda()
 
 logits = model(x)
 ```
 
 ## Todo
 
+- [x] let the network control sparsity k
 - [ ] ablate with topk attention, make sure it isn't because of hard attention
-- [ ] let the network control sparsity k, potentially with maximum scaled as log(seq_len)
 
 ## Citations
 
 ```bibtex
 @article{Wright2015CoordinateDA,
     title   = {Coordinate descent algorithms},
     author  = {Stephen J. Wright},
```

#### html2text {}

```diff
@@ -1,24 +1,28 @@
 ## Coordinate Descent Attention (wip) Implementation of an Attention layer
 where each head can attend to more than just one token, using coordinate
 descent to pick topk. Perhaps the number of tokens to attend to can even be
 learned. In the case that experiments above fail, will use the repo for a few
 other ideas, among them getting coordinate descent routing working for
-autoregressive transformers. Ongoing_experiments ## Install ```bash $ pip
-install coordinate-descent-attention ``` ## Usage ```python import torch from
-coordinate_descent_attention import Transformer model = Transformer( num_tokens
-= 256, dim = 512, depth = 2, seq_len = 2048, dim_head = 64, heads = 8,
-use_coor_descent = True # set to True to switch from softmax to coordinate
-descent on qk similarity matrix ).cuda() x = torch.randint(0, 256, (1,
-2048)).cuda() logits = model(x) ``` ## Todo - [ ] ablate with topk attention,
-make sure it isn't because of hard attention - [ ] let the network control
-sparsity k, potentially with maximum scaled as log(seq_len) ## Citations
-```bibtex @article{Wright2015CoordinateDA, title = {Coordinate descent
-algorithms}, author = {Stephen J. Wright}, journal = {Mathematical
-Programming}, year = {2015}, volume = {151}, pages = {3-34} } ``` ```bibtex
-@inproceedings{Gupta2021MemoryefficientTV, title = {Memory-efficient
+autoregressive transformers. Ongoing_experiments Update: I don't think the
+improvements are worth it. The memory usage becomes impractical as the number
+of iterations goes up as well. I'll keep playing around with topk attention
+though, because it bothers me that softmax becomes a bottleneck for the tokens
+far in the future, especially as sequence lengths go above 8k ## Appreciation -
+StabilityAI for the sponsorship to carry out independent research ## Install
+```bash $ pip install coordinate-descent-attention ``` ## Usage ```python
+import torch from coordinate_descent_attention import Transformer model =
+Transformer( num_tokens = 256, dim = 512, depth = 2, seq_len = 2048, dim_head =
+64, heads = 8, use_coor_descent = True # set to True to switch from softmax to
+coordinate descent on qk similarity matrix ).cuda() x = torch.randint(0, 256,
+(1, 2048)).cuda() logits = model(x) ``` ## Todo - [x] let the network control
+sparsity k - [ ] ablate with topk attention, make sure it isn't because of hard
+attention ## Citations ```bibtex @article{Wright2015CoordinateDA, title =
+{Coordinate descent algorithms}, author = {Stephen J. Wright}, journal =
+{Mathematical Programming}, year = {2015}, volume = {151}, pages = {3-34} } ```
+```bibtex @inproceedings{Gupta2021MemoryefficientTV, title = {Memory-efficient
 Transformers via Top-k Attention}, author = {Ankit Gupta and Guy Dar and Shaya
 Goodman and David Ciprut and Jonathan Berant}, booktitle = {SUSTAINLP}, year =
 {2021} } ``` ```bibtex @article{Zhao2019ExplicitST, title = {Explicit Sparse
 Transformer: Concentrated Attention Through Explicit Selection}, author =
 {Guangxiang Zhao and Junyang Lin and Zhiyuan Zhang and Xuancheng Ren and Qi Su
 and Xu Sun}, journal = {ArXiv}, year = {2019}, volume = {abs/1912.11637} } ```
```

### Comparing `coordinate-descent-attention-0.0.4/coordinate_descent_attention/autoregressive_wrapper.py` & `coordinate-descent-attention-0.0.5/coordinate_descent_attention/autoregressive_wrapper.py`

 * *Files identical despite different names*

### Comparing `coordinate-descent-attention-0.0.4/coordinate_descent_attention/coordinate_descent_attention.py` & `coordinate-descent-attention-0.0.5/coordinate_descent_attention/coordinate_descent_attention.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,23 @@
 import torch
 import torch.nn.functional as F
 from torch import nn, einsum
 
 from einops import rearrange, repeat
 
+from colt5_attention.triton_coor_descent import triton_coor_descent
+
 # helpers
 
 def exists(val):
     return val is not None
 
 def default(val, d):
     return val if exists(val) else d
 
-# tensor helpers
-
-def log(t, eps = 1e-20):
-    return torch.log(t.clamp(min = eps))
-
-# coordinate descent helpers
-
-def coor_descent(
-    s,
-    *,
-    n_iters,
-    k,
-    eps = 1e-1,
-    clamp_fn = F.relu,
-    mask = None,
-):
-    mask_value = -torch.finfo(s.dtype).max
-    constant = eps * log(k)
-
-    b = -clamp_fn(s)
-
-    for _ in range(n_iters):
-        if exists(mask):
-            s = s.masked_fill(~mask, mask_value)
-
-        a = constant - eps * ((s + b) / eps).logsumexp(dim = -1, keepdim = True)
-        b = -clamp_fn(s + a)
-
-    if exists(mask):
-        s = s.masked_fill(~mask, mask_value)
-
-    scores = ((s + a + b) / eps).exp()
-    return scores
-
 # classes
 
 def FeedForward(dim, mult = 4):
     dim_hidden = int(dim * mult)
 
     return nn.Sequential(
         nn.LayerNorm(dim),
@@ -63,26 +31,28 @@
         self,
         dim,
         dim_head = 64,
         heads = 8,
         use_coor_descent = False,
         coor_descent_iters = 50,
         coor_descent_sparsity_k = 1,
+        coor_descent_sparsity_k_ratio = 9 / 8,
         coor_descent_eps = 1e-1,
         attn_null_kv = 0,
         learned_sparsity_k = False
     ):
         super().__init__()
         self.scale = dim_head ** -0.5
         self.heads = heads
         dim_inner = dim_head * heads
 
         self.use_coor_descent = use_coor_descent
         self.coor_descent_iters = coor_descent_iters
         self.coor_descent_sparsity_k = coor_descent_sparsity_k
+        self.coor_descent_sparsity_k_ratio = coor_descent_sparsity_k_ratio
         self.coor_descent_eps = coor_descent_eps
 
         self.to_learned_k = None
         if learned_sparsity_k:
             self.to_learned_k = nn.Linear(dim, heads)
             nn.init.constant_(self.to_learned_k.bias, -10)
 
@@ -119,23 +89,26 @@
 
         # whether to use coordinate descent or not
 
         if self.use_coor_descent:
 
             if exists(self.to_learned_k):
                 sparsity_k = self.to_learned_k(x).sigmoid() * (self.coor_descent_sparsity_k - 1) + 1
-                sparsity_k = rearrange(sparsity_k, 'b i h -> b h i 1')
+                sparsity_k = rearrange(sparsity_k, 'b i h -> (b h i)')
             else:
                 sparsity_k = torch.ones(i, device = device, dtype = dtype) * self.coor_descent_sparsity_k
-                sparsity_k = rearrange(sparsity_k, 'i -> i 1')
 
-            attn = coor_descent(
+            effective_k = sparsity_k * self.coor_descent_sparsity_k_ratio
+
+            causal_mask = repeat(causal_mask, 'i j -> b h i j', b = sim.shape[0], h = sim.shape[1])
+
+            attn = triton_coor_descent(
                 sim,
                 n_iters = self.coor_descent_iters,
-                k = sparsity_k,
+                k = effective_k,
                 eps = self.coor_descent_eps,
                 mask = ~causal_mask
             )
         else:
             sim = sim.masked_fill(causal_mask, -torch.finfo(sim.dtype).max)
             attn = sim.softmax(dim = -1)
```

### Comparing `coordinate-descent-attention-0.0.4/coordinate_descent_attention.egg-info/PKG-INFO` & `coordinate-descent-attention-0.0.5/coordinate_descent_attention.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coordinate-descent-attention
-Version: 0.0.4
+Version: 0.0.5
 Summary: Coordinate Descent Attention - Pytorch
 Home-page: https://github.com/lucidrains/coodinate-descent-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,attention mechanism
 Classifier: Development Status :: 4 - Beta
```

### Comparing `coordinate-descent-attention-0.0.4/setup.py` & `coordinate-descent-attention-0.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'coordinate-descent-attention',
   packages = find_packages(exclude=[]),
-  version = '0.0.4',
+  version = '0.0.5',
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
-    'einops>=0.4',
+    'einops>=0.6.1',
     'torch>=1.6',
+    'colt5-attention>=0.5.0'
   ],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Topic :: Scientific/Engineering :: Artificial Intelligence',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3.6',
```

