# Comparing `tmp/CoLT5-attention-0.5.3.tar.gz` & `tmp/CoLT5-attention-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CoLT5-attention-0.5.3.tar", last modified: Thu May  4 15:29:25 2023, max compression
+gzip compressed data, was "CoLT5-attention-0.5.4.tar", last modified: Thu May  4 20:17:42 2023, max compression
```

## Comparing `CoLT5-attention-0.5.3.tar` & `CoLT5-attention-0.5.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:29:25.233439 CoLT5-attention-0.5.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:29:25.229439 CoLT5-attention-0.5.3/CoLT5_attention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-04 15:29:25.000000 CoLT5-attention-0.5.3/CoLT5_attention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-04 15:29:25.000000 CoLT5-attention-0.5.3/CoLT5_attention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 15:29:25.000000 CoLT5-attention-0.5.3/CoLT5_attention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-04 15:29:25.000000 CoLT5-attention-0.5.3/CoLT5_attention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-04 15:29:25.000000 CoLT5-attention-0.5.3/CoLT5_attention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-04 15:29:06.000000 CoLT5-attention-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-04 15:29:25.233439 CoLT5-attention-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9795 2023-05-04 15:29:06.000000 CoLT5-attention-0.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:29:25.233439 CoLT5-attention-0.5.3/colt5_attention/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-04 15:29:06.000000 CoLT5-attention-0.5.3/colt5_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-04 15:29:06.000000 CoLT5-attention-0.5.3/colt5_attention/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-04 15:29:06.000000 CoLT5-attention-0.5.3/colt5_attention/coor_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-04 15:29:06.000000 CoLT5-attention-0.5.3/colt5_attention/sinkhorn.py
--rw-r--r--   0 runner    (1001) docker     (123)    34323 2023-05-04 15:29:06.000000 CoLT5-attention-0.5.3/colt5_attention/transformer_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     8506 2023-05-04 15:29:06.000000 CoLT5-attention-0.5.3/colt5_attention/triton_coor_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 15:29:25.233439 CoLT5-attention-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-04 15:29:06.000000 CoLT5-attention-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:17:42.699657 CoLT5-attention-0.5.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:17:42.699657 CoLT5-attention-0.5.4/CoLT5_attention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-04 20:17:42.000000 CoLT5-attention-0.5.4/CoLT5_attention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-04 20:17:42.000000 CoLT5-attention-0.5.4/CoLT5_attention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 20:17:42.000000 CoLT5-attention-0.5.4/CoLT5_attention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-04 20:17:42.000000 CoLT5-attention-0.5.4/CoLT5_attention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-04 20:17:42.000000 CoLT5-attention-0.5.4/CoLT5_attention.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-04 20:17:25.000000 CoLT5-attention-0.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-04 20:17:42.699657 CoLT5-attention-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10027 2023-05-04 20:17:25.000000 CoLT5-attention-0.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:17:42.699657 CoLT5-attention-0.5.4/colt5_attention/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-04 20:17:25.000000 CoLT5-attention-0.5.4/colt5_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-04 20:17:25.000000 CoLT5-attention-0.5.4/colt5_attention/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-04 20:17:25.000000 CoLT5-attention-0.5.4/colt5_attention/coor_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-04 20:17:25.000000 CoLT5-attention-0.5.4/colt5_attention/sinkhorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35809 2023-05-04 20:17:25.000000 CoLT5-attention-0.5.4/colt5_attention/transformer_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-05-04 20:17:25.000000 CoLT5-attention-0.5.4/colt5_attention/triton_coor_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 20:17:42.699657 CoLT5-attention-0.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-04 20:17:25.000000 CoLT5-attention-0.5.4/setup.py
```

### Comparing `CoLT5-attention-0.5.3/CoLT5_attention.egg-info/PKG-INFO` & `CoLT5-attention-0.5.4/CoLT5_attention.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.5.3
+Version: 0.5.4
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.5.3/LICENSE` & `CoLT5-attention-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.5.3/PKG-INFO` & `CoLT5-attention-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.5.3
+Version: 0.5.4
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.5.3/README.md` & `CoLT5-attention-0.5.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -92,39 +92,41 @@
 
 ```python
 import torch
 from colt5_attention import ConditionalRoutedCrossAttention
 
 # mock input, let us say it is a transformer of 1024 length attending to 1 million context past memories
 
-tokens = torch.randn(2, 1024, 512).cuda()
-tokens_mask = torch.ones(2, 1024).bool().cuda()
+tokens = torch.randn(1, 1024, 512).cuda()
+tokens_mask = torch.ones(1, 1024).bool().cuda()
 
-memories = torch.randn(2, int(1e6), 512).cuda()
-memories_mask = torch.ones(2, int(1e6)).bool().cuda()
+memories = torch.randn(1, 1_048_576, 512).cuda()
+memories_mask = torch.ones(1, 1_048_576).bool().cuda()
 
 # conditionally routed cross attention
 
 cross_attn = ConditionalRoutedCrossAttention(
     dim = 512,
     dim_head = 64,
     heads = 8,
     num_tokens_q = 512,         # only 512 routed from 1024
     num_tokens_kv = 1024,       # only 1024 routed from 1 million
     kv_routing_tokens = 2,      # say you want 2 routing tokens to route different sets of key / values to the queries. 4 attention heads will be allocated to each routed set in this example (8 / 2)
+    use_triton = True,          # use cuda kernel
+    route_block_size = 131072   # route in blocks of 131072
 ).cuda()
 
 cross_attn_out = cross_attn(
     tokens,
     context = memories,
     mask = tokens_mask,
     context_mask = memories_mask
 )
 
-cross_attn_out.shape # (2, 1024, 512) - same as tokens
+cross_attn_out.shape # (1, 1024, 512) - same as tokens
 ```
 
 Finally, this repository also has an improvised version for autoregressive attention. The way this was achieved was by viewing the sequence in windows. Each window can only attend to windows of key / values into the past. The local attention of the light branch covers the intra-window attention.
 
 The coordinate descent is made viable through a CUDA kernel written in <a href="https://github.com/openai/triton">Triton</a>. Finally, to get autoregressive generation to work well, I had to make sure for the unrouted tokens (for queries), outputs a learned output embedding rather than just zeros.
 
 Currently I am seeing occasional differences between the gradients (as high as 1e-1 for a very small fraction of elements) once the number of iterations exceed 20. However, enwik8 seems to train well and I can see the effects of the routing. Training is surprisingly stable too
@@ -172,16 +174,17 @@
     - [x] forwards        
     - [x] backwards
     - [x] add some tests and benchmark for triton vs plain pytorch coor_descent - 10x faster for forward, 4x faster for backwards and memory saved is n_iters times
     - [x] fall back on plain coordinate descent for cpu
     - [x] handle edge case for when a row is completely masked out for triton, or simply enforce it never to be so
     - [x] fix masking in coordinate descent
     - [x] simplified some logic within the triton kernel and the problem went away. probably some tiny quirk with the compiler
+    - [x] maximum block size in triton allowed is 131k, make sure at least quarter of million sequence length can be reached. to get around this initially, one can fold a million token sequence into ~9 131k and uniformly route. offer uniform routing scheme within router itself
     - [ ] allow for saving intermediates every number of iterations - trading memory for recompute efficiency during backwards
-    - [ ] maximum block size in triton allowed is 131k, make sure at least quarter of million sequence length can be reached. to get around this initially, one can fold a million token sequence into ~9 131k and uniformly route. offer uniform routing scheme within router itself
+    - [ ] remove sinkhorn and cumulative softmax approaches and cleanup; neither can work as well as coordinate descent
 
 ## Citations
 
 ```bibtex
 @inproceedings{Ainslie2023CoLT5FL,
     title   = {CoLT5: Faster Long-Range Transformers with Conditional Computation},
     author  = {Joshua Ainslie and Tao Lei and Michiel de Jong and Santiago Ontan'on and Siddhartha Brahma and Yury Zemlyanskiy and David Uthus and Mandy Guo and James Lee-Thorp and Yi Tay and Yun-Hsuan Sung and Sumit Sanghai},
```

#### html2text {}

```diff
@@ -37,28 +37,29 @@
 'coor_descent' # you have your choice of coordinate descent, as in paper - or
 'sinkhorn' or 'cum_softmax' ) block_out = block(tokens, mask = mask) # (2,
 32768, 512) ``` Also included a variation of the conditionally routed attention
 for cross attention, to be tried with long context memories in a transformer-xl
 ```python import torch from colt5_attention import
 ConditionalRoutedCrossAttention # mock input, let us say it is a transformer of
 1024 length attending to 1 million context past memories tokens = torch.randn
-(2, 1024, 512).cuda() tokens_mask = torch.ones(2, 1024).bool().cuda() memories
-= torch.randn(2, int(1e6), 512).cuda() memories_mask = torch.ones(2, int
-(1e6)).bool().cuda() # conditionally routed cross attention cross_attn =
+(1, 1024, 512).cuda() tokens_mask = torch.ones(1, 1024).bool().cuda() memories
+= torch.randn(1, 1_048_576, 512).cuda() memories_mask = torch.ones(1,
+1_048_576).bool().cuda() # conditionally routed cross attention cross_attn =
 ConditionalRoutedCrossAttention( dim = 512, dim_head = 64, heads = 8,
 num_tokens_q = 512, # only 512 routed from 1024 num_tokens_kv = 1024, # only
 1024 routed from 1 million kv_routing_tokens = 2, # say you want 2 routing
 tokens to route different sets of key / values to the queries. 4 attention
-heads will be allocated to each routed set in this example (8 / 2) ).cuda()
-cross_attn_out = cross_attn( tokens, context = memories, mask = tokens_mask,
-context_mask = memories_mask ) cross_attn_out.shape # (2, 1024, 512) - same as
-tokens ``` Finally, this repository also has an improvised version for
-autoregressive attention. The way this was achieved was by viewing the sequence
-in windows. Each window can only attend to windows of key / values into the
-past. The local attention of the light branch covers the intra-window
+heads will be allocated to each routed set in this example (8 / 2) use_triton =
+True, # use cuda kernel route_block_size = 131072 # route in blocks of 131072
+).cuda() cross_attn_out = cross_attn( tokens, context = memories, mask =
+tokens_mask, context_mask = memories_mask ) cross_attn_out.shape # (1, 1024,
+512) - same as tokens ``` Finally, this repository also has an improvised
+version for autoregressive attention. The way this was achieved was by viewing
+the sequence in windows. Each window can only attend to windows of key / values
+into the past. The local attention of the light branch covers the intra-window
 attention. The coordinate descent is made viable through a CUDA kernel written
 in Triton. Finally, to get autoregressive generation to work well, I had to
 make sure for the unrouted tokens (for queries), outputs a learned output
 embedding rather than just zeros. Currently I am seeing occasional differences
 between the gradients (as high as 1e-1 for a very small fraction of elements)
 once the number of iterations exceed 20. However, enwik8 seems to train well
 and I can see the effects of the routing. Training is surprisingly stable too
@@ -91,27 +92,28 @@
 out for diffusion - [ ] fused coordinate descent kernel using triton - [x]
 forwards - [x] backwards - [x] add some tests and benchmark for triton vs plain
 pytorch coor_descent - 10x faster for forward, 4x faster for backwards and
 memory saved is n_iters times - [x] fall back on plain coordinate descent for
 cpu - [x] handle edge case for when a row is completely masked out for triton,
 or simply enforce it never to be so - [x] fix masking in coordinate descent -
 [x] simplified some logic within the triton kernel and the problem went away.
-probably some tiny quirk with the compiler - [ ] allow for saving intermediates
-every number of iterations - trading memory for recompute efficiency during
-backwards - [ ] maximum block size in triton allowed is 131k, make sure at
-least quarter of million sequence length can be reached. to get around this
-initially, one can fold a million token sequence into ~9 131k and uniformly
-route. offer uniform routing scheme within router itself ## Citations ```bibtex
-@inproceedings{Ainslie2023CoLT5FL, title = {CoLT5: Faster Long-Range
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
+probably some tiny quirk with the compiler - [x] maximum block size in triton
+allowed is 131k, make sure at least quarter of million sequence length can be
+reached. to get around this initially, one can fold a million token sequence
+into ~9 131k and uniformly route. offer uniform routing scheme within router
+itself - [ ] allow for saving intermediates every number of iterations -
+trading memory for recompute efficiency during backwards - [ ] remove sinkhorn
+and cumulative softmax approaches and cleanup; neither can work as well as
+coordinate descent ## Citations ```bibtex @inproceedings{Ainslie2023CoLT5FL,
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

### Comparing `CoLT5-attention-0.5.3/colt5_attention/attend.py` & `CoLT5-attention-0.5.4/colt5_attention/attend.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.5.3/colt5_attention/coor_descent.py` & `CoLT5-attention-0.5.4/colt5_attention/coor_descent.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.5.3/colt5_attention/sinkhorn.py` & `CoLT5-attention-0.5.4/colt5_attention/sinkhorn.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.5.3/colt5_attention/transformer_block.py` & `CoLT5-attention-0.5.4/colt5_attention/transformer_block.py`

 * *Files 2% similar despite different names*

```diff
@@ -369,15 +369,16 @@
         self,
         dim,
         straight_through = True,
         n_iters = 50,           # 50 iterations in the paper
         fetch_k_ratio = 9 / 8,  # in the paper, they do a bit slightly higher k (times this ratio) for better learning
         eps = 1.,               # the epsilon for coordinate descent. in CoLT5 paper they used 1. apparently
         num_routing_tokens = 1,
-        use_triton = False
+        use_triton = False,
+        route_block_size = None
     ):
         super().__init__()
         assert fetch_k_ratio >= 1.
         self.eps = eps
 
         self.n_iters = n_iters
         self.fetch_k_ratio = fetch_k_ratio
@@ -386,14 +387,17 @@
 
         if use_triton:
             from colt5_attention.triton_coor_descent import triton_coor_descent
             self.coor_descent = triton_coor_descent
 
         self.is_one_routing_token = num_routing_tokens == 1
         self.num_routing_tokens = num_routing_tokens
+
+        self.route_block_size = route_block_size
+
         self.routing_token = nn.Parameter(torch.randn(num_routing_tokens, dim))
         self.straight_through = straight_through
 
     def route_back(self, src, routed_tokens, indices):
         batch_range = create_batch_range(routed_tokens)
         src[batch_range, indices] = routed_tokens
         return src
@@ -401,15 +405,36 @@
     def forward(
         self,
         x,
         *,
         num_tokens,
         mask = None
     ):
-        n, device, eps, num_routes = x.shape[-2], x.device, self.eps, self.num_routing_tokens
+        n, device, eps, num_routes, route_block_size = x.shape[-2], x.device, self.eps, self.num_routing_tokens, self.route_block_size
+
+        # whether to route even amounts from blocks of the sequence
+
+        if exists(route_block_size):
+            num_blocks = n // route_block_size
+            prev_seq_mult = num_blocks * route_block_size
+
+            # just curtail to last multiple of route block size
+
+            x = x[:, :prev_seq_mult]
+
+            # group sequence into blocks to route
+
+            x = rearrange(x, 'b (n w) d -> (b n) w d', w = route_block_size)
+
+            if exists(mask):
+                mask = mask[:, :prev_seq_mult]
+                mask = rearrange(mask, 'b (n w) -> (b n) w', w = route_block_size)
+
+            n = route_block_size
+            num_tokens = math.ceil(num_tokens / num_blocks)
 
         # s stands for eventual normalized score
 
         s = einsum('b n d, r d -> b r n', x, self.routing_token)
 
         # merge routing dimension into batch
 
@@ -449,14 +474,24 @@
 
         # split out routing dimension again if need be
 
         if not self.is_one_routing_token:
             selected_scores = unpack_one(selected_scores, ps, '* n')
             selected_indices = unpack_one(selected_indices, ps, '* n')
 
+        # undo the windowing, if one were routing uniformly in blocks
+
+        if exists(route_block_size):
+            selected_scores = rearrange(selected_scores, '(b n) ... w -> b ... (n w)', n = num_blocks)
+            selected_indices = rearrange(selected_indices, '(b n) ... w -> b ... n w', n = num_blocks)
+
+            indices_offset = torch.arange(num_blocks, device = device) * route_block_size
+            selected_indices = selected_indices + rearrange(indices_offset, 'n -> n 1')
+            selected_indices = rearrange(selected_indices, 'b ... n w -> b ... (n w)')
+
         return selected_scores, selected_indices
 
 # all router types
 
 ROUTERS = dict(
     cum_softmax = DifferentiableTopKRouter,
     sinkhorn = SinkhornRouter,
@@ -873,15 +908,16 @@
         router_straight_through = True, # would make sure all normalized scores are 1., still differentiable
         router_type = 'coor_descent',
         router_kwargs: dict = {},
         kv_routing_tokens = 1,
         multiply_keys_by_score = False,
         use_triton = False,
         use_null_q_tokens = True,
-        use_flash_attn = False
+        use_flash_attn = False,
+        route_block_size = None
     ):
         super().__init__()
         assert router_type in ROUTERS.keys()
 
         self.router_type = router_type
 
         router_klass = ROUTERS.get(router_type)
@@ -902,14 +938,15 @@
             **router_kwargs
         )
 
         self.kv_router = router_klass(
             dim = dim,
             straight_through = router_straight_through,
             num_routing_tokens = kv_routing_tokens,
+            route_block_size = route_block_size,
             **router_kwargs
         )
 
         self.heavy_attn = Attention(
             dim = dim,
             dim_head = dim_head,
             heads = heads,
```

### Comparing `CoLT5-attention-0.5.3/colt5_attention/triton_coor_descent.py` & `CoLT5-attention-0.5.4/colt5_attention/triton_coor_descent.py`

 * *Files 3% similar despite different names*

```diff
@@ -294,14 +294,17 @@
             k = torch.full((n_rows,), k)
         elif k.ndim == 1:
             k = repeat(k, 'n -> (b n)', b = x.shape[0] // k.shape[0])
 
         k = k.to(x)
 
         BLOCK_SIZE = triton.next_power_of_2(n_cols)
+
+        assert BLOCK_SIZE <= 131072, 'the maximum block size allowed is 131072 for triton cuda kernel - set the `route_block_size` for the CoordinateDescentRouter to be this value or less in order to uniformly route to get around this limitation'
+
         num_warps = calc_num_warps(BLOCK_SIZE)
 
         y = torch.empty_like(x)
 
         coor_descent_kernel_forward[(n_rows,)](
             y,
             x,
```

### Comparing `CoLT5-attention-0.5.3/setup.py` & `CoLT5-attention-0.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'CoLT5-attention',
   packages = find_packages(),
-  version = '0.5.3',
+  version = '0.5.4',
   license='MIT',
   description = 'Conditionally Routed Attention',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/CoLT5-attention',
   keywords = [
```

