# Comparing `tmp/CoLT5-attention-0.5.4.tar.gz` & `tmp/CoLT5-attention-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CoLT5-attention-0.5.4.tar", last modified: Thu May  4 20:17:42 2023, max compression
+gzip compressed data, was "CoLT5-attention-0.5.5.tar", last modified: Thu May  4 21:26:34 2023, max compression
```

## Comparing `CoLT5-attention-0.5.4.tar` & `CoLT5-attention-0.5.5.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:17:42.699657 CoLT5-attention-0.5.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:17:42.699657 CoLT5-attention-0.5.4/CoLT5_attention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-04 20:17:42.000000 CoLT5-attention-0.5.4/CoLT5_attention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-04 20:17:42.000000 CoLT5-attention-0.5.4/CoLT5_attention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 20:17:42.000000 CoLT5-attention-0.5.4/CoLT5_attention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-04 20:17:42.000000 CoLT5-attention-0.5.4/CoLT5_attention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-04 20:17:42.000000 CoLT5-attention-0.5.4/CoLT5_attention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-04 20:17:25.000000 CoLT5-attention-0.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-04 20:17:42.699657 CoLT5-attention-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10027 2023-05-04 20:17:25.000000 CoLT5-attention-0.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:17:42.699657 CoLT5-attention-0.5.4/colt5_attention/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-04 20:17:25.000000 CoLT5-attention-0.5.4/colt5_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-04 20:17:25.000000 CoLT5-attention-0.5.4/colt5_attention/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-04 20:17:25.000000 CoLT5-attention-0.5.4/colt5_attention/coor_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-04 20:17:25.000000 CoLT5-attention-0.5.4/colt5_attention/sinkhorn.py
--rw-r--r--   0 runner    (1001) docker     (123)    35809 2023-05-04 20:17:25.000000 CoLT5-attention-0.5.4/colt5_attention/transformer_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-05-04 20:17:25.000000 CoLT5-attention-0.5.4/colt5_attention/triton_coor_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 20:17:42.699657 CoLT5-attention-0.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-04 20:17:25.000000 CoLT5-attention-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:26:34.520100 CoLT5-attention-0.5.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:26:34.516100 CoLT5-attention-0.5.5/CoLT5_attention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-04 21:26:34.000000 CoLT5-attention-0.5.5/CoLT5_attention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-04 21:26:34.000000 CoLT5-attention-0.5.5/CoLT5_attention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 21:26:34.000000 CoLT5-attention-0.5.5/CoLT5_attention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-04 21:26:34.000000 CoLT5-attention-0.5.5/CoLT5_attention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-04 21:26:34.000000 CoLT5-attention-0.5.5/CoLT5_attention.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-04 21:26:03.000000 CoLT5-attention-0.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-04 21:26:34.520100 CoLT5-attention-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9865 2023-05-04 21:26:03.000000 CoLT5-attention-0.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:26:34.520100 CoLT5-attention-0.5.5/colt5_attention/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-04 21:26:03.000000 CoLT5-attention-0.5.5/colt5_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-04 21:26:03.000000 CoLT5-attention-0.5.5/colt5_attention/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-04 21:26:03.000000 CoLT5-attention-0.5.5/colt5_attention/coor_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29424 2023-05-04 21:26:03.000000 CoLT5-attention-0.5.5/colt5_attention/transformer_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-05-04 21:26:03.000000 CoLT5-attention-0.5.5/colt5_attention/triton_coor_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 21:26:34.520100 CoLT5-attention-0.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-04 21:26:03.000000 CoLT5-attention-0.5.5/setup.py
```

### Comparing `CoLT5-attention-0.5.4/CoLT5_attention.egg-info/PKG-INFO` & `CoLT5-attention-0.5.5/CoLT5_attention.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.5.4
+Version: 0.5.5
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.5.4/LICENSE` & `CoLT5-attention-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.5.4/PKG-INFO` & `CoLT5-attention-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.5.4
+Version: 0.5.5
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.5.4/README.md` & `CoLT5-attention-0.5.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <img src="./colt5.png" width="400px"></img>
 
 ## CoLT5 Attention - Pytorch
 
 Implementation of the conditionally routed efficient attention in the proposed <a href="https://arxiv.org/abs/2303.09752">CoLT5</a> architecture, in Pytorch.
 
-Besides their use of coordinate descent from <a href="https://arxiv.org/abs/2211.01267">this paper</a> (main algorithm originally from <a href="https://arxiv.org/abs/1502.04759">Wright et al</a>), will also add two other approaches, one based on cumulative softmax, the other gumbel sinkhorn (optimal transport).
+They used coordinate descent from <a href="https://arxiv.org/abs/2211.01267">this paper</a> (main algorithm originally from <a href="https://arxiv.org/abs/1502.04759">Wright et al</a>) to route a subset of tokens for 'heavier' branches of the feedforward and attention blocks.
 
 Update: unsure of how the routing normalized scores for the key-values are used. Did some improvising there, <a href="https://github.com/lucidrains/CoLT5-attention/blob/main/colt5_attention/transformer_block.py#L86">scaling the projected values</a>, but if you think you know the answer, please open an issue
 
 Update 2: seems to work well with the improvisation above
 
 ## Appreciation
 
@@ -77,16 +77,15 @@
     light_window_size = 128,
     heavy_dim_head = 64,
     heavy_heads = 8,
     light_ff_mult = 0.5,
     heavy_ff_mult = 4,
     num_heavy_ff_tokens = 1024,
     num_heavy_attn_tokens_q = 1024,
-    num_heavy_attn_tokens_kv = 1024,
-    router_type = 'coor_descent'  # you have your choice of coordinate descent, as in paper - or 'sinkhorn' or 'cum_softmax'
+    num_heavy_attn_tokens_kv = 1024
 )
 
 block_out = block(tokens, mask = mask) # (2, 32768, 512)
 ```
 
 Also included a variation of the conditionally routed attention for cross attention, to be tried with long context memories in a transformer-xl
 
@@ -175,16 +174,16 @@
     - [x] backwards
     - [x] add some tests and benchmark for triton vs plain pytorch coor_descent - 10x faster for forward, 4x faster for backwards and memory saved is n_iters times
     - [x] fall back on plain coordinate descent for cpu
     - [x] handle edge case for when a row is completely masked out for triton, or simply enforce it never to be so
     - [x] fix masking in coordinate descent
     - [x] simplified some logic within the triton kernel and the problem went away. probably some tiny quirk with the compiler
     - [x] maximum block size in triton allowed is 131k, make sure at least quarter of million sequence length can be reached. to get around this initially, one can fold a million token sequence into ~9 131k and uniformly route. offer uniform routing scheme within router itself
+    - [x] remove sinkhorn and cumulative softmax approaches and cleanup; neither can work as well as coordinate descent
     - [ ] allow for saving intermediates every number of iterations - trading memory for recompute efficiency during backwards
-    - [ ] remove sinkhorn and cumulative softmax approaches and cleanup; neither can work as well as coordinate descent
 
 ## Citations
 
 ```bibtex
 @inproceedings{Ainslie2023CoLT5FL,
     title   = {CoLT5: Faster Long-Range Transformers with Conditional Computation},
     author  = {Joshua Ainslie and Tao Lei and Michiel de Jong and Santiago Ontan'on and Siddhartha Brahma and Yury Zemlyanskiy and David Uthus and Mandy Guo and James Lee-Thorp and Yi Tay and Yun-Hsuan Sung and Sumit Sanghai},
```

#### html2text {}

```diff
@@ -1,21 +1,20 @@
 [./colt5.png] ## CoLT5 Attention - Pytorch Implementation of the conditionally
-routed efficient attention in the proposed CoLT5 architecture, in Pytorch.
-Besides their use of coordinate descent from this_paper (main algorithm
-originally from Wright_et_al), will also add two other approaches, one based on
-cumulative softmax, the other gumbel sinkhorn (optimal transport). Update:
-unsure of how the routing normalized scores for the key-values are used. Did
-some improvising there, scaling_the_projected_values, but if you think you know
-the answer, please open an issue Update 2: seems to work well with the
-improvisation above ## Appreciation - Stability.ai for the generous sponsorship
-to work on cutting edge artificial intelligence research - einops for making my
-life easy - Triton for allowing me to speed up coordinate descent with a fused
-implementation in just 2 days, sparing me from having to write a thousand lines
-of CUDA code ## Install ```bash $ pip install colt5-attention ``` ## Usage
-```python import torch from colt5_attention import
+routed efficient attention in the proposed CoLT5 architecture, in Pytorch. They
+used coordinate descent from this_paper (main algorithm originally from Wright
+et_al) to route a subset of tokens for 'heavier' branches of the feedforward
+and attention blocks. Update: unsure of how the routing normalized scores for
+the key-values are used. Did some improvising there, scaling_the_projected
+values, but if you think you know the answer, please open an issue Update 2:
+seems to work well with the improvisation above ## Appreciation - Stability.ai
+for the generous sponsorship to work on cutting edge artificial intelligence
+research - einops for making my life easy - Triton for allowing me to speed up
+coordinate descent with a fused implementation in just 2 days, sparing me from
+having to write a thousand lines of CUDA code ## Install ```bash $ pip install
+colt5-attention ``` ## Usage ```python import torch from colt5_attention import
 ( ConditionalRoutedFeedForward, ConditionalRoutedAttention,
 ConditionalRoutedTransformerBlock ) # mock input, say it is 32768 length tokens
 = torch.randn(2, 32768, 512) mask = torch.ones(2, 32768).bool() # can handle
 variable lengthed sequences # feedforward ff = ConditionalRoutedFeedForward
 ( dim = 512, light_ff_mult = 0.5, # hidden dimension ratio of light branch
 heavy_ff_mult = 4, # hidden dimension ratio of heavy branch num_heavy_tokens =
 1024 # heavy branch receives only 1024 routed tokens of 32768 ) ff_out = ff
@@ -29,91 +28,90 @@
 32768 num_heavy_tokens_kv = 1024 # heavy branch receives only 1024 routed
 tokens of 32768 ) attn_out = attn(tokens, mask = mask) # (2, 32768, 512) -
 light and heavy branch summed # both attention and feedforward with residual #
 the complete transformer block # a stack of these would constitute the encoder
 of CoLT5 block = ConditionalRoutedTransformerBlock( dim = 512, light_dim_head =
 64, light_heads = 8, light_window_size = 128, heavy_dim_head = 64, heavy_heads
 = 8, light_ff_mult = 0.5, heavy_ff_mult = 4, num_heavy_ff_tokens = 1024,
-num_heavy_attn_tokens_q = 1024, num_heavy_attn_tokens_kv = 1024, router_type =
-'coor_descent' # you have your choice of coordinate descent, as in paper - or
-'sinkhorn' or 'cum_softmax' ) block_out = block(tokens, mask = mask) # (2,
-32768, 512) ``` Also included a variation of the conditionally routed attention
-for cross attention, to be tried with long context memories in a transformer-xl
-```python import torch from colt5_attention import
-ConditionalRoutedCrossAttention # mock input, let us say it is a transformer of
-1024 length attending to 1 million context past memories tokens = torch.randn
-(1, 1024, 512).cuda() tokens_mask = torch.ones(1, 1024).bool().cuda() memories
-= torch.randn(1, 1_048_576, 512).cuda() memories_mask = torch.ones(1,
-1_048_576).bool().cuda() # conditionally routed cross attention cross_attn =
-ConditionalRoutedCrossAttention( dim = 512, dim_head = 64, heads = 8,
-num_tokens_q = 512, # only 512 routed from 1024 num_tokens_kv = 1024, # only
-1024 routed from 1 million kv_routing_tokens = 2, # say you want 2 routing
-tokens to route different sets of key / values to the queries. 4 attention
-heads will be allocated to each routed set in this example (8 / 2) use_triton =
-True, # use cuda kernel route_block_size = 131072 # route in blocks of 131072
-).cuda() cross_attn_out = cross_attn( tokens, context = memories, mask =
-tokens_mask, context_mask = memories_mask ) cross_attn_out.shape # (1, 1024,
-512) - same as tokens ``` Finally, this repository also has an improvised
-version for autoregressive attention. The way this was achieved was by viewing
-the sequence in windows. Each window can only attend to windows of key / values
-into the past. The local attention of the light branch covers the intra-window
-attention. The coordinate descent is made viable through a CUDA kernel written
-in Triton. Finally, to get autoregressive generation to work well, I had to
-make sure for the unrouted tokens (for queries), outputs a learned output
-embedding rather than just zeros. Currently I am seeing occasional differences
-between the gradients (as high as 1e-1 for a very small fraction of elements)
-once the number of iterations exceed 20. However, enwik8 seems to train well
-and I can see the effects of the routing. Training is surprisingly stable too
-ex. ```python import torch from colt5_attention import
-ConditionalRoutedAutoregressiveAttention # mock input, say it is 8192 length
-tokens = torch.randn(2, 8192, 512).cuda() # attention attn =
-ConditionalRoutedAutoregressiveAttention( dim = 512, light_dim_head = 64, #
-attention head dimension of light branch light_heads = 8, # number of attention
-heads for light branch light_window_size = 128, # local attention receptive
-field for light heavy_window_size = 128, # the windowing for the routed heavy
-attention, by default, will be equal to the light window size. be aware if this
-is any greater than the light window size, there may be tokens that would be
-missed by attention heavy_dim_head = 64, # attention head dimension of heavy
-branch heavy_heads = 8, # number of attention heads for heavy branch
-num_heavy_tokens_q = 32, # heavy branch receives only 32 out of 128 of the
-windowed queries (1024 query tokens total) num_heavy_tokens_kv = 1024, # heavy
-branch receives only 1024 routed tokens for key-values num_routed_kv = 2, # one
-can split the attention heads so that groups of heads attend to different sets
-of key - values (2 routing tokens in this case) use_triton = True, # will need
-to use Triton for this to be viable, otherwise it is too slow and memory
-efficient with the number of iterations use_flash_attn = True # use flash
-attention in heavy branch ).cuda() attn_out = attn(tokens) + tokens # (2, 8192,
-512) - output of attention with residual (prenorm is included) ``` ## Todo -
-[x] add the coordinate descent method as another router - [x] allow for multi-
-headed routing (multiple routing tokens), only for key-values - [x] add an
-autoregressive version of the conditionally routed attention - [x] test out the
-autoregressive version and verify that more routed key / value tokens lead to
-better results - it works - [x] make flash attention compatible - [ ] create a
-variant of CoLT5 for high resolution feature maps (image attention) - then try
-out for diffusion - [ ] fused coordinate descent kernel using triton - [x]
-forwards - [x] backwards - [x] add some tests and benchmark for triton vs plain
-pytorch coor_descent - 10x faster for forward, 4x faster for backwards and
-memory saved is n_iters times - [x] fall back on plain coordinate descent for
-cpu - [x] handle edge case for when a row is completely masked out for triton,
-or simply enforce it never to be so - [x] fix masking in coordinate descent -
-[x] simplified some logic within the triton kernel and the problem went away.
-probably some tiny quirk with the compiler - [x] maximum block size in triton
-allowed is 131k, make sure at least quarter of million sequence length can be
-reached. to get around this initially, one can fold a million token sequence
-into ~9 131k and uniformly route. offer uniform routing scheme within router
-itself - [ ] allow for saving intermediates every number of iterations -
-trading memory for recompute efficiency during backwards - [ ] remove sinkhorn
+num_heavy_attn_tokens_q = 1024, num_heavy_attn_tokens_kv = 1024 ) block_out =
+block(tokens, mask = mask) # (2, 32768, 512) ``` Also included a variation of
+the conditionally routed attention for cross attention, to be tried with long
+context memories in a transformer-xl ```python import torch from
+colt5_attention import ConditionalRoutedCrossAttention # mock input, let us say
+it is a transformer of 1024 length attending to 1 million context past memories
+tokens = torch.randn(1, 1024, 512).cuda() tokens_mask = torch.ones(1,
+1024).bool().cuda() memories = torch.randn(1, 1_048_576, 512).cuda()
+memories_mask = torch.ones(1, 1_048_576).bool().cuda() # conditionally routed
+cross attention cross_attn = ConditionalRoutedCrossAttention( dim = 512,
+dim_head = 64, heads = 8, num_tokens_q = 512, # only 512 routed from 1024
+num_tokens_kv = 1024, # only 1024 routed from 1 million kv_routing_tokens = 2,
+# say you want 2 routing tokens to route different sets of key / values to the
+queries. 4 attention heads will be allocated to each routed set in this example
+(8 / 2) use_triton = True, # use cuda kernel route_block_size = 131072 # route
+in blocks of 131072 ).cuda() cross_attn_out = cross_attn( tokens, context =
+memories, mask = tokens_mask, context_mask = memories_mask )
+cross_attn_out.shape # (1, 1024, 512) - same as tokens ``` Finally, this
+repository also has an improvised version for autoregressive attention. The way
+this was achieved was by viewing the sequence in windows. Each window can only
+attend to windows of key / values into the past. The local attention of the
+light branch covers the intra-window attention. The coordinate descent is made
+viable through a CUDA kernel written in Triton. Finally, to get autoregressive
+generation to work well, I had to make sure for the unrouted tokens (for
+queries), outputs a learned output embedding rather than just zeros. Currently
+I am seeing occasional differences between the gradients (as high as 1e-1 for a
+very small fraction of elements) once the number of iterations exceed 20.
+However, enwik8 seems to train well and I can see the effects of the routing.
+Training is surprisingly stable too ex. ```python import torch from
+colt5_attention import ConditionalRoutedAutoregressiveAttention # mock input,
+say it is 8192 length tokens = torch.randn(2, 8192, 512).cuda() # attention
+attn = ConditionalRoutedAutoregressiveAttention( dim = 512, light_dim_head =
+64, # attention head dimension of light branch light_heads = 8, # number of
+attention heads for light branch light_window_size = 128, # local attention
+receptive field for light heavy_window_size = 128, # the windowing for the
+routed heavy attention, by default, will be equal to the light window size. be
+aware if this is any greater than the light window size, there may be tokens
+that would be missed by attention heavy_dim_head = 64, # attention head
+dimension of heavy branch heavy_heads = 8, # number of attention heads for
+heavy branch num_heavy_tokens_q = 32, # heavy branch receives only 32 out of
+128 of the windowed queries (1024 query tokens total) num_heavy_tokens_kv =
+1024, # heavy branch receives only 1024 routed tokens for key-values
+num_routed_kv = 2, # one can split the attention heads so that groups of heads
+attend to different sets of key - values (2 routing tokens in this case)
+use_triton = True, # will need to use Triton for this to be viable, otherwise
+it is too slow and memory efficient with the number of iterations
+use_flash_attn = True # use flash attention in heavy branch ).cuda() attn_out =
+attn(tokens) + tokens # (2, 8192, 512) - output of attention with residual
+(prenorm is included) ``` ## Todo - [x] add the coordinate descent method as
+another router - [x] allow for multi-headed routing (multiple routing tokens),
+only for key-values - [x] add an autoregressive version of the conditionally
+routed attention - [x] test out the autoregressive version and verify that more
+routed key / value tokens lead to better results - it works - [x] make flash
+attention compatible - [ ] create a variant of CoLT5 for high resolution
+feature maps (image attention) - then try out for diffusion - [ ] fused
+coordinate descent kernel using triton - [x] forwards - [x] backwards - [x] add
+some tests and benchmark for triton vs plain pytorch coor_descent - 10x faster
+for forward, 4x faster for backwards and memory saved is n_iters times - [x]
+fall back on plain coordinate descent for cpu - [x] handle edge case for when a
+row is completely masked out for triton, or simply enforce it never to be so -
+[x] fix masking in coordinate descent - [x] simplified some logic within the
+triton kernel and the problem went away. probably some tiny quirk with the
+compiler - [x] maximum block size in triton allowed is 131k, make sure at least
+quarter of million sequence length can be reached. to get around this
+initially, one can fold a million token sequence into ~9 131k and uniformly
+route. offer uniform routing scheme within router itself - [x] remove sinkhorn
 and cumulative softmax approaches and cleanup; neither can work as well as
-coordinate descent ## Citations ```bibtex @inproceedings{Ainslie2023CoLT5FL,
-title = {CoLT5: Faster Long-Range Transformers with Conditional Computation},
-author = {Joshua Ainslie and Tao Lei and Michiel de Jong and Santiago Ontan'on
-and Siddhartha Brahma and Yury Zemlyanskiy and David Uthus and Mandy Guo and
-James Lee-Thorp and Yi Tay and Yun-Hsuan Sung and Sumit Sanghai}, year = {2023}
-} ``` ```bibtex @article{Tillet2019TritonAI, title = {Triton: an intermediate
-language and compiler for tiled neural network computations}, author =
-{Philippe Tillet and H. Kung and D. Cox}, journal = {Proceedings of the 3rd ACM
-SIGPLAN International Workshop on Machine Learning and Programming Languages},
-year = {2019} } ``` ```bibtex @inproceedings{dao2022flashattention, title =
-{Flash{A}ttention: Fast and Memory-Efficient Exact Attention with {IO}-
-Awareness}, author = {Dao, Tri and Fu, Daniel Y. and Ermon, Stefano and Rudra,
-Atri and R{\'e}, Christopher}, booktitle = {Advances in Neural Information
-Processing Systems}, year = {2022} } ```
+coordinate descent - [ ] allow for saving intermediates every number of
+iterations - trading memory for recompute efficiency during backwards ##
+Citations ```bibtex @inproceedings{Ainslie2023CoLT5FL, title = {CoLT5: Faster
+Long-Range Transformers with Conditional Computation}, author = {Joshua Ainslie
+and Tao Lei and Michiel de Jong and Santiago Ontan'on and Siddhartha Brahma and
+Yury Zemlyanskiy and David Uthus and Mandy Guo and James Lee-Thorp and Yi Tay
+and Yun-Hsuan Sung and Sumit Sanghai}, year = {2023} } ``` ```bibtex @article
+{Tillet2019TritonAI, title = {Triton: an intermediate language and compiler for
+tiled neural network computations}, author = {Philippe Tillet and H. Kung and
+D. Cox}, journal = {Proceedings of the 3rd ACM SIGPLAN International Workshop
+on Machine Learning and Programming Languages}, year = {2019} } ``` ```bibtex
+@inproceedings{dao2022flashattention, title = {Flash{A}ttention: Fast and
+Memory-Efficient Exact Attention with {IO}-Awareness}, author = {Dao, Tri and
+Fu, Daniel Y. and Ermon, Stefano and Rudra, Atri and R{\'e}, Christopher},
+booktitle = {Advances in Neural Information Processing Systems}, year = {2022}
+} ```
```

### Comparing `CoLT5-attention-0.5.4/colt5_attention/attend.py` & `CoLT5-attention-0.5.5/colt5_attention/attend.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.5.4/colt5_attention/coor_descent.py` & `CoLT5-attention-0.5.5/colt5_attention/coor_descent.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.5.4/colt5_attention/transformer_block.py` & `CoLT5-attention-0.5.5/colt5_attention/transformer_block.py`

 * *Files 11% similar despite different names*

```diff
@@ -189,177 +189,14 @@
         # merge heads
 
         out = rearrange(out, 'b h n d -> b n (h d)')
         return self.to_out(out)
 
 # routing related logic
 
-class DifferentiableTopKRouter(nn.Module):
-    """ differentiable topk using cumulative softmax """
-
-    def __init__(
-        self,
-        dim,
-        straight_through = True,
-        temperature = 1.,
-        num_routing_tokens = 1
-    ):
-        super().__init__()
-        self.is_one_routing_token = num_routing_tokens == 1
-        self.num_routing_tokens = num_routing_tokens
-        self.routing_token = nn.Parameter(torch.randn(num_routing_tokens, dim))
-
-        self.straight_through = straight_through
-        self.temperature = temperature
-
-    def route_back(self, src, routed_tokens, indices):
-        batch_range = create_batch_range(routed_tokens)
-        src[batch_range, indices] = routed_tokens
-        return src
-
-    def forward(
-        self,
-        x,
-        *,
-        num_tokens,
-        mask = None
-    ):
-        num_routes = self.num_routing_tokens
-
-        # eventual normalized score
-
-        scores = einsum('b n d, r d -> b r n', x, self.routing_token)
-
-        # merge routing dimension into batch
-
-        x = repeat(x, 'b ... -> (b r) ...', r = num_routes)
-        scores, ps = pack_one(scores, '* n')
-
-        if exists(mask):
-            mask = repeat(mask, 'b ... -> (b r) ...', r = num_routes)
-
-        scores = scores / self.temperature
-
-        if exists(mask):
-            mask_value = -torch.finfo(scores.dtype).max
-            scores = scores.masked_fill(~mask, mask_value)
-
-        scores, indices = scores.sort(dim = -1)
-
-        scores = scores - scores.amax(dim = -1, keepdim = True).detach()
-
-        exp_scores = scores.exp()
-
-        cum_softmax = exp_scores / exp_scores.cumsum(dim = -1).clamp(min = 1e-6)
-
-        selected_scores, selected_indices = map(lambda t: t[:, -num_tokens:], (cum_softmax, indices))
-
-        if self.straight_through:
-            # this would make sure all normalized scores returned are 1., but still differentiable using straight-through trick
-            selected_scores = selected_scores + (1. - selected_scores).detach()
-
-            if exists(mask):
-                selected_mask = batched_gather(mask, selected_indices)
-                selected_scores = selected_scores.masked_fill(~selected_mask, 0.)
-
-        # split out routing dimension again if need be
-
-        if not self.is_one_routing_token:
-            selected_scores = unpack_one(selected_scores, ps, '* n')
-            selected_indices = unpack_one(selected_indices, ps, '* n')
-
-        return selected_scores, selected_indices
-
-# sinkhorn type routing, with ties to optimal transport
-
-from colt5_attention.sinkhorn import gumbel_sinkhorn, scatter_mean, log
-
-class SinkhornRouter(nn.Module):
-    """ gumbel sinkhorn router """
-    """ ex. https://arxiv.org/abs/1910.09036 """
-
-    def __init__(
-        self,
-        dim,
-        straight_through = True,
-        n_iters = 8,
-        temperature = 0.7,
-        num_routing_tokens = 1
-    ):
-        super().__init__()
-        self.is_one_routing_token = num_routing_tokens == 1
-        self.num_routing_tokens = num_routing_tokens
-        self.routing_token = nn.Parameter(torch.randn(num_routing_tokens, dim))
-
-        self.straight_through = straight_through
-        self.gumbel_sinkhorn_fn = partial(gumbel_sinkhorn, temperature = temperature, n_iters = n_iters)
-
-    def route_back(self, src, routed_tokens, indices):
-        return scatter_mean(src, routed_tokens, indices, dim = 1)
-
-    def forward(
-        self,
-        x,
-        *,
-        num_tokens,
-        mask = None
-    ):
-        n, num_routes = x.shape[-2], self.num_routing_tokens
-        num_tokens = min(n, num_tokens)
-
-        # eventual normalized score
-
-        scores = einsum('b n d, r d -> b r n', x, self.routing_token)
-
-        # merge routing dimension into batch
-
-        x = repeat(x, 'b ... -> (b r) ...', r = num_routes)
-        scores, ps = pack_one(scores, '* n')
-
-        if exists(mask):
-            mask = repeat(mask, 'b ... -> (b r) ...', r = num_routes)
-
-        # calculate scores
-
-        scores = repeat(scores, '... j -> ... i j', i = num_tokens)
-
-        if exists(mask):
-            mask_value = -torch.finfo(scores.dtype).max
-            sinkhorn_mask = rearrange(mask, 'b j -> b 1 j')
-            scores = scores.masked_fill(~sinkhorn_mask, mask_value)
-
-        # sinkhorn
-
-        scores = self.gumbel_sinkhorn_fn(scores)
-
-        # mask again just in case
-
-        if exists(mask):
-            scores = scores.masked_fill(~sinkhorn_mask, mask_value)
-
-        selected_scores, selected_indices = scores.topk(1, dim = -1)
-        selected_scores, selected_indices = map(lambda t: rearrange(t, '... 1 -> ...'), (selected_scores, selected_indices))
-
-        if self.straight_through:
-            # this would make sure all normalized scores returned are 1., but still differentiable using straight-through trick
-            selected_scores = selected_scores + (1. - selected_scores).detach()
-
-            if exists(mask):
-                selected_mask = batched_gather(mask, selected_indices)
-
-                selected_scores = selected_scores.masked_fill(~selected_mask, 0.)
-
-        # split out routing dimension again if need be
-
-        if not self.is_one_routing_token:
-            selected_scores = unpack_one(selected_scores, ps, '* n')
-            selected_indices = unpack_one(selected_indices, ps, '* n')
-
-        return selected_scores, selected_indices
-
 from colt5_attention.coor_descent import coor_descent
 
 class CoordinateDescentRouter(nn.Module):
     """
     from Wright et al. https://arxiv.org/abs/1502.04759
     then adopted by https://arxiv.org/abs/2211.01267 for multi-vector document retrieval by Qian et al
     finally, used successfully by this paper for routing to heavy branch attention / feedforward
@@ -486,50 +323,35 @@
 
             indices_offset = torch.arange(num_blocks, device = device) * route_block_size
             selected_indices = selected_indices + rearrange(indices_offset, 'n -> n 1')
             selected_indices = rearrange(selected_indices, 'b ... n w -> b ... (n w)')
 
         return selected_scores, selected_indices
 
-# all router types
-
-ROUTERS = dict(
-    cum_softmax = DifferentiableTopKRouter,
-    sinkhorn = SinkhornRouter,
-    coor_descent = CoordinateDescentRouter
-)
-
 # main classes
 
 class ConditionalRoutedFeedForward(nn.Module):
     def __init__(
         self,
         dim,
         *,
         num_heavy_tokens,
         light_ff_mult = 0.5,
         heavy_ff_mult = 4,
         router_straight_through = True, # would make sure all normalized scores are 1., still differentiable
-        router_type = 'coor_descent',
         router_kwargs: dict = {},
         use_triton = False
     ):
         super().__init__()
-        assert router_type in ROUTERS.keys()
-
         self.num_heavy_tokens = num_heavy_tokens
 
-        self.router_type = router_type
-
-        router_klass = ROUTERS.get(router_type)
-
-        if router_type == 'coor_descent' and use_triton:
+        if use_triton:
             router_kwargs = {**router_kwargs, 'use_triton': True}
 
-        self.router = router_klass(
+        self.router = CoordinateDescentRouter(
             dim = dim,
             straight_through = router_straight_through,
             **router_kwargs
         )
 
         self.light_ff = FeedForward(dim, light_ff_mult)
         self.heavy_ff = FeedForward(dim, heavy_ff_mult)
@@ -578,30 +400,24 @@
         num_routed_kv = 1,
         light_dim_head = 64,
         light_heads = 8,
         light_window_size = 128,        # each token would see ~ 64 tokens either way to left or right
         heavy_dim_head = 64,
         heavy_heads = 8,
         router_straight_through = True, # would make sure all normalized scores are 1., still differentiable
-        router_type = 'coor_descent',
         router_kwargs: dict = {},
         multiply_keys_by_score = False,
         multiply_queries_by_score = False,
         use_triton = False,
         use_null_q_tokens = True,
         use_flash_attn = False
     ):
         super().__init__()
-        assert router_type in ROUTERS.keys()
-
-        self.router_type = router_type
 
-        router_klass = ROUTERS.get(router_type)
-
-        if router_type == 'coor_descent' and use_triton:
+        if use_triton:
             router_kwargs = {**router_kwargs, 'use_triton': True}
 
         self.num_heavy_tokens_q = num_heavy_tokens_q
         self.num_heavy_tokens_kv = num_heavy_tokens_kv
 
         self.multiply_queries_by_score = multiply_queries_by_score
 
@@ -617,21 +433,21 @@
             look_forward = 1
         )
 
         self.null_q_token = None
         if use_null_q_tokens:
             self.null_q_token = nn.Parameter(torch.randn(dim)) # for the query tokens not selected by the router, give it a learned output embed
 
-        self.q_router = router_klass(
+        self.q_router = CoordinateDescentRouter(
             dim = dim,
             straight_through = router_straight_through,
             **router_kwargs
         )
 
-        self.kv_router = router_klass(
+        self.kv_router = CoordinateDescentRouter(
             dim = dim,
             num_routing_tokens = num_routed_kv,
             straight_through = router_straight_through,
             **router_kwargs
         )
 
         self.heavy_attn = Attention(
@@ -717,30 +533,24 @@
         light_dim_head = 64,
         light_heads = 8,
         light_window_size = 128,        # each token would see ~ 64 tokens either way to left or right
         heavy_window_size = None,
         heavy_dim_head = 64,
         heavy_heads = 8,
         router_straight_through = True, # would make sure all normalized scores are 1., still differentiable
-        router_type = 'coor_descent',
         router_kwargs: dict = {},
         multiply_keys_by_score = False,
         multiply_queries_by_score = False,
         use_triton = False,
         use_null_q_tokens = True,
         use_flash_attn = False
     ):
         super().__init__()
-        assert router_type in ROUTERS.keys()
-
-        self.router_type = router_type
-
-        router_klass = ROUTERS.get(router_type)
 
-        if router_type == 'coor_descent' and use_triton:
+        if use_triton:
             router_kwargs = {**router_kwargs, 'use_triton': True}
 
         self.num_heavy_tokens_q = num_heavy_tokens_q
         self.num_heavy_tokens_kv = num_heavy_tokens_kv
 
         self.multiply_queries_by_score = multiply_queries_by_score
 
@@ -757,21 +567,21 @@
             use_rotary_pos_emb = False
         )
 
         self.null_q_token = None
         if use_null_q_tokens:
             self.null_q_token = nn.Parameter(torch.randn(dim)) # for the query tokens not selected by the router, give it a learned output embed
 
-        self.q_router = router_klass(
+        self.q_router = CoordinateDescentRouter(
             dim = dim,
             straight_through = router_straight_through,
             **router_kwargs
         )
 
-        self.kv_router = router_klass(
+        self.kv_router = CoordinateDescentRouter(
             dim = dim,
             num_routing_tokens = num_routed_kv,
             straight_through = router_straight_through,
             **router_kwargs
         )
 
         self.heavy_attn = Attention(
@@ -902,47 +712,41 @@
         *,
         num_tokens_q,
         num_tokens_kv,
         num_sets_kv = 1,                # setting this greater than 1 would route multiple sets of key / values, each of size num_tokens_kv, using this many routing tokens
         dim_head = 64,
         heads = 8,
         router_straight_through = True, # would make sure all normalized scores are 1., still differentiable
-        router_type = 'coor_descent',
         router_kwargs: dict = {},
         kv_routing_tokens = 1,
         multiply_keys_by_score = False,
         use_triton = False,
         use_null_q_tokens = True,
         use_flash_attn = False,
         route_block_size = None
     ):
         super().__init__()
-        assert router_type in ROUTERS.keys()
-
-        self.router_type = router_type
 
-        router_klass = ROUTERS.get(router_type)
-
-        if router_type == 'coor_descent' and use_triton:
+        if use_triton:
             router_kwargs = {**router_kwargs, 'use_triton': True}
 
         self.num_tokens_q = num_tokens_q
         self.num_tokens_kv = num_tokens_kv
 
         self.null_q_token = None
         if use_null_q_tokens:
             self.null_q_token = nn.Parameter(torch.randn(dim)) # for the query tokens not selected by the router, give it a learned output embed
 
-        self.q_router = router_klass(
+        self.q_router = CoordinateDescentRouter(
             dim = dim,
             straight_through = router_straight_through,
             **router_kwargs
         )
 
-        self.kv_router = router_klass(
+        self.kv_router = CoordinateDescentRouter(
             dim = dim,
             straight_through = router_straight_through,
             num_routing_tokens = kv_routing_tokens,
             route_block_size = route_block_size,
             **router_kwargs
         )
 
@@ -1043,30 +847,28 @@
         light_heads = 8,
         light_window_size = 128,
         heavy_dim_head = 64,
         heavy_heads = 8,
         light_ff_mult = 0.5,
         heavy_ff_mult = 4,
         router_straight_through = True,
-        router_type = 'coor_descent',
         router_kwargs: dict = {},
         multiply_keys_by_score = False,
         multiply_queries_by_score = False,
         use_triton = False,
         use_null_q_tokens = True,
         use_flash_attn = False
     ):
         super().__init__()
         self.conditional_ff = ConditionalRoutedFeedForward(
             dim,
             num_heavy_tokens = num_heavy_ff_tokens,
             light_ff_mult = light_ff_mult,
             heavy_ff_mult = heavy_ff_mult,
             router_straight_through = router_straight_through,
-            router_type = router_type,
             router_kwargs = router_kwargs,
             use_triton = use_triton
         )
 
         self.conditional_attn = ConditionalRoutedAttention(
             dim,
             light_dim_head = light_dim_head,
@@ -1074,15 +876,14 @@
             light_window_size = light_window_size,
             heavy_dim_head = heavy_dim_head,
             heavy_heads = heavy_heads,
             num_heavy_tokens_q = num_heavy_attn_tokens_q,
             num_heavy_tokens_kv = num_heavy_attn_tokens_kv,
             num_routed_kv = num_routed_kv,
             router_straight_through = router_straight_through,
-            router_type = router_type,
             router_kwargs = router_kwargs,
             multiply_keys_by_score = multiply_keys_by_score,
             multiply_queries_by_score = multiply_queries_by_score,
             use_triton = use_triton,
             use_null_q_tokens = use_null_q_tokens,
             use_flash_attn = use_flash_attn
         )
```

### Comparing `CoLT5-attention-0.5.4/colt5_attention/triton_coor_descent.py` & `CoLT5-attention-0.5.5/colt5_attention/triton_coor_descent.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.5.4/setup.py` & `CoLT5-attention-0.5.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'CoLT5-attention',
   packages = find_packages(),
-  version = '0.5.4',
+  version = '0.5.5',
   license='MIT',
   description = 'Conditionally Routed Attention',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/CoLT5-attention',
   keywords = [
```

