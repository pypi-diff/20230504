# Comparing `tmp/CoLT5-attention-0.4.8.tar.gz` & `tmp/CoLT5-attention-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CoLT5-attention-0.4.8.tar", last modified: Wed May  3 16:32:22 2023, max compression
+gzip compressed data, was "CoLT5-attention-0.4.9.tar", last modified: Wed May  3 17:00:48 2023, max compression
```

## Comparing `CoLT5-attention-0.4.8.tar` & `CoLT5-attention-0.4.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:32:22.899337 CoLT5-attention-0.4.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:32:22.899337 CoLT5-attention-0.4.8/CoLT5_attention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-03 16:32:22.000000 CoLT5-attention-0.4.8/CoLT5_attention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-03 16:32:22.000000 CoLT5-attention-0.4.8/CoLT5_attention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 16:32:22.000000 CoLT5-attention-0.4.8/CoLT5_attention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-03 16:32:22.000000 CoLT5-attention-0.4.8/CoLT5_attention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 16:32:22.000000 CoLT5-attention-0.4.8/CoLT5_attention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-03 16:32:09.000000 CoLT5-attention-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-03 16:32:22.899337 CoLT5-attention-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-05-03 16:32:09.000000 CoLT5-attention-0.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:32:22.899337 CoLT5-attention-0.4.8/colt5_attention/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-03 16:32:09.000000 CoLT5-attention-0.4.8/colt5_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-03 16:32:09.000000 CoLT5-attention-0.4.8/colt5_attention/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-03 16:32:09.000000 CoLT5-attention-0.4.8/colt5_attention/coor_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-03 16:32:09.000000 CoLT5-attention-0.4.8/colt5_attention/sinkhorn.py
--rw-r--r--   0 runner    (1001) docker     (123)    34285 2023-05-03 16:32:09.000000 CoLT5-attention-0.4.8/colt5_attention/transformer_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     8451 2023-05-03 16:32:09.000000 CoLT5-attention-0.4.8/colt5_attention/triton_coor_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 16:32:22.899337 CoLT5-attention-0.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-03 16:32:09.000000 CoLT5-attention-0.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:00:48.103401 CoLT5-attention-0.4.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:00:48.103401 CoLT5-attention-0.4.9/CoLT5_attention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-03 17:00:48.000000 CoLT5-attention-0.4.9/CoLT5_attention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-03 17:00:48.000000 CoLT5-attention-0.4.9/CoLT5_attention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 17:00:48.000000 CoLT5-attention-0.4.9/CoLT5_attention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-03 17:00:48.000000 CoLT5-attention-0.4.9/CoLT5_attention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 17:00:48.000000 CoLT5-attention-0.4.9/CoLT5_attention.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-03 17:00:31.000000 CoLT5-attention-0.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-03 17:00:48.103401 CoLT5-attention-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9538 2023-05-03 17:00:31.000000 CoLT5-attention-0.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:00:48.103401 CoLT5-attention-0.4.9/colt5_attention/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-03 17:00:31.000000 CoLT5-attention-0.4.9/colt5_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-03 17:00:31.000000 CoLT5-attention-0.4.9/colt5_attention/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-03 17:00:31.000000 CoLT5-attention-0.4.9/colt5_attention/coor_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-03 17:00:31.000000 CoLT5-attention-0.4.9/colt5_attention/sinkhorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34323 2023-05-03 17:00:31.000000 CoLT5-attention-0.4.9/colt5_attention/transformer_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8451 2023-05-03 17:00:31.000000 CoLT5-attention-0.4.9/colt5_attention/triton_coor_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 17:00:48.103401 CoLT5-attention-0.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-03 17:00:31.000000 CoLT5-attention-0.4.9/setup.py
```

### Comparing `CoLT5-attention-0.4.8/CoLT5_attention.egg-info/PKG-INFO` & `CoLT5-attention-0.4.9/CoLT5_attention.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.4.8
+Version: 0.4.9
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.4.8/LICENSE` & `CoLT5-attention-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.4.8/PKG-INFO` & `CoLT5-attention-0.4.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.4.8
+Version: 0.4.9
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.4.8/README.md` & `CoLT5-attention-0.4.9/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 Implementation of the conditionally routed efficient attention in the proposed <a href="https://arxiv.org/abs/2303.09752">CoLT5</a> architecture, in Pytorch.
 
 Besides their use of coordinate descent from <a href="https://arxiv.org/abs/2211.01267">this paper</a> (main algorithm originally from <a href="https://arxiv.org/abs/1502.04759">Wright et al</a>), will also add two other approaches, one based on cumulative softmax, the other gumbel sinkhorn (optimal transport).
 
 Update: unsure of how the routing normalized scores for the key-values are used. Did some improvising there, <a href="https://github.com/lucidrains/CoLT5-attention/blob/main/colt5_attention/transformer_block.py#L86">scaling the projected values</a>, but if you think you know the answer, please open an issue
 
+Update 2: seems to work well with the improvisation above
+
 ## Appreciation
 
 - <a href="https://stability.ai/">Stability.ai</a> for the generous sponsorship to work on cutting edge artificial intelligence research
 
 - <a href="https://github.com/arogozhnikov/einops">einops</a> for making my life easy
 
 - <a href="https://github.com/openai/triton">Triton</a> for allowing me to speed up coordinate descent with a fused implementation in just 2 days, sparing me from having to write a thousand lines of CUDA code
@@ -117,14 +119,46 @@
     mask = tokens_mask,
     context_mask = memories_mask
 )
 
 cross_attn_out.shape # (2, 1024, 512) - same as tokens
 ```
 
+Finally, this repository also has an improvised version for autoregressive attention. The way this was achieved was by viewing the sequence in windows. Each window can only attend to windows of key / values into the past. The local attention of the light branch covers the intra-window attention. The coordinate descent is made viable through a CUDA kernel written in <a href="https://github.com/openai/triton">Triton</a>.
+
+ex.
+
+```python
+import torch
+from colt5_attention import ConditionalRoutedAutoregressiveAttention
+
+# mock input, say it is 8192 length
+
+tokens = torch.randn(2, 8192, 512).cuda()
+
+# attention
+
+attn = ConditionalRoutedAutoregressiveAttention(
+    dim = 512,
+    light_dim_head = 64,          # attention head dimension of light branch
+    light_heads = 8,              # number of attention heads for light branch
+    light_window_size = 128,      # local attention receptive field for light
+    heavy_window_size = 128,      # the windowing for the routed heavy attention, by default, will be equal to the light window size. be aware if this is any greater than the light window size, there may be tokens that would be missed by attention
+    heavy_dim_head = 64,          # attention head dimension of heavy branch
+    heavy_heads = 8,              # number of attention heads for heavy branch
+    num_heavy_tokens_q = 32,      # heavy branch receives only 32 out of 128 of the windowed queries (1024 query tokens total)
+    num_heavy_tokens_kv = 1024,   # heavy branch receives only 1024 routed tokens for key-values
+    num_routed_kv = 2,            # one can split the attention heads so that groups of heads attend to different sets of key - values (2 routing tokens in this case)
+    use_triton = True,            # will need to use Triton for this to be viable, otherwise it is too slow and memory efficient with the number of iterations
+    use_flash_attn = True         # use flash attention in heavy branch
+).cuda()
+
+attn_out = attn(tokens) + tokens # (2, 8192, 512) - output of attention with residual (prenorm is included)
+```
+
 ## Todo
 
 - [x] add the coordinate descent method as another router
 - [x] allow for multi-headed routing (multiple routing tokens), only for key-values
 - [x] add an autoregressive version of the conditionally routed attention
 - [x] test out the autoregressive version and verify that more routed key / value tokens lead to better results - it works
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
 [./colt5.png] ## CoLT5 Attention - Pytorch Implementation of the conditionally
 routed efficient attention in the proposed CoLT5 architecture, in Pytorch.
 Besides their use of coordinate descent from this_paper (main algorithm
 originally from Wright_et_al), will also add two other approaches, one based on
 cumulative softmax, the other gumbel sinkhorn (optimal transport). Update:
 unsure of how the routing normalized scores for the key-values are used. Did
 some improvising there, scaling_the_projected_values, but if you think you know
-the answer, please open an issue ## Appreciation - Stability.ai for the
-generous sponsorship to work on cutting edge artificial intelligence research -
-einops for making my life easy - Triton for allowing me to speed up coordinate
-descent with a fused implementation in just 2 days, sparing me from having to
-write a thousand lines of CUDA code ## Install ```bash $ pip install colt5-
-attention ``` ## Usage ```python import torch from colt5_attention import
+the answer, please open an issue Update 2: seems to work well with the
+improvisation above ## Appreciation - Stability.ai for the generous sponsorship
+to work on cutting edge artificial intelligence research - einops for making my
+life easy - Triton for allowing me to speed up coordinate descent with a fused
+implementation in just 2 days, sparing me from having to write a thousand lines
+of CUDA code ## Install ```bash $ pip install colt5-attention ``` ## Usage
+```python import torch from colt5_attention import
 ( ConditionalRoutedFeedForward, ConditionalRoutedAttention,
 ConditionalRoutedTransformerBlock ) # mock input, say it is 32768 length tokens
 = torch.randn(2, 32768, 512) mask = torch.ones(2, 32768).bool() # can handle
 variable lengthed sequences # feedforward ff = ConditionalRoutedFeedForward
 ( dim = 512, light_ff_mult = 0.5, # hidden dimension ratio of light branch
 heavy_ff_mult = 4, # hidden dimension ratio of heavy branch num_heavy_tokens =
 1024 # heavy branch receives only 1024 routed tokens of 32768 ) ff_out = ff
@@ -46,43 +47,67 @@
 ConditionalRoutedCrossAttention( dim = 512, dim_head = 64, heads = 8,
 num_tokens_q = 512, # only 512 routed from 1024 num_tokens_kv = 1024, # only
 1024 routed from 1 million kv_routing_tokens = 2, # say you want 2 routing
 tokens to route different sets of key / values to the queries. 4 attention
 heads will be allocated to each routed set in this example (8 / 2) ).cuda()
 cross_attn_out = cross_attn( tokens, context = memories, mask = tokens_mask,
 context_mask = memories_mask ) cross_attn_out.shape # (2, 1024, 512) - same as
-tokens ``` ## Todo - [x] add the coordinate descent method as another router -
-[x] allow for multi-headed routing (multiple routing tokens), only for key-
-values - [x] add an autoregressive version of the conditionally routed
-attention - [x] test out the autoregressive version and verify that more routed
-key / value tokens lead to better results - it works - [ ] for variable
-sequence lengths, allow for setting k as a function of sequence lengths per
-sample in batch - [ ] create a variant of CoLT5 for high resolution feature
-maps (image attention) - then try out for diffusion - [ ] in the cross
-attention scenario, support for routing token that first queries the source
-tokens, before retrieving from memories - [ ] make flash attention compatible -
-[ ] fused coordinate descent kernel using triton - [x] forwards - [x] backwards
-- [x] add some tests and benchmark for triton vs plain pytorch coor_descent -
-10x faster for forward, 4x faster for backwards and memory saved is n_iters
-times - [x] fall back on plain coordinate descent for cpu - [x] handle edge
-case for when a row is completely masked out for triton, or simply enforce it
-never to be so - [x] fix masking in coordinate descent - [ ] allow for saving
-intermediates every number of iterations - trading memory for recompute
-efficiency during backwards - [ ] issue with intermittent gradient errors
-occurs only during masking - [ ] maximum block size in triton allowed is 131k,
-make sure at least quarter of million sequence length can be reached. to get
-around this initially, one can fold a million token sequence into ~9 131k and
-uniformly route. offer uniform routing scheme within router itself ## Citations
-```bibtex @inproceedings{Ainslie2023CoLT5FL, title = {CoLT5: Faster Long-Range
-Transformers with Conditional Computation}, author = {Joshua Ainslie and Tao
-Lei and Michiel de Jong and Santiago Ontan'on and Siddhartha Brahma and Yury
-Zemlyanskiy and David Uthus and Mandy Guo and James Lee-Thorp and Yi Tay and
-Yun-Hsuan Sung and Sumit Sanghai}, year = {2023} } ``` ```bibtex @article
-{Tillet2019TritonAI, title = {Triton: an intermediate language and compiler for
-tiled neural network computations}, author = {Philippe Tillet and H. Kung and
-D. Cox}, journal = {Proceedings of the 3rd ACM SIGPLAN International Workshop
-on Machine Learning and Programming Languages}, year = {2019} } ``` ```bibtex
-@inproceedings{dao2022flashattention, title = {Flash{A}ttention: Fast and
-Memory-Efficient Exact Attention with {IO}-Awareness}, author = {Dao, Tri and
-Fu, Daniel Y. and Ermon, Stefano and Rudra, Atri and R{\'e}, Christopher},
-booktitle = {Advances in Neural Information Processing Systems}, year = {2022}
-} ```
+tokens ``` Finally, this repository also has an improvised version for
+autoregressive attention. The way this was achieved was by viewing the sequence
+in windows. Each window can only attend to windows of key / values into the
+past. The local attention of the light branch covers the intra-window
+attention. The coordinate descent is made viable through a CUDA kernel written
+in Triton. ex. ```python import torch from colt5_attention import
+ConditionalRoutedAutoregressiveAttention # mock input, say it is 8192 length
+tokens = torch.randn(2, 8192, 512).cuda() # attention attn =
+ConditionalRoutedAutoregressiveAttention( dim = 512, light_dim_head = 64, #
+attention head dimension of light branch light_heads = 8, # number of attention
+heads for light branch light_window_size = 128, # local attention receptive
+field for light heavy_window_size = 128, # the windowing for the routed heavy
+attention, by default, will be equal to the light window size. be aware if this
+is any greater than the light window size, there may be tokens that would be
+missed by attention heavy_dim_head = 64, # attention head dimension of heavy
+branch heavy_heads = 8, # number of attention heads for heavy branch
+num_heavy_tokens_q = 32, # heavy branch receives only 32 out of 128 of the
+windowed queries (1024 query tokens total) num_heavy_tokens_kv = 1024, # heavy
+branch receives only 1024 routed tokens for key-values num_routed_kv = 2, # one
+can split the attention heads so that groups of heads attend to different sets
+of key - values (2 routing tokens in this case) use_triton = True, # will need
+to use Triton for this to be viable, otherwise it is too slow and memory
+efficient with the number of iterations use_flash_attn = True # use flash
+attention in heavy branch ).cuda() attn_out = attn(tokens) + tokens # (2, 8192,
+512) - output of attention with residual (prenorm is included) ``` ## Todo -
+[x] add the coordinate descent method as another router - [x] allow for multi-
+headed routing (multiple routing tokens), only for key-values - [x] add an
+autoregressive version of the conditionally routed attention - [x] test out the
+autoregressive version and verify that more routed key / value tokens lead to
+better results - it works - [ ] for variable sequence lengths, allow for
+setting k as a function of sequence lengths per sample in batch - [ ] create a
+variant of CoLT5 for high resolution feature maps (image attention) - then try
+out for diffusion - [ ] in the cross attention scenario, support for routing
+token that first queries the source tokens, before retrieving from memories -
+[ ] make flash attention compatible - [ ] fused coordinate descent kernel using
+triton - [x] forwards - [x] backwards - [x] add some tests and benchmark for
+triton vs plain pytorch coor_descent - 10x faster for forward, 4x faster for
+backwards and memory saved is n_iters times - [x] fall back on plain coordinate
+descent for cpu - [x] handle edge case for when a row is completely masked out
+for triton, or simply enforce it never to be so - [x] fix masking in coordinate
+descent - [ ] allow for saving intermediates every number of iterations -
+trading memory for recompute efficiency during backwards - [ ] issue with
+intermittent gradient errors occurs only during masking - [ ] maximum block
+size in triton allowed is 131k, make sure at least quarter of million sequence
+length can be reached. to get around this initially, one can fold a million
+token sequence into ~9 131k and uniformly route. offer uniform routing scheme
+within router itself ## Citations ```bibtex @inproceedings{Ainslie2023CoLT5FL,
+title = {CoLT5: Faster Long-Range Transformers with Conditional Computation},
+author = {Joshua Ainslie and Tao Lei and Michiel de Jong and Santiago Ontan'on
+and Siddhartha Brahma and Yury Zemlyanskiy and David Uthus and Mandy Guo and
+James Lee-Thorp and Yi Tay and Yun-Hsuan Sung and Sumit Sanghai}, year = {2023}
+} ``` ```bibtex @article{Tillet2019TritonAI, title = {Triton: an intermediate
+language and compiler for tiled neural network computations}, author =
+{Philippe Tillet and H. Kung and D. Cox}, journal = {Proceedings of the 3rd ACM
+SIGPLAN International Workshop on Machine Learning and Programming Languages},
+year = {2019} } ``` ```bibtex @inproceedings{dao2022flashattention, title =
+{Flash{A}ttention: Fast and Memory-Efficient Exact Attention with {IO}-
+Awareness}, author = {Dao, Tri and Fu, Daniel Y. and Ermon, Stefano and Rudra,
+Atri and R{\'e}, Christopher}, booktitle = {Advances in Neural Information
+Processing Systems}, year = {2022} } ```
```

### Comparing `CoLT5-attention-0.4.8/colt5_attention/attend.py` & `CoLT5-attention-0.4.9/colt5_attention/attend.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.4.8/colt5_attention/coor_descent.py` & `CoLT5-attention-0.4.9/colt5_attention/coor_descent.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.4.8/colt5_attention/sinkhorn.py` & `CoLT5-attention-0.4.9/colt5_attention/sinkhorn.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.4.8/colt5_attention/transformer_block.py` & `CoLT5-attention-0.4.9/colt5_attention/transformer_block.py`

 * *Files 0% similar despite different names*

```diff
@@ -714,14 +714,15 @@
         self.light_attn = LocalMHA(
             dim = dim,
             dim_head = light_dim_head,
             heads = light_heads,
             window_size = light_window_size,
             prenorm = True,
             causal = True,
+            exact_windowsize = False,
             use_rotary_pos_emb = False
         )
 
         self.null_q_token = None
         if use_null_q_tokens:
             self.null_q_token = nn.Parameter(torch.randn(dim)) # for the query tokens not selected by the router, give it a learned output embed
```

### Comparing `CoLT5-attention-0.4.8/colt5_attention/triton_coor_descent.py` & `CoLT5-attention-0.4.9/colt5_attention/triton_coor_descent.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.4.8/setup.py` & `CoLT5-attention-0.4.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'CoLT5-attention',
   packages = find_packages(),
-  version = '0.4.8',
+  version = '0.4.9',
   license='MIT',
   description = 'Conditionally Routed Attention',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/CoLT5-attention',
   keywords = [
     'artificial intelligence',
     'attention mechanism',
     'dynamic routing'
   ],
   install_requires=[
     'einops>=0.6.1',
-    'local-attention>=1.8.5',
+    'local-attention>=1.8.6',
     'packaging',
     'torch>=1.10'
   ],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Topic :: Scientific/Engineering :: Artificial Intelligence',
```

