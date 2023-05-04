# Comparing `tmp/auto_gptq-0.0.5.tar.gz` & `tmp/auto_gptq-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_gptq-0.0.5.tar", last modified: Wed Apr 26 10:01:56 2023, max compression
+gzip compressed data, was "auto_gptq-0.1.0.tar", last modified: Thu May  4 16:21:38 2023, max compression
```

## Comparing `auto_gptq-0.0.5.tar` & `auto_gptq-0.1.0.tar`

### file list

```diff
@@ -1,51 +1,56 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:01:56.646464 auto_gptq-0.0.5/
--rw-r--r--   0 root         (0) root         (0)     1075 2023-04-23 08:35:20.000000 auto_gptq-0.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)      120 2023-04-26 10:01:56.645464 auto_gptq-0.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9621 2023-04-26 09:57:15.000000 auto_gptq-0.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:01:56.641464 auto_gptq-0.0.5/auto_gptq/
--rw-r--r--   0 root         (0) root         (0)       83 2023-04-24 05:55:08.000000 auto_gptq-0.0.5/auto_gptq/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:01:56.642464 auto_gptq-0.0.5/auto_gptq/eval_tasks/
--rw-r--r--   0 root         (0) root         (0)      161 2023-04-24 05:55:08.000000 auto_gptq-0.0.5/auto_gptq/eval_tasks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2194 2023-04-24 05:55:08.000000 auto_gptq-0.0.5/auto_gptq/eval_tasks/_base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:01:56.642464 auto_gptq-0.0.5/auto_gptq/eval_tasks/_utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 05:55:08.000000 auto_gptq-0.0.5/auto_gptq/eval_tasks/_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1128 2023-04-24 05:55:08.000000 auto_gptq-0.0.5/auto_gptq/eval_tasks/_utils/classification_utils.py
--rw-r--r--   0 root         (0) root         (0)    11122 2023-04-24 05:55:08.000000 auto_gptq-0.0.5/auto_gptq/eval_tasks/_utils/data_utils.py
--rw-r--r--   0 root         (0) root         (0)     1448 2023-04-24 05:55:08.000000 auto_gptq-0.0.5/auto_gptq/eval_tasks/_utils/generation_utils.py
--rw-r--r--   0 root         (0) root         (0)     1215 2023-04-24 05:55:08.000000 auto_gptq-0.0.5/auto_gptq/eval_tasks/language_modeling_task.py
--rw-r--r--   0 root         (0) root         (0)     3653 2023-04-24 05:55:08.000000 auto_gptq-0.0.5/auto_gptq/eval_tasks/sequence_classification_task.py
--rw-r--r--   0 root         (0) root         (0)     2571 2023-04-24 05:55:08.000000 auto_gptq-0.0.5/auto_gptq/eval_tasks/text_summarization_task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:01:56.644464 auto_gptq-0.0.5/auto_gptq/modeling/
--rw-r--r--   0 root         (0) root         (0)      184 2023-04-24 05:55:08.000000 auto_gptq-0.0.5/auto_gptq/modeling/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15952 2023-04-26 09:57:15.000000 auto_gptq-0.0.5/auto_gptq/modeling/_base.py
--rw-r--r--   0 root         (0) root         (0)      402 2023-04-26 09:57:15.000000 auto_gptq-0.0.5/auto_gptq/modeling/_const.py
--rw-r--r--   0 root         (0) root         (0)     2819 2023-04-26 09:57:15.000000 auto_gptq-0.0.5/auto_gptq/modeling/_utils.py
--rw-r--r--   0 root         (0) root         (0)     2033 2023-04-26 09:57:15.000000 auto_gptq-0.0.5/auto_gptq/modeling/auto.py
--rw-r--r--   0 root         (0) root         (0)      444 2023-04-24 17:06:09.000000 auto_gptq-0.0.5/auto_gptq/modeling/bloom.py
--rw-r--r--   0 root         (0) root         (0)      429 2023-04-24 17:09:50.000000 auto_gptq-0.0.5/auto_gptq/modeling/gpt_neox.py
--rw-r--r--   0 root         (0) root         (0)      378 2023-04-23 08:35:20.000000 auto_gptq-0.0.5/auto_gptq/modeling/gptj.py
--rw-r--r--   0 root         (0) root         (0)      585 2023-04-23 08:35:20.000000 auto_gptq-0.0.5/auto_gptq/modeling/llama.py
--rw-r--r--   0 root         (0) root         (0)      334 2023-04-26 09:57:15.000000 auto_gptq-0.0.5/auto_gptq/modeling/moss.py
--rw-r--r--   0 root         (0) root         (0)      696 2023-04-23 08:35:20.000000 auto_gptq-0.0.5/auto_gptq/modeling/opt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:01:56.644464 auto_gptq-0.0.5/auto_gptq/nn_modules/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 09:57:15.000000 auto_gptq-0.0.5/auto_gptq/nn_modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9822 2023-04-26 09:57:15.000000 auto_gptq-0.0.5/auto_gptq/nn_modules/qlinear.py
--rw-r--r--   0 root         (0) root         (0)    18408 2023-04-26 09:57:15.000000 auto_gptq-0.0.5/auto_gptq/nn_modules/qlinear_triton.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:01:56.644464 auto_gptq-0.0.5/auto_gptq/nn_modules/triton_utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 09:57:15.000000 auto_gptq-0.0.5/auto_gptq/nn_modules/triton_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6925 2023-04-26 09:57:15.000000 auto_gptq-0.0.5/auto_gptq/nn_modules/triton_utils/custom_autotune.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:01:56.645464 auto_gptq-0.0.5/auto_gptq/quantization/
--rw-r--r--   0 root         (0) root         (0)       45 2023-04-26 09:57:15.000000 auto_gptq-0.0.5/auto_gptq/quantization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5813 2023-04-26 09:57:15.000000 auto_gptq-0.0.5/auto_gptq/quantization/gptq.py
--rw-r--r--   0 root         (0) root         (0)     4271 2023-04-26 09:57:15.000000 auto_gptq-0.0.5/auto_gptq/quantization/quantizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:01:56.641464 auto_gptq-0.0.5/auto_gptq.egg-info/
--rw-r--r--   0 root         (0) root         (0)      120 2023-04-26 10:01:56.000000 auto_gptq-0.0.5/auto_gptq.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1279 2023-04-26 10:01:56.000000 auto_gptq-0.0.5/auto_gptq.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 10:01:56.000000 auto_gptq-0.0.5/auto_gptq.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      122 2023-04-26 10:01:56.000000 auto_gptq-0.0.5/auto_gptq.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-26 10:01:56.000000 auto_gptq-0.0.5/auto_gptq.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:01:56.645464 auto_gptq-0.0.5/quant_cuda/
--rw-r--r--   0 root         (0) root         (0)     2287 2023-04-26 09:57:15.000000 auto_gptq-0.0.5/quant_cuda/quant_cuda.cpp
--rw-r--r--   0 root         (0) root         (0)    12817 2023-04-26 09:57:15.000000 auto_gptq-0.0.5/quant_cuda/quant_cuda_kernel.cu
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 10:01:56.646464 auto_gptq-0.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1436 2023-04-26 10:00:09.000000 auto_gptq-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 16:21:38.589723 auto_gptq-0.1.0/
+-rw-rw-rw-   0        0        0     1096 2023-04-13 14:32:51.000000 auto_gptq-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      126 2023-05-04 16:21:38.589723 auto_gptq-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9775 2023-05-04 16:15:32.000000 auto_gptq-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 16:21:38.489776 auto_gptq-0.1.0/auto_gptq/
+-rw-rw-rw-   0        0        0       85 2023-04-23 15:46:04.000000 auto_gptq-0.1.0/auto_gptq/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 16:21:38.514701 auto_gptq-0.1.0/auto_gptq/eval_tasks/
+-rw-rw-rw-   0        0        0      124 2023-04-28 14:56:43.000000 auto_gptq-0.1.0/auto_gptq/eval_tasks/__init__.py
+-rw-rw-rw-   0        0        0     2259 2023-04-28 14:56:43.000000 auto_gptq-0.1.0/auto_gptq/eval_tasks/_base.py
+drwxrwxrwx   0        0        0        0 2023-05-04 16:21:38.519734 auto_gptq-0.1.0/auto_gptq/eval_tasks/_utils/
+-rw-rw-rw-   0        0        0        0 2023-04-23 15:46:04.000000 auto_gptq-0.1.0/auto_gptq/eval_tasks/_utils/__init__.py
+-rw-rw-rw-   0        0        0     1165 2023-04-23 15:46:04.000000 auto_gptq-0.1.0/auto_gptq/eval_tasks/_utils/classification_utils.py
+-rw-rw-rw-   0        0        0     1486 2023-04-23 15:46:04.000000 auto_gptq-0.1.0/auto_gptq/eval_tasks/_utils/generation_utils.py
+-rw-rw-rw-   0        0        0     1262 2023-04-23 15:46:04.000000 auto_gptq-0.1.0/auto_gptq/eval_tasks/language_modeling_task.py
+-rw-rw-rw-   0        0        0     3760 2023-04-23 15:46:04.000000 auto_gptq-0.1.0/auto_gptq/eval_tasks/sequence_classification_task.py
+-rw-rw-rw-   0        0        0     2646 2023-04-24 12:51:09.000000 auto_gptq-0.1.0/auto_gptq/eval_tasks/text_summarization_task.py
+drwxrwxrwx   0        0        0        0 2023-05-04 16:21:38.534543 auto_gptq-0.1.0/auto_gptq/modeling/
+-rw-rw-rw-   0        0        0      233 2023-04-28 14:56:43.000000 auto_gptq-0.1.0/auto_gptq/modeling/__init__.py
+-rw-rw-rw-   0        0        0    23514 2023-05-04 13:51:26.000000 auto_gptq-0.1.0/auto_gptq/modeling/_base.py
+-rw-rw-rw-   0        0        0      427 2023-04-28 14:56:43.000000 auto_gptq-0.1.0/auto_gptq/modeling/_const.py
+-rw-rw-rw-   0        0        0     4720 2023-05-04 14:09:44.000000 auto_gptq-0.1.0/auto_gptq/modeling/_utils.py
+-rw-rw-rw-   0        0        0     2677 2023-04-29 12:44:45.000000 auto_gptq-0.1.0/auto_gptq/modeling/auto.py
+-rw-rw-rw-   0        0        0      490 2023-04-28 14:56:43.000000 auto_gptq-0.1.0/auto_gptq/modeling/bloom.py
+-rw-rw-rw-   0        0        0      409 2023-04-28 14:56:43.000000 auto_gptq-0.1.0/auto_gptq/modeling/gpt2.py
+-rw-rw-rw-   0        0        0      478 2023-04-28 14:56:43.000000 auto_gptq-0.1.0/auto_gptq/modeling/gpt_neox.py
+-rw-rw-rw-   0        0        0      423 2023-04-28 14:56:43.000000 auto_gptq-0.1.0/auto_gptq/modeling/gptj.py
+-rw-rw-rw-   0        0        0      469 2023-04-28 15:06:27.000000 auto_gptq-0.1.0/auto_gptq/modeling/llama.py
+-rw-rw-rw-   0        0        0      395 2023-04-29 02:36:14.000000 auto_gptq-0.1.0/auto_gptq/modeling/moss.py
+-rw-rw-rw-   0        0        0      581 2023-04-28 15:06:27.000000 auto_gptq-0.1.0/auto_gptq/modeling/opt.py
+drwxrwxrwx   0        0        0        0 2023-05-04 16:21:38.553323 auto_gptq-0.1.0/auto_gptq/nn_modules/
+-rw-rw-rw-   0        0        0        0 2023-04-26 13:22:55.000000 auto_gptq-0.1.0/auto_gptq/nn_modules/__init__.py
+-rw-rw-rw-   0        0        0     9254 2023-04-30 12:35:15.000000 auto_gptq-0.1.0/auto_gptq/nn_modules/layernorm_triton.py
+-rw-rw-rw-   0        0        0    10285 2023-05-04 14:09:44.000000 auto_gptq-0.1.0/auto_gptq/nn_modules/qlinear.py
+-rw-rw-rw-   0        0        0    11608 2023-05-04 14:16:08.000000 auto_gptq-0.1.0/auto_gptq/nn_modules/qlinear_old.py
+-rw-rw-rw-   0        0        0    19259 2023-04-28 14:56:43.000000 auto_gptq-0.1.0/auto_gptq/nn_modules/qlinear_triton.py
+drwxrwxrwx   0        0        0        0 2023-05-04 16:21:38.559832 auto_gptq-0.1.0/auto_gptq/nn_modules/triton_utils/
+-rw-rw-rw-   0        0        0        0 2023-04-26 13:22:55.000000 auto_gptq-0.1.0/auto_gptq/nn_modules/triton_utils/__init__.py
+-rw-rw-rw-   0        0        0     7099 2023-04-26 13:22:55.000000 auto_gptq-0.1.0/auto_gptq/nn_modules/triton_utils/custom_autotune.py
+drwxrwxrwx   0        0        0        0 2023-05-04 16:21:38.589723 auto_gptq-0.1.0/auto_gptq/quantization/
+-rw-rw-rw-   0        0        0       47 2023-04-26 13:22:55.000000 auto_gptq-0.1.0/auto_gptq/quantization/__init__.py
+-rw-rw-rw-   0        0        0     6007 2023-04-28 14:56:43.000000 auto_gptq-0.1.0/auto_gptq/quantization/gptq.py
+-rw-rw-rw-   0        0        0     4408 2023-04-26 13:22:55.000000 auto_gptq-0.1.0/auto_gptq/quantization/quantizer.py
+drwxrwxrwx   0        0        0        0 2023-05-04 16:21:38.589723 auto_gptq-0.1.0/auto_gptq/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-28 14:56:43.000000 auto_gptq-0.1.0/auto_gptq/utils/__init__.py
+-rw-rw-rw-   0        0        0    11389 2023-04-28 14:56:43.000000 auto_gptq-0.1.0/auto_gptq/utils/data_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-04 16:21:38.499744 auto_gptq-0.1.0/auto_gptq.egg-info/
+-rw-rw-rw-   0        0        0      126 2023-05-04 16:21:38.000000 auto_gptq-0.1.0/auto_gptq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1399 2023-05-04 16:21:38.000000 auto_gptq-0.1.0/auto_gptq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 16:21:38.000000 auto_gptq-0.1.0/auto_gptq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      141 2023-05-04 16:21:38.000000 auto_gptq-0.1.0/auto_gptq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-04 16:21:38.000000 auto_gptq-0.1.0/auto_gptq.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 16:21:38.589723 auto_gptq-0.1.0/quant_cuda/
+-rw-rw-rw-   0        0        0     6642 2023-05-04 13:51:26.000000 auto_gptq-0.1.0/quant_cuda/quant_cuda.cpp
+-rw-rw-rw-   0        0        0    40650 2023-05-04 14:33:51.000000 auto_gptq-0.1.0/quant_cuda/quant_cuda_kernel.cu
+-rw-rw-rw-   0        0        0       42 2023-05-04 16:21:38.589723 auto_gptq-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1599 2023-05-04 16:18:50.000000 auto_gptq-0.1.0/setup.py
```

### Comparing `auto_gptq-0.0.5/LICENSE` & `auto_gptq-0.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 潘其威(William)
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 潘其威(William)
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `auto_gptq-0.0.5/README.md` & `auto_gptq-0.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,602 +1,611 @@
-00000000: 2320 4175 746f 4750 5451 0a41 6e20 6561  # AutoGPTQ.An ea
-00000010: 7379 2d74 6f2d 7573 6520 6d6f 6465 6c20  sy-to-use model 
-00000020: 7175 616e 7469 7a61 7469 6f6e 2070 6163  quantization pac
-00000030: 6b61 6765 2077 6974 6820 7573 6572 2d66  kage with user-f
-00000040: 7269 656e 646c 7920 6170 6973 2c20 6261  riendly apis, ba
-00000050: 7365 6420 6f6e 2047 5054 5120 616c 676f  sed on GPTQ algo
-00000060: 7269 7468 6d2e 0a0a 2323 204e 6577 7320  rithm...## News 
-00000070: 6f72 2055 7064 6174 650a 2d20 3230 3233  or Update.- 2023
-00000080: 2d30 342d 3236 202d 2028 5570 6461 7465  -04-26 - (Update
-00000090: 2920 2d20 5573 696e 6720 6074 7269 746f  ) - Using `trito
-000000a0: 6e60 2074 6f20 7370 6565 6420 7570 2069  n` to speed up i
-000000b0: 6e66 6572 656e 6365 2069 7320 6e6f 7720  nference is now 
-000000c0: 7375 7070 6f72 7465 642e 0a2d 2032 3032  supported..- 202
-000000d0: 332d 3034 2d32 3520 2d20 284e 6577 7326  3-04-25 - (News&
-000000e0: 5570 6461 7465 2920 2d20 5b4d 4f53 535d  Update) - [MOSS]
-000000f0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000100: 636f 6d2f 4f70 656e 4c4d 4c61 622f 4d4f  com/OpenLMLab/MO
-00000110: 5353 2920 6973 2061 6e20 6f70 656e 2d73  SS) is an open-s
-00000120: 6f75 7263 6520 746f 6f6c 2d61 7567 6d65  ource tool-augme
-00000130: 6e74 6564 2063 6f6e 7665 7273 6174 696f  nted conversatio
-00000140: 6e61 6c20 6c61 6e67 7561 6765 206d 6f64  nal language mod
-00000150: 656c 2066 726f 6d20 4675 6461 6e20 556e  el from Fudan Un
-00000160: 6976 6572 7369 7479 2c20 7175 616e 7469  iversity, quanti
-00000170: 7a61 7469 6f6e 2069 7320 6e6f 7720 7375  zation is now su
-00000180: 7070 6f72 7465 6420 696e 2041 7574 6f47  pported in AutoG
-00000190: 5054 512e 0a2d 2032 3032 332d 3034 2d32  PTQ..- 2023-04-2
-000001a0: 3320 2d20 2855 7064 6174 6529 202d 2053  3 - (Update) - S
-000001b0: 7570 706f 7274 2065 7661 6c75 6174 696f  upport evaluatio
-000001c0: 6e20 6f6e 206d 756c 7469 706c 6520 2864  n on multiple (d
-000001d0: 6f77 6e2d 7374 7265 616d 2920 7461 736b  own-stream) task
-000001e0: 7320 7375 6368 2061 733a 206c 616e 6775  s such as: langu
-000001f0: 6167 652d 6d6f 6465 6c69 6e67 2c20 7465  age-modeling, te
-00000200: 7874 2d63 6c61 7373 6966 6963 6174 696f  xt-classificatio
-00000210: 6e2c 2074 6578 742d 7375 6d6d 6172 697a  n, text-summariz
-00000220: 6174 696f 6e2e 0a2d 2032 3032 332d 3034  ation..- 2023-04
-00000230: 2d32 3220 2d20 284e 6577 7329 202d 2071  -22 - (News) - q
-00000240: 776f 7071 776f 7032 3030 2773 205b 4175  wopqwop200's [Au
-00000250: 746f 4750 5451 2d74 7269 746f 6e5d 2868  toGPTQ-triton](h
-00000260: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000270: 6d2f 7177 6f70 7177 6f70 3230 302f 4175  m/qwopqwop200/Au
-00000280: 746f 4750 5451 2d74 7269 746f 6e29 2070  toGPTQ-triton) p
-00000290: 726f 7669 6465 7320 6661 7374 6572 2073  rovides faster s
-000002a0: 7065 6564 2074 6f20 696e 7465 6772 6174  peed to integrat
-000002b0: 6520 7769 7468 2071 7561 6e74 697a 6564  e with quantized
-000002c0: 206d 6f64 656c 2c20 666f 7220 6576 6572   model, for ever
-000002d0: 796f 6e65 2077 686f 2063 616e 2061 6363  yone who can acc
-000002e0: 6573 7320 746f 2074 7269 746f 6e2c 2074  ess to triton, t
-000002f0: 7279 2061 6e64 2065 6e6a 6f79 2079 6f75  ry and enjoy you
-00000300: 7273 656c 6621 0a2d 2032 3032 332d 3034  rself!.- 2023-04
-00000310: 2d32 3020 2d20 284e 6577 7329 202d 2041  -20 - (News) - A
-00000320: 7574 6f47 5054 5120 6973 2061 7574 6f6d  utoGPTQ is autom
-00000330: 6174 6963 616c 6c79 2063 6f6d 7061 7469  atically compati
-00000340: 626c 6520 7769 7468 2053 7461 6269 6c69  ble with Stabili
-00000350: 7479 2d41 4927 7320 6e65 776c 7920 7265  ty-AI's newly re
-00000360: 6c65 6173 6564 2060 6770 745f 6e65 6f78  leased `gpt_neox
-00000370: 6020 7479 7065 206d 6f64 656c 2066 616d  ` type model fam
-00000380: 696c 7920 5b53 7461 626c 654c 4d5d 2868  ily [StableLM](h
-00000390: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000003a0: 6d2f 5374 6162 696c 6974 792d 4149 2f53  m/Stability-AI/S
-000003b0: 7461 626c 654c 4d29 2e0a 2d20 3230 3233  tableLM)..- 2023
-000003c0: 2d30 342d 3136 202d 2028 5570 6461 7465  -04-16 - (Update
-000003d0: 2920 2d20 5375 7070 6f72 7420 7175 616e  ) - Support quan
-000003e0: 7469 7a61 7469 6f6e 2061 6e64 2069 6e66  tization and inf
-000003f0: 6572 656e 6365 2066 6f72 2060 626c 6f6f  erence for `bloo
-00000400: 6d60 2c20 6067 7074 5f6e 656f 7860 2c20  m`, `gpt_neox`, 
-00000410: 6067 7074 6a60 2c20 606c 6c61 6d61 6020  `gptj`, `llama` 
-00000420: 616e 6420 606f 7074 602e 0a0a 2323 2049  and `opt`...## I
-00000430: 6e73 7461 6c6c 6174 696f 6e0a 0a23 2323  nstallation..###
-00000440: 2051 7569 636b 2049 6e73 7461 6c6c 6174   Quick Installat
-00000450: 696f 6e0a 596f 7520 6361 6e20 696e 7374  ion.You can inst
-00000460: 616c 6c20 7468 6520 6c61 7465 7374 2073  all the latest s
-00000470: 7461 626c 6520 7265 6c65 6173 6520 6f66  table release of
-00000480: 2041 7574 6f47 5054 5120 6672 6f6d 2070   AutoGPTQ from p
-00000490: 6970 3a0a 6060 6073 6865 6c6c 0a70 6970  ip:.```shell.pip
-000004a0: 2069 6e73 7461 6c6c 2061 7574 6f2d 6770   install auto-gp
-000004b0: 7471 0a60 6060 0a42 7920 6465 6661 756c  tq.```.By defaul
-000004c0: 742c 2070 7974 6f72 6368 2065 7874 656e  t, pytorch exten
-000004d0: 7369 6f6e 7320 7769 6c6c 2062 6520 696e  sions will be in
-000004e0: 7374 616c 6c65 6420 7768 656e 2060 746f  stalled when `to
-000004f0: 7263 6860 2069 7320 616c 7265 6164 7920  rch` is already 
-00000500: 696e 2079 6f75 7220 7669 7274 7561 6c20  in your virtual 
-00000510: 656e 7669 726f 6e6d 656e 742c 2069 6620  environment, if 
-00000520: 796f 7520 646f 6e27 7420 7761 6e74 2074  you don't want t
-00000530: 6f20 7573 6520 6375 6461 2065 7874 656e  o use cuda exten
-00000540: 7369 6f6e 732c 2075 7369 6e67 3a0a 6060  sions, using:.``
-00000550: 6073 6865 6c6c 0a42 5549 4c44 5f43 5544  `shell.BUILD_CUD
-00000560: 415f 4558 543d 3020 7069 7020 696e 7374  A_EXT=0 pip inst
-00000570: 616c 6c20 6175 746f 2d67 7074 710a 6060  all auto-gptq.``
-00000580: 600a 466f 7220 736f 6d65 2070 656f 706c  `.For some peopl
-00000590: 6520 7761 6e74 2074 6f20 7472 7920 4c4c  e want to try LL
-000005a0: 614d 6120 616e 6420 7768 6f73 6520 6074  aMa and whose `t
-000005b0: 7261 6e73 666f 726d 6572 7360 2076 6572  ransformers` ver
-000005c0: 7369 6f6e 206e 6f74 206d 6565 7420 7468  sion not meet th
-000005d0: 6520 6e65 7765 7374 206f 6e65 2074 6861  e newest one tha
-000005e0: 7420 7375 7070 6f72 7473 2069 742c 2075  t supports it, u
-000005f0: 7369 6e67 3a0a 6060 6073 6865 6c6c 0a70  sing:.```shell.p
-00000600: 6970 2069 6e73 7461 6c6c 2061 7574 6f2d  ip install auto-
-00000610: 6770 7471 5b6c 6c61 6d61 5d0a 6060 600a  gptq[llama].```.
-00000620: 546f 2069 6e74 6567 7261 7465 2077 6974  To integrate wit
-00000630: 6820 6074 7269 746f 6e60 2c20 7573 696e  h `triton`, usin
-00000640: 673a 0a3e 2077 6172 6e69 6e67 3a20 332d  g:.> warning: 3-
-00000650: 6269 7420 7175 616e 7469 7a61 7469 6f6e  bit quantization
-00000660: 2069 7320 6e6f 7420 7375 7070 6f72 7465   is not supporte
-00000670: 6420 7768 656e 2075 7369 6e67 2074 7269  d when using tri
-00000680: 746f 6e0a 0a60 6060 7368 656c 6c0a 7069  ton..```shell.pi
-00000690: 7020 696e 7374 616c 6c20 6175 746f 2d67  p install auto-g
-000006a0: 7074 715b 7472 6974 6f6e 5d0a 6060 600a  ptq[triton].```.
-000006b0: 0a23 2323 2049 6e73 7461 6c6c 2066 726f  .### Install fro
-000006c0: 6d20 736f 7572 6365 0a43 6c6f 6e65 2074  m source.Clone t
-000006d0: 6865 2073 6f75 7263 6520 636f 6465 3a0a  he source code:.
-000006e0: 6060 6073 6865 6c6c 0a67 6974 2063 6c6f  ```shell.git clo
-000006f0: 6e65 2068 7474 7073 3a2f 2f67 6974 6875  ne https://githu
-00000700: 622e 636f 6d2f 5061 6e51 6957 6569 2f41  b.com/PanQiWei/A
-00000710: 7574 6f47 5054 512e 6769 7420 2626 2063  utoGPTQ.git && c
-00000720: 6420 4175 746f 4750 5451 0a60 6060 0a54  d AutoGPTQ.```.T
-00000730: 6865 6e2c 2069 6e73 7461 6c6c 2066 726f  hen, install fro
-00000740: 6d20 736f 7572 6365 3a0a 6060 6073 6865  m source:.```she
-00000750: 6c6c 0a70 6970 2069 6e73 7461 6c6c 202e  ll.pip install .
-00000760: 0a60 6060 0a4c 696b 6520 7175 6963 6b20  .```.Like quick 
-00000770: 696e 7374 616c 6c61 7469 6f6e 2c20 796f  installation, yo
-00000780: 7520 6361 6e20 616c 736f 2073 6574 2060  u can also set `
-00000790: 4255 494c 445f 4355 4441 5f45 5854 3d30  BUILD_CUDA_EXT=0
-000007a0: 6020 746f 2064 6973 6162 6c65 2070 7974  ` to disable pyt
-000007b0: 6f72 6368 2065 7874 656e 7369 6f6e 2062  orch extension b
-000007c0: 7569 6c64 696e 672e 0a0a 5573 6520 602e  uilding...Use `.
-000007d0: 5b6c 6c61 6d61 5d60 2069 6620 796f 7520  [llama]` if you 
-000007e0: 7761 6e74 2074 6f20 7472 7920 4c4c 614d  want to try LLaM
-000007f0: 6120 6d6f 6465 6c2e 0a0a 5573 6520 602e  a model...Use `.
-00000800: 5b74 7269 746f 6e5d 6020 6966 2079 6f75  [triton]` if you
-00000810: 2077 616e 7420 746f 2069 6e74 6567 7261   want to integra
-00000820: 7465 2077 6974 6820 7472 6974 6f6e 2061  te with triton a
-00000830: 6e64 2069 7427 7320 6176 6169 6c61 626c  nd it's availabl
-00000840: 6520 6f6e 2079 6f75 7220 6f70 6572 6174  e on your operat
-00000850: 696e 6720 7379 7374 656d 2e0a 0a0a 2323  ing system....##
-00000860: 2053 7570 706f 7274 6564 204d 6f64 656c   Supported Model
-00000870: 730a 4375 7272 656e 746c 792c 2060 6175  s.Currently, `au
-00000880: 746f 5f67 7074 7160 2073 7570 706f 7274  to_gptq` support
-00000890: 733a 2060 626c 6f6f 6d60 2c20 6067 7074  s: `bloom`, `gpt
-000008a0: 5f6e 656f 7860 2c20 6067 7074 6a60 2c20  _neox`, `gptj`, 
-000008b0: 606c 6c61 6d61 602c 2060 6d6f 7373 6020  `llama`, `moss` 
-000008c0: 616e 6420 606f 7074 603b 206d 6f72 6520  and `opt`; more 
-000008d0: 4361 7573 616c 4c4d 7320 7769 6c6c 2063  CausalLMs will c
-000008e0: 6f6d 6520 736f 6f6e 210a 0a23 2320 5375  ome soon!..## Su
-000008f0: 7070 6f72 7465 6420 4576 616c 7561 7469  pported Evaluati
-00000900: 6f6e 2054 6173 6b73 0a43 7572 7265 6e74  on Tasks.Current
-00000910: 6c79 2c20 6061 7574 6f5f 6770 7471 6020  ly, `auto_gptq` 
-00000920: 7375 7070 6f72 7473 3a20 604c 616e 6775  supports: `Langu
-00000930: 6167 654d 6f64 656c 696e 6754 6173 6b60  ageModelingTask`
-00000940: 2c20 6053 6571 7565 6e63 6543 6c61 7373  , `SequenceClass
-00000950: 6966 6963 6174 696f 6e54 6173 6b60 2061  ificationTask` a
-00000960: 6e64 2060 5465 7874 5375 6d6d 6172 697a  nd `TextSummariz
-00000970: 6174 696f 6e54 6173 6b60 3b20 6d6f 7265  ationTask`; more
-00000980: 2054 6173 6b73 2077 696c 6c20 636f 6d65   Tasks will come
-00000990: 2073 6f6f 6e21 0a0a 2323 2055 7361 6765   soon!..## Usage
-000009a0: 0a0a 2323 2320 4261 7369 630a 3e20 7761  ..### Basic.> wa
-000009b0: 726e 696e 673a 2074 6869 7320 6973 206a  rning: this is j
-000009c0: 7573 7420 6120 7368 6f77 2063 6173 6520  ust a show case 
-000009d0: 6f66 2074 6865 2075 7361 6765 206f 6620  of the usage of 
-000009e0: 6261 7369 6320 6170 6973 2069 6e20 4175  basic apis in Au
-000009f0: 746f 4750 5451 2c20 7768 6963 6820 7573  toGPTQ, which us
-00000a00: 6573 206f 6e6c 7920 6f6e 6520 7361 6d70  es only one samp
-00000a10: 6c65 2074 6f20 7175 616e 7469 7a65 2061  le to quantize a
-00000a20: 206d 7563 6820 736d 616c 6c20 6d6f 6465   much small mode
-00000a30: 6c2c 2074 6875 7320 6d61 7920 6e6f 7420  l, thus may not 
-00000a40: 7065 7266 6f72 6d73 2061 7320 7765 6c6c  performs as well
-00000a50: 2061 7320 6578 7065 6374 6564 2069 6e20   as expected in 
-00000a60: 4c4c 4d73 2e0a 0a42 656c 6f77 2069 7320  LLMs...Below is 
-00000a70: 616e 2065 7861 6d70 6c65 2066 6f72 2074  an example for t
-00000a80: 6865 2073 696d 706c 6573 7420 7573 6520  he simplest use 
-00000a90: 6f66 2061 7574 6f5f 6770 7471 3a20 0a60  of auto_gptq: .`
-00000aa0: 6060 7079 7468 6f6e 0a66 726f 6d20 7472  ``python.from tr
-00000ab0: 616e 7366 6f72 6d65 7273 2069 6d70 6f72  ansformers impor
-00000ac0: 7420 4175 746f 546f 6b65 6e69 7a65 722c  t AutoTokenizer,
-00000ad0: 2054 6578 7447 656e 6572 6174 696f 6e50   TextGenerationP
-00000ae0: 6970 656c 696e 650a 6672 6f6d 2061 7574  ipeline.from aut
-00000af0: 6f5f 6770 7471 2069 6d70 6f72 7420 4175  o_gptq import Au
-00000b00: 746f 4750 5451 466f 7243 6175 7361 6c4c  toGPTQForCausalL
-00000b10: 4d2c 2042 6173 6551 7561 6e74 697a 6543  M, BaseQuantizeC
-00000b20: 6f6e 6669 670a 0a0a 7072 6574 7261 696e  onfig...pretrain
-00000b30: 6564 5f6d 6f64 656c 5f64 6972 203d 2022  ed_model_dir = "
-00000b40: 6661 6365 626f 6f6b 2f6f 7074 2d31 3235  facebook/opt-125
-00000b50: 6d22 0a71 7561 6e74 697a 6564 5f6d 6f64  m".quantized_mod
-00000b60: 656c 5f64 6972 203d 2022 6f70 742d 3132  el_dir = "opt-12
-00000b70: 356d 2d34 6269 7422 0a0a 0a74 6f6b 656e  5m-4bit"...token
-00000b80: 697a 6572 203d 2041 7574 6f54 6f6b 656e  izer = AutoToken
-00000b90: 697a 6572 2e66 726f 6d5f 7072 6574 7261  izer.from_pretra
-00000ba0: 696e 6564 2870 7265 7472 6169 6e65 645f  ined(pretrained_
-00000bb0: 6d6f 6465 6c5f 6469 722c 2075 7365 5f66  model_dir, use_f
-00000bc0: 6173 743d 5472 7565 290a 6578 616d 706c  ast=True).exampl
-00000bd0: 6520 3d20 746f 6b65 6e69 7a65 7228 0a20  e = tokenizer(. 
-00000be0: 2020 2022 6175 746f 5f67 7074 7120 6973     "auto_gptq is
-00000bf0: 2061 2075 7365 6675 6c20 746f 6f6c 2074   a useful tool t
-00000c00: 6861 7420 6361 6e20 6175 746f 6d61 7469  hat can automati
-00000c10: 6361 6c6c 7920 636f 6d70 7265 7373 206d  cally compress m
-00000c20: 6f64 656c 2069 6e74 6f20 342d 6269 7420  odel into 4-bit 
-00000c30: 6f72 2065 7665 6e20 6869 6768 6572 2072  or even higher r
-00000c40: 6174 6520 6279 2075 7369 6e67 2047 5054  ate by using GPT
-00000c50: 5120 616c 676f 7269 7468 6d2e 222c 0a20  Q algorithm.",. 
-00000c60: 2020 2072 6574 7572 6e5f 7465 6e73 6f72     return_tensor
-00000c70: 733d 2270 7422 0a29 0a0a 7175 616e 7469  s="pt".)..quanti
-00000c80: 7a65 5f63 6f6e 6669 6720 3d20 4261 7365  ze_config = Base
-00000c90: 5175 616e 7469 7a65 436f 6e66 6967 280a  QuantizeConfig(.
-00000ca0: 2020 2020 6269 7473 3d34 2c20 2023 2071      bits=4,  # q
-00000cb0: 7561 6e74 697a 6520 6d6f 6465 6c20 746f  uantize model to
-00000cc0: 2034 2d62 6974 0a20 2020 2067 726f 7570   4-bit.    group
-00000cd0: 5f73 697a 653d 3132 382c 2020 2320 6974  _size=128,  # it
-00000ce0: 2069 7320 7265 636f 6d6d 656e 6465 6420   is recommended 
-00000cf0: 746f 2073 6574 2074 6865 2076 616c 7565  to set the value
-00000d00: 2074 6f20 3132 380a 290a 0a23 206c 6f61   to 128.)..# loa
-00000d10: 6420 756e 2d71 7561 6e74 697a 6564 206d  d un-quantized m
-00000d20: 6f64 656c 2c20 7468 6520 6d6f 6465 6c20  odel, the model 
-00000d30: 7769 6c6c 2061 6c77 6179 7320 6265 2066  will always be f
-00000d40: 6f72 6365 206c 6f61 6465 6420 696e 746f  orce loaded into
-00000d50: 2063 7075 0a6d 6f64 656c 203d 2041 7574   cpu.model = Aut
-00000d60: 6f47 5054 5146 6f72 4361 7573 616c 4c4d  oGPTQForCausalLM
-00000d70: 2e66 726f 6d5f 7072 6574 7261 696e 6564  .from_pretrained
-00000d80: 2870 7265 7472 6169 6e65 645f 6d6f 6465  (pretrained_mode
-00000d90: 6c5f 6469 722c 2071 7561 6e74 697a 655f  l_dir, quantize_
-00000da0: 636f 6e66 6967 290a 0a23 2071 7561 6e74  config)..# quant
-00000db0: 697a 6520 6d6f 6465 6c2c 2074 6865 2065  ize model, the e
-00000dc0: 7861 6d70 6c65 7320 7368 6f75 6c64 2062  xamples should b
-00000dd0: 6520 6c69 7374 206f 6620 6469 6374 2077  e list of dict w
-00000de0: 686f 7365 206b 6579 7320 6361 6e20 6f6e  hose keys can on
-00000df0: 6c79 2062 6520 2269 6e70 7574 5f69 6473  ly be "input_ids
-00000e00: 2220 616e 6420 2261 7474 656e 7469 6f6e  " and "attention
-00000e10: 5f6d 6173 6b22 200a 2320 7769 7468 2076  _mask" .# with v
-00000e20: 616c 7565 2075 6e64 6572 2074 6f72 6368  alue under torch
-00000e30: 2e4c 6f6e 6754 656e 736f 7220 7479 7065  .LongTensor type
-00000e40: 2e0a 6d6f 6465 6c2e 7175 616e 7469 7a65  ..model.quantize
-00000e50: 285b 6578 616d 706c 655d 2c20 7573 655f  ([example], use_
-00000e60: 7472 6974 6f6e 3d46 616c 7365 290a 0a23  triton=False)..#
-00000e70: 2073 6176 6520 7175 616e 7469 7a65 6420   save quantized 
-00000e80: 6d6f 6465 6c0a 6d6f 6465 6c2e 7361 7665  model.model.save
-00000e90: 5f71 7561 6e74 697a 6564 2871 7561 6e74  _quantized(quant
-00000ea0: 697a 6564 5f6d 6f64 656c 5f64 6972 290a  ized_model_dir).
-00000eb0: 0a23 2073 6176 6520 7175 616e 7469 7a65  .# save quantize
-00000ec0: 6420 6d6f 6465 6c20 7573 696e 6720 7361  d model using sa
-00000ed0: 6665 7465 6e73 6f72 730a 6d6f 6465 6c2e  fetensors.model.
-00000ee0: 7361 7665 5f71 7561 6e74 697a 6564 2871  save_quantized(q
-00000ef0: 7561 6e74 697a 6564 5f6d 6f64 656c 5f64  uantized_model_d
-00000f00: 6972 2c20 7573 655f 7361 6665 7465 6e73  ir, use_safetens
-00000f10: 6f72 733d 5472 7565 290a 0a23 206c 6f61  ors=True)..# loa
-00000f20: 6420 7175 616e 7469 7a65 6420 6d6f 6465  d quantized mode
-00000f30: 6c2c 2063 7572 7265 6e74 6c79 206f 6e6c  l, currently onl
-00000f40: 7920 7375 7070 6f72 7420 6370 7520 6f72  y support cpu or
-00000f50: 2073 696e 676c 6520 6770 750a 6d6f 6465   single gpu.mode
-00000f60: 6c20 3d20 4175 746f 4750 5451 466f 7243  l = AutoGPTQForC
-00000f70: 6175 7361 6c4c 4d2e 6672 6f6d 5f71 7561  ausalLM.from_qua
-00000f80: 6e74 697a 6564 2871 7561 6e74 697a 6564  ntized(quantized
-00000f90: 5f6d 6f64 656c 5f64 6972 2c20 6465 7669  _model_dir, devi
-00000fa0: 6365 3d22 6375 6461 3a30 222c 2075 7365  ce="cuda:0", use
-00000fb0: 5f74 7269 746f 6e3d 4661 6c73 6529 0a0a  _triton=False)..
-00000fc0: 2320 696e 6665 7265 6e63 6520 7769 7468  # inference with
-00000fd0: 206d 6f64 656c 2e67 656e 6572 6174 650a   model.generate.
-00000fe0: 7072 696e 7428 746f 6b65 6e69 7a65 722e  print(tokenizer.
-00000ff0: 6465 636f 6465 286d 6f64 656c 2e67 656e  decode(model.gen
-00001000: 6572 6174 6528 2a2a 746f 6b65 6e69 7a65  erate(**tokenize
-00001010: 7228 2261 7574 6f5f 6770 7471 2069 7322  r("auto_gptq is"
-00001020: 2c20 7265 7475 726e 5f74 656e 736f 7273  , return_tensors
-00001030: 3d22 7074 2229 2e74 6f28 2263 7564 613a  ="pt").to("cuda:
-00001040: 3022 2929 5b30 5d29 290a 0a23 206f 7220  0"))[0]))..# or 
-00001050: 796f 7520 6361 6e20 616c 736f 2075 7365  you can also use
-00001060: 2070 6970 656c 696e 650a 7069 7065 6c69   pipeline.pipeli
-00001070: 6e65 203d 2054 6578 7447 656e 6572 6174  ne = TextGenerat
-00001080: 696f 6e50 6970 656c 696e 6528 6d6f 6465  ionPipeline(mode
-00001090: 6c3d 6d6f 6465 6c2c 2074 6f6b 656e 697a  l=model, tokeniz
-000010a0: 6572 3d74 6f6b 656e 697a 6572 290a 7072  er=tokenizer).pr
-000010b0: 696e 7428 7069 7065 6c69 6e65 2822 6175  int(pipeline("au
-000010c0: 746f 5f67 7074 7120 6973 2229 5b30 5d5b  to_gptq is")[0][
-000010d0: 2267 656e 6572 6174 6564 5f74 6578 7422  "generated_text"
-000010e0: 5d29 0a60 6060 0a0a 2323 2320 4375 7374  ]).```..### Cust
-000010f0: 6f6d 697a 6520 4d6f 6465 6c0a 4265 6c6f  omize Model.Belo
-00001100: 7720 6973 2061 6e20 6578 616d 706c 6520  w is an example 
-00001110: 746f 2065 7874 656e 6420 6061 7574 6f5f  to extend `auto_
-00001120: 6770 7471 6020 746f 2073 7570 706f 7274  gptq` to support
-00001130: 2060 4f50 5460 206d 6f64 656c 2c20 6173   `OPT` model, as
-00001140: 2079 6f75 2077 696c 6c20 7365 652c 2069   you will see, i
-00001150: 7427 7320 7665 7279 2065 6173 793a 0a60  t's very easy:.`
-00001160: 6060 7079 7468 6f6e 0a66 726f 6d20 6175  ``python.from au
-00001170: 746f 5f67 7074 712e 6d6f 6465 6c69 6e67  to_gptq.modeling
-00001180: 2069 6d70 6f72 7420 4261 7365 4750 5451   import BaseGPTQ
-00001190: 466f 7243 6175 7361 6c4c 4d0a 0a0a 636c  ForCausalLM...cl
-000011a0: 6173 7320 4f50 5447 5054 5146 6f72 4361  ass OPTGPTQForCa
-000011b0: 7573 616c 4c4d 2842 6173 6547 5054 5146  usalLM(BaseGPTQF
-000011c0: 6f72 4361 7573 616c 4c4d 293a 0a20 2020  orCausalLM):.   
-000011d0: 2023 2063 6861 696e 6564 2061 7474 7269   # chained attri
-000011e0: 6275 7465 206e 616d 6520 6f66 2074 7261  bute name of tra
-000011f0: 6e73 666f 726d 6572 206c 6179 6572 2062  nsformer layer b
-00001200: 6c6f 636b 0a20 2020 206c 6179 6572 735f  lock.    layers_
-00001210: 626c 6f63 6b5f 6e61 6d65 203d 2022 6d6f  block_name = "mo
-00001220: 6465 6c2e 6465 636f 6465 722e 6c61 7965  del.decoder.laye
-00001230: 7273 220a 2020 2020 2320 6368 6169 6e65  rs".    # chaine
-00001240: 6420 6174 7472 6962 7574 6520 6e61 6d65  d attribute name
-00001250: 7320 6f66 206f 7468 6572 206e 6e20 6d6f  s of other nn mo
-00001260: 6475 6c65 7320 7468 6174 2069 6e20 7468  dules that in th
-00001270: 6520 7361 6d65 206c 6576 656c 2061 7320  e same level as 
-00001280: 7468 6520 7472 616e 7366 6f72 6d65 7220  the transformer 
-00001290: 6c61 7965 7220 626c 6f63 6b0a 2020 2020  layer block.    
-000012a0: 6f75 7473 6964 655f 6c61 7965 725f 6d6f  outside_layer_mo
-000012b0: 6475 6c65 7320 3d20 5b0a 2020 2020 2020  dules = [.      
-000012c0: 2020 226d 6f64 656c 2e64 6563 6f64 6572    "model.decoder
-000012d0: 2e65 6d62 6564 5f74 6f6b 656e 7322 2c20  .embed_tokens", 
-000012e0: 226d 6f64 656c 2e64 6563 6f64 6572 2e65  "model.decoder.e
-000012f0: 6d62 6564 5f70 6f73 6974 696f 6e73 222c  mbed_positions",
-00001300: 2022 6d6f 6465 6c2e 6465 636f 6465 722e   "model.decoder.
-00001310: 7072 6f6a 6563 745f 6f75 7422 2c0a 2020  project_out",.  
-00001320: 2020 2020 2020 226d 6f64 656c 2e64 6563        "model.dec
-00001330: 6f64 6572 2e70 726f 6a65 6374 5f69 6e22  oder.project_in"
-00001340: 2c20 226d 6f64 656c 2e64 6563 6f64 6572  , "model.decoder
-00001350: 2e66 696e 616c 5f6c 6179 6572 5f6e 6f72  .final_layer_nor
-00001360: 6d22 0a20 2020 205d 0a20 2020 2023 2063  m".    ].    # c
-00001370: 6861 696e 6564 2061 7474 7269 6275 7465  hained attribute
-00001380: 206e 616d 6573 206f 6620 6c69 6e65 6172   names of linear
-00001390: 206c 6179 6572 7320 696e 2074 7261 6e73   layers in trans
-000013a0: 666f 726d 6572 206c 6179 6572 206d 6f64  former layer mod
-000013b0: 756c 650a 2020 2020 2320 6e6f 726d 616c  ule.    # normal
-000013c0: 6c79 2c20 7468 6572 6520 6172 6520 666f  ly, there are fo
-000013d0: 7572 2073 7562 206c 6973 7473 2c20 666f  ur sub lists, fo
-000013e0: 7220 6561 6368 206f 6e65 2074 6865 206d  r each one the m
-000013f0: 6f64 756c 6573 2069 6e20 6974 2063 616e  odules in it can
-00001400: 2062 6520 7365 656e 2061 7320 6f6e 6520   be seen as one 
-00001410: 6f70 6572 6174 696f 6e2c 200a 2020 2020  operation, .    
-00001420: 2320 616e 6420 7468 6520 6f72 6465 7220  # and the order 
-00001430: 7368 6f75 6c64 2062 6520 7468 6520 6f72  should be the or
-00001440: 6465 7220 7768 656e 2074 6865 7920 6172  der when they ar
-00001450: 6520 7472 756c 7920 6578 6563 7574 6564  e truly executed
-00001460: 2c20 696e 2074 6869 7320 6361 7365 2028  , in this case (
-00001470: 616e 6420 7573 7561 6c6c 7920 696e 206d  and usually in m
-00001480: 6f73 7420 6361 7365 7329 2c20 0a20 2020  ost cases), .   
-00001490: 2023 2074 6865 7920 6172 653a 2061 7474   # they are: att
-000014a0: 656e 7469 6f6e 2071 5f6b 5f76 2070 726f  ention q_k_v pro
-000014b0: 6a65 6374 696f 6e2c 2061 7474 656e 7469  jection, attenti
-000014c0: 6f6e 206f 7574 7075 7420 7072 6f6a 6563  on output projec
-000014d0: 7469 6f6e 2c20 4d4c 5020 7072 6f6a 6563  tion, MLP projec
-000014e0: 7420 696e 7075 742c 204d 4c50 2070 726f  t input, MLP pro
-000014f0: 6a65 6374 206f 7574 7075 740a 2020 2020  ject output.    
-00001500: 696e 7369 6465 5f6c 6179 6572 5f6d 6f64  inside_layer_mod
-00001510: 756c 6573 203d 205b 0a20 2020 2020 2020  ules = [.       
-00001520: 205b 2273 656c 665f 6174 746e 2e6b 5f70   ["self_attn.k_p
-00001530: 726f 6a22 2c20 2273 656c 665f 6174 746e  roj", "self_attn
-00001540: 2e76 5f70 726f 6a22 2c20 2273 656c 665f  .v_proj", "self_
-00001550: 6174 746e 2e71 5f70 726f 6a22 5d2c 0a20  attn.q_proj"],. 
-00001560: 2020 2020 2020 205b 2273 656c 665f 6174         ["self_at
-00001570: 746e 2e6f 7574 5f70 726f 6a22 5d2c 0a20  tn.out_proj"],. 
-00001580: 2020 2020 2020 205b 2266 6331 225d 2c0a         ["fc1"],.
-00001590: 2020 2020 2020 2020 5b22 6663 3222 5d0a          ["fc2"].
-000015a0: 2020 2020 5d0a 0a20 2020 2040 7374 6174      ]..    @stat
-000015b0: 6963 6d65 7468 6f64 0a20 2020 2023 2074  icmethod.    # t
-000015c0: 6865 206f 7665 7272 6964 696e 6720 6f66  he overriding of
-000015d0: 2074 6869 7320 6d65 7468 6f64 206d 6179   this method may
-000015e0: 206e 6f74 206e 6563 6573 7361 7279 2066   not necessary f
-000015f0: 6f72 206d 6f73 7420 6f74 6865 7220 6d6f  or most other mo
-00001600: 6465 6c73 0a20 2020 2064 6566 205f 7265  dels.    def _re
-00001610: 7369 7a65 5f61 7474 656e 7469 6f6e 5f6d  size_attention_m
-00001620: 6173 6b28 6174 7465 6e74 696f 6e5f 6d61  ask(attention_ma
-00001630: 736b 293a 0a20 2020 2020 2020 2061 7474  sk):.        att
-00001640: 656e 7469 6f6e 5f6d 6173 6b20 3d20 5b65  ention_mask = [e
-00001650: 6163 682e 756e 7371 7565 657a 6528 3129  ach.unsqueeze(1)
-00001660: 2066 6f72 2065 6163 6820 696e 2061 7474   for each in att
-00001670: 656e 7469 6f6e 5f6d 6173 6b5d 0a20 2020  ention_mask].   
-00001680: 2020 2020 2072 6574 7572 6e20 6174 7465       return atte
-00001690: 6e74 696f 6e5f 6d61 736b 0a60 6060 0a41  ntion_mask.```.A
-000016a0: 6674 6572 2074 6869 732c 2079 6f75 2063  fter this, you c
-000016b0: 616e 2075 7365 2060 4f50 5447 5054 5146  an use `OPTGPTQF
-000016c0: 6f72 4361 7573 616c 4c4d 2e66 726f 6d5f  orCausalLM.from_
-000016d0: 7072 6574 7261 696e 6564 6020 616e 6420  pretrained` and 
-000016e0: 6f74 6865 7220 6675 6e63 7469 6f6e 730a  other functions.
-000016f0: 0a23 2323 2045 7661 6c75 6174 696f 6e20  .### Evaluation 
-00001700: 6f6e 2044 6f77 6e73 7472 6561 6d20 5461  on Downstream Ta
-00001710: 736b 730a 4f6e 6520 6361 6e20 7573 6520  sks.One can use 
-00001720: 7461 736b 7320 6465 6669 6e65 6420 696e  tasks defined in
-00001730: 2060 6175 746f 5f67 7074 712e 6576 616c   `auto_gptq.eval
-00001740: 5f74 6173 6b73 6020 746f 2065 7661 6c75  _tasks` to evalu
-00001750: 6174 6520 6d6f 6465 6c27 7320 7065 7266  ate model's perf
-00001760: 6f72 6d61 6e63 6520 6f6e 2073 7065 6369  ormance on speci
-00001770: 6669 6320 646f 776e 2d73 7472 6561 6d20  fic down-stream 
-00001780: 7461 736b 2062 6566 6f72 6520 616e 6420  task before and 
-00001790: 6166 7465 7220 7175 616e 7469 7a61 7469  after quantizati
-000017a0: 6f6e 2e0a 0a54 6865 2070 7265 6465 6669  on...The predefi
-000017b0: 6e65 6420 7461 736b 7320 7375 7070 6f72  ned tasks suppor
-000017c0: 7420 616c 6c20 6361 7573 616c 2d6c 616e  t all causal-lan
-000017d0: 6775 6167 652d 6d6f 6465 6c73 2069 6d70  guage-models imp
-000017e0: 6c65 6d65 6e74 6564 2069 6e20 5b48 7567  lemented in [Hug
-000017f0: 6769 6e67 2046 6163 6520 7472 616e 7366  ging Face transf
-00001800: 6f72 6d65 7273 5d28 6874 7470 733a 2f2f  ormers](https://
-00001810: 6769 7468 7562 2e63 6f6d 2f68 7567 6769  github.com/huggi
-00001820: 6e67 6661 6365 2f74 7261 6e73 666f 726d  ngface/transform
-00001830: 6572 7329 2061 6e64 2069 6e20 7468 6973  ers) and in this
-00001840: 2070 726f 6a65 6374 2e0a 0a42 656c 6f77   project...Below
-00001850: 2069 7320 616e 2065 7861 6d70 6c65 2074   is an example t
-00001860: 6f20 6576 616c 7561 7465 2060 456c 6575  o evaluate `Eleu
-00001870: 7468 6572 4149 2f67 7074 2d6a 2d36 6260  therAI/gpt-j-6b`
-00001880: 206f 6e20 7365 7175 656e 6365 2d63 6c61   on sequence-cla
-00001890: 7373 6966 6963 6174 696f 6e20 7461 736b  ssification task
-000018a0: 2075 7369 6e67 2060 6361 7264 6966 666e   using `cardiffn
-000018b0: 6c70 2f74 7765 6574 5f73 656e 7469 6d65  lp/tweet_sentime
-000018c0: 6e74 5f6d 756c 7469 6c69 6e67 7561 6c60  nt_multilingual`
-000018d0: 2064 6174 6173 6574 3a0a 6060 6070 7974   dataset:.```pyt
-000018e0: 686f 6e0a 6672 6f6d 2066 756e 6374 6f6f  hon.from functoo
-000018f0: 6c73 2069 6d70 6f72 7420 7061 7274 6961  ls import partia
-00001900: 6c0a 0a69 6d70 6f72 7420 6461 7461 7365  l..import datase
-00001910: 7473 0a66 726f 6d20 7472 616e 7366 6f72  ts.from transfor
-00001920: 6d65 7273 2069 6d70 6f72 7420 4175 746f  mers import Auto
-00001930: 546f 6b65 6e69 7a65 722c 2041 7574 6f4d  Tokenizer, AutoM
-00001940: 6f64 656c 466f 7243 6175 7361 6c4c 4d2c  odelForCausalLM,
-00001950: 2047 656e 6572 6174 696f 6e43 6f6e 6669   GenerationConfi
-00001960: 670a 0a66 726f 6d20 6175 746f 5f67 7074  g..from auto_gpt
-00001970: 7120 696d 706f 7274 2041 7574 6f47 5054  q import AutoGPT
-00001980: 5146 6f72 4361 7573 616c 4c4d 2c20 4261  QForCausalLM, Ba
-00001990: 7365 5175 616e 7469 7a65 436f 6e66 6967  seQuantizeConfig
-000019a0: 0a66 726f 6d20 6175 746f 5f67 7074 712e  .from auto_gptq.
-000019b0: 6576 616c 5f74 6173 6b73 2069 6d70 6f72  eval_tasks impor
-000019c0: 7420 5365 7175 656e 6365 436c 6173 7369  t SequenceClassi
-000019d0: 6669 6361 7469 6f6e 5461 736b 0a0a 0a4d  ficationTask...M
-000019e0: 4f44 454c 203d 2022 456c 6575 7468 6572  ODEL = "Eleuther
-000019f0: 4149 2f67 7074 2d6a 2d36 6222 0a44 4154  AI/gpt-j-6b".DAT
-00001a00: 4153 4554 203d 2022 6361 7264 6966 666e  ASET = "cardiffn
-00001a10: 6c70 2f74 7765 6574 5f73 656e 7469 6d65  lp/tweet_sentime
-00001a20: 6e74 5f6d 756c 7469 6c69 6e67 7561 6c22  nt_multilingual"
-00001a30: 0a54 454d 504c 4154 4520 3d20 2251 7565  .TEMPLATE = "Que
-00001a40: 7374 696f 6e3a 5768 6174 2773 2074 6865  stion:What's the
-00001a50: 2073 656e 7469 6d65 6e74 206f 6620 7468   sentiment of th
-00001a60: 6520 6769 7665 6e20 7465 7874 3f20 4368  e given text? Ch
-00001a70: 6f69 6365 7320 6172 6520 7b6c 6162 656c  oices are {label
-00001a80: 737d 2e5c 6e54 6578 743a 207b 7465 7874  s}.\nText: {text
-00001a90: 7d5c 6e41 6e73 7765 723a 220a 4944 324c  }\nAnswer:".ID2L
-00001aa0: 4142 454c 203d 207b 0a20 2020 2030 3a20  ABEL = {.    0: 
-00001ab0: 226e 6567 6174 6976 6522 2c0a 2020 2020  "negative",.    
-00001ac0: 313a 2022 6e65 7574 7261 6c22 2c0a 2020  1: "neutral",.  
-00001ad0: 2020 323a 2022 706f 7369 7469 7665 220a    2: "positive".
-00001ae0: 7d0a 4c41 4245 4c53 203d 206c 6973 7428  }.LABELS = list(
-00001af0: 4944 324c 4142 454c 2e76 616c 7565 7328  ID2LABEL.values(
-00001b00: 2929 0a0a 0a64 6566 2064 735f 7265 6661  ))...def ds_refa
-00001b10: 6374 6f72 5f66 6e28 7361 6d70 6c65 7329  ctor_fn(samples)
-00001b20: 3a0a 2020 2020 7465 7874 5f64 6174 6120  :.    text_data 
-00001b30: 3d20 7361 6d70 6c65 735b 2274 6578 7422  = samples["text"
-00001b40: 5d0a 2020 2020 6c61 6265 6c5f 6461 7461  ].    label_data
-00001b50: 203d 2073 616d 706c 6573 5b22 6c61 6265   = samples["labe
-00001b60: 6c22 5d0a 0a20 2020 206e 6577 5f73 616d  l"]..    new_sam
-00001b70: 706c 6573 203d 207b 2270 726f 6d70 7422  ples = {"prompt"
-00001b80: 3a20 5b5d 2c20 226c 6162 656c 223a 205b  : [], "label": [
-00001b90: 5d7d 0a20 2020 2066 6f72 2074 6578 742c  ]}.    for text,
-00001ba0: 206c 6162 656c 2069 6e20 7a69 7028 7465   label in zip(te
-00001bb0: 7874 5f64 6174 612c 206c 6162 656c 5f64  xt_data, label_d
-00001bc0: 6174 6129 3a0a 2020 2020 2020 2020 7072  ata):.        pr
-00001bd0: 6f6d 7074 203d 2054 454d 504c 4154 452e  ompt = TEMPLATE.
-00001be0: 666f 726d 6174 286c 6162 656c 733d 4c41  format(labels=LA
-00001bf0: 4245 4c53 2c20 7465 7874 3d74 6578 7429  BELS, text=text)
-00001c00: 0a20 2020 2020 2020 206e 6577 5f73 616d  .        new_sam
-00001c10: 706c 6573 5b22 7072 6f6d 7074 225d 2e61  ples["prompt"].a
-00001c20: 7070 656e 6428 7072 6f6d 7074 290a 2020  ppend(prompt).  
-00001c30: 2020 2020 2020 6e65 775f 7361 6d70 6c65        new_sample
-00001c40: 735b 226c 6162 656c 225d 2e61 7070 656e  s["label"].appen
-00001c50: 6428 4944 324c 4142 454c 5b6c 6162 656c  d(ID2LABEL[label
-00001c60: 5d29 0a0a 2020 2020 7265 7475 726e 206e  ])..    return n
-00001c70: 6577 5f73 616d 706c 6573 0a0a 0a23 2020  ew_samples...#  
-00001c80: 6d6f 6465 6c20 3d20 4175 746f 4d6f 6465  model = AutoMode
-00001c90: 6c46 6f72 4361 7573 616c 4c4d 2e66 726f  lForCausalLM.fro
-00001ca0: 6d5f 7072 6574 7261 696e 6564 284d 4f44  m_pretrained(MOD
-00001cb0: 454c 292e 6576 616c 2829 2e68 616c 6628  EL).eval().half(
-00001cc0: 292e 746f 2822 6375 6461 3a30 2229 0a6d  ).to("cuda:0").m
-00001cd0: 6f64 656c 203d 2041 7574 6f47 5054 5146  odel = AutoGPTQF
-00001ce0: 6f72 4361 7573 616c 4c4d 2e66 726f 6d5f  orCausalLM.from_
-00001cf0: 7072 6574 7261 696e 6564 284d 4f44 454c  pretrained(MODEL
-00001d00: 2c20 4261 7365 5175 616e 7469 7a65 436f  , BaseQuantizeCo
-00001d10: 6e66 6967 2829 290a 746f 6b65 6e69 7a65  nfig()).tokenize
-00001d20: 7220 3d20 4175 746f 546f 6b65 6e69 7a65  r = AutoTokenize
-00001d30: 722e 6672 6f6d 5f70 7265 7472 6169 6e65  r.from_pretraine
-00001d40: 6428 4d4f 4445 4c29 0a0a 7461 736b 203d  d(MODEL)..task =
-00001d50: 2053 6571 7565 6e63 6543 6c61 7373 6966   SequenceClassif
-00001d60: 6963 6174 696f 6e54 6173 6b28 0a20 2020  icationTask(.   
-00001d70: 2020 2020 206d 6f64 656c 3d6d 6f64 656c       model=model
-00001d80: 2c0a 2020 2020 2020 2020 746f 6b65 6e69  ,.        tokeni
-00001d90: 7a65 723d 746f 6b65 6e69 7a65 722c 0a20  zer=tokenizer,. 
-00001da0: 2020 2020 2020 2063 6c61 7373 6573 3d4c         classes=L
-00001db0: 4142 454c 532c 0a20 2020 2020 2020 2064  ABELS,.        d
-00001dc0: 6174 615f 6e61 6d65 5f6f 725f 7061 7468  ata_name_or_path
-00001dd0: 3d44 4154 4153 4554 2c0a 2020 2020 2020  =DATASET,.      
-00001de0: 2020 7072 6f6d 7074 5f63 6f6c 5f6e 616d    prompt_col_nam
-00001df0: 653d 2270 726f 6d70 7422 2c0a 2020 2020  e="prompt",.    
-00001e00: 2020 2020 6c61 6265 6c5f 636f 6c5f 6e61      label_col_na
-00001e10: 6d65 3d22 6c61 6265 6c22 2c0a 2020 2020  me="label",.    
-00001e20: 2020 2020 2a2a 7b0a 2020 2020 2020 2020      **{.        
-00001e30: 2020 2020 226e 756d 5f73 616d 706c 6573      "num_samples
-00001e40: 223a 2031 3030 302c 2020 2320 686f 7720  ": 1000,  # how 
-00001e50: 6d61 6e79 2073 616d 706c 6573 2077 696c  many samples wil
-00001e60: 6c20 6265 2073 616d 706c 6564 2074 6f20  l be sampled to 
-00001e70: 6576 616c 7561 7469 6f6e 0a20 2020 2020  evaluation.     
-00001e80: 2020 2020 2020 2022 7361 6d70 6c65 5f6d         "sample_m
-00001e90: 6178 5f6c 656e 223a 2031 3032 342c 2020  ax_len": 1024,  
-00001ea0: 2320 6d61 7820 746f 6b65 6e73 2066 6f72  # max tokens for
-00001eb0: 2065 6163 6820 7361 6d70 6c65 0a20 2020   each sample.   
-00001ec0: 2020 2020 2020 2020 2022 626c 6f63 6b5f           "block_
-00001ed0: 6d61 785f 6c65 6e22 3a20 3230 3438 2c20  max_len": 2048, 
-00001ee0: 2023 206d 6178 2074 6f6b 656e 7320 666f   # max tokens fo
-00001ef0: 7220 6561 6368 2064 6174 6120 626c 6f63  r each data bloc
-00001f00: 6b0a 2020 2020 2020 2020 2020 2020 2320  k.            # 
-00001f10: 6675 6e63 7469 6f6e 2074 6f20 6c6f 6164  function to load
-00001f20: 2064 6174 6173 6574 2c20 6f6e 6520 6d75   dataset, one mu
-00001f30: 7374 206f 6e6c 7920 6163 6365 7074 2064  st only accept d
-00001f40: 6174 615f 6e61 6d65 5f6f 725f 7061 7468  ata_name_or_path
-00001f50: 2061 7320 696e 7075 7420 0a20 2020 2020   as input .     
-00001f60: 2020 2020 2020 2023 2061 6e64 2072 6574         # and ret
-00001f70: 7572 6e20 6461 7461 7365 7473 2e44 6174  urn datasets.Dat
-00001f80: 6173 6574 0a20 2020 2020 2020 2020 2020  aset.           
-00001f90: 2022 6c6f 6164 5f66 6e22 3a20 7061 7274   "load_fn": part
-00001fa0: 6961 6c28 6461 7461 7365 7473 2e6c 6f61  ial(datasets.loa
-00001fb0: 645f 6461 7461 7365 742c 206e 616d 653d  d_dataset, name=
-00001fc0: 2265 6e67 6c69 7368 2229 2c20 200a 2020  "english"),  .  
-00001fd0: 2020 2020 2020 2020 2020 2320 6675 6e63            # func
-00001fe0: 7469 6f6e 2074 6f20 7072 6570 726f 6365  tion to preproce
-00001ff0: 7373 2064 6174 6173 6574 2c20 7768 6963  ss dataset, whic
-00002000: 6820 6973 2075 7365 6420 666f 7220 6461  h is used for da
-00002010: 7461 7365 7473 2e44 6174 6173 6574 2e6d  tasets.Dataset.m
-00002020: 6170 2c20 0a20 2020 2020 2020 2020 2020  ap, .           
-00002030: 2023 206d 7573 7420 7265 7475 726e 2044   # must return D
-00002040: 6963 745b 7374 722c 206c 6973 745d 2077  ict[str, list] w
-00002050: 6974 6820 6f6e 6c79 2074 776f 206b 6579  ith only two key
-00002060: 733a 205b 7072 6f6d 7074 5f63 6f6c 5f6e  s: [prompt_col_n
-00002070: 616d 652c 206c 6162 656c 5f63 6f6c 5f6e  ame, label_col_n
-00002080: 616d 655d 0a20 2020 2020 2020 2020 2020  ame].           
-00002090: 2022 7072 6570 726f 6365 7373 5f66 6e22   "preprocess_fn"
-000020a0: 3a20 6473 5f72 6566 6163 746f 725f 666e  : ds_refactor_fn
-000020b0: 2c20 200a 2020 2020 2020 2020 2020 2020  ,  .            
-000020c0: 2320 7472 756e 6361 7465 206c 6162 656c  # truncate label
-000020d0: 2077 6865 6e20 7361 6d70 6c65 2773 206c   when sample's l
-000020e0: 656e 6774 6820 6578 6365 6564 2073 616d  ength exceed sam
-000020f0: 706c 655f 6d61 785f 6c65 6e0a 2020 2020  ple_max_len.    
-00002100: 2020 2020 2020 2020 2274 7275 6e63 6174          "truncat
-00002110: 655f 7072 6f6d 7074 223a 2046 616c 7365  e_prompt": False
-00002120: 2020 0a20 2020 2020 2020 207d 0a20 2020    .        }.   
-00002130: 2029 0a0a 2320 6e6f 7465 2074 6861 7420   )..# note that 
-00002140: 6d61 785f 6e65 775f 746f 6b65 6e73 2077  max_new_tokens w
-00002150: 696c 6c20 6265 2061 7574 6f6d 6174 6963  ill be automatic
-00002160: 616c 6c79 2073 7065 6369 6669 6564 2069  ally specified i
-00002170: 6e74 6572 6e61 6c6c 7920 6261 7365 6420  nternally based 
-00002180: 6f6e 2067 6976 656e 2063 6c61 7373 6573  on given classes
-00002190: 0a70 7269 6e74 2874 6173 6b2e 7275 6e28  .print(task.run(
-000021a0: 2929 0a0a 2320 7365 6c66 2d63 6f6e 7369  ))..# self-consi
-000021b0: 7374 656e 6379 0a70 7269 6e74 280a 2020  stency.print(.  
-000021c0: 2020 7461 736b 2e72 756e 280a 2020 2020    task.run(.    
-000021d0: 2020 2020 6765 6e65 7261 7469 6f6e 5f63      generation_c
-000021e0: 6f6e 6669 673d 4765 6e65 7261 7469 6f6e  onfig=Generation
-000021f0: 436f 6e66 6967 280a 2020 2020 2020 2020  Config(.        
-00002200: 2020 2020 6e75 6d5f 6265 616d 733d 332c      num_beams=3,
-00002210: 0a20 2020 2020 2020 2020 2020 206e 756d  .            num
-00002220: 5f72 6574 7572 6e5f 7365 7175 656e 6365  _return_sequence
-00002230: 733d 332c 0a20 2020 2020 2020 2020 2020  s=3,.           
-00002240: 2064 6f5f 7361 6d70 6c65 3d54 7275 650a   do_sample=True.
-00002250: 2020 2020 2020 2020 290a 2020 2020 290a          ).    ).
-00002260: 290a 6060 600a 0a23 2323 204d 6f72 6520  ).```..### More 
-00002270: 4578 616d 706c 6573 0a46 6f72 206d 6f72  Examples.For mor
-00002280: 6520 6578 616d 706c 6573 2c20 706c 6561  e examples, plea
-00002290: 7365 2074 7572 6e20 746f 205b 6578 616d  se turn to [exam
-000022a0: 706c 6573 5d28 6578 616d 706c 6573 2f52  ples](examples/R
-000022b0: 4541 444d 452e 6d64 290a 0a23 2320 5369  EADME.md)..## Si
-000022c0: 6465 204e 6f74 6573 0a23 2323 2056 5241  de Notes.### VRA
-000022d0: 4d0a 4375 7272 656e 746c 792c 2049 2070  M.Currently, I p
-000022e0: 7574 2065 7665 7279 7468 696e 6720 2864  ut everything (d
-000022f0: 6174 612c 206d 6f64 656c 2c20 6574 632e  ata, model, etc.
-00002300: 2920 696e 746f 2043 5055 2075 7469 6c20  ) into CPU util 
-00002310: 6f6e 6520 6973 2072 6571 7569 7265 6420  one is required 
-00002320: 746f 2062 6520 7573 6564 206f 7220 6578  to be used or ex
-00002330: 6563 7574 6564 206f 6e20 4750 5520 2861  ecuted on GPU (a
-00002340: 6e64 2077 696c 6c20 6261 636b 2074 6f20  nd will back to 
-00002350: 4350 5520 6f6e 6365 2074 6865 2065 7865  CPU once the exe
-00002360: 6375 7469 6f6e 2066 696e 6973 6865 6429  cution finished)
-00002370: 2e20 5468 6f75 6768 2049 2064 6964 6e27  . Though I didn'
-00002380: 7420 7275 6e20 616e 7920 6265 6e63 686d  t run any benchm
-00002390: 6172 6b20 746f 2074 6869 7320 6461 7465  ark to this date
-000023a0: 2c20 6275 7420 7468 6520 6d61 7869 6d75  , but the maximu
-000023b0: 6d20 5652 414d 2075 7361 6765 2066 6f72  m VRAM usage for
-000023c0: 2047 5054 4a20 6973 2061 626f 7574 2036   GPTJ is about 6
-000023d0: 4742 2c20 7768 6963 6820 6d61 7920 6265  GB, which may be
-000023e0: 2063 6f6e 7369 6465 7265 6420 6173 2061   considered as a
-000023f0: 2072 6566 6572 656e 6365 2e0a 0a23 2320   reference...## 
-00002400: 4163 6b6e 6f77 6c65 6467 656d 656e 740a  Acknowledgement.
-00002410: 2d20 5370 6563 6961 6c6c 7920 7468 616e  - Specially than
-00002420: 6b73 202a 2a45 6c69 6173 2046 7261 6e74  ks **Elias Frant
-00002430: 6172 2a2a 2c20 2a2a 5361 6c65 6820 4173  ar**, **Saleh As
-00002440: 686b 626f 6f73 2a2a 2c20 2a2a 546f 7273  hkboos**, **Tors
-00002450: 7465 6e20 486f 6566 6c65 722a 2a20 616e  ten Hoefler** an
-00002460: 6420 2a2a 4461 6e20 416c 6973 7461 7268  d **Dan Alistarh
-00002470: 2a2a 2066 6f72 2070 726f 706f 7369 6e67  ** for proposing
-00002480: 202a 2a47 5054 512a 2a20 616c 676f 7269   **GPTQ** algori
-00002490: 7468 6d20 616e 6420 6f70 656e 2073 6f75  thm and open sou
-000024a0: 7263 6520 7468 6520 5b63 6f64 655d 2868  rce the [code](h
-000024b0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000024c0: 6d2f 4953 542d 4441 534c 6162 2f67 7074  m/IST-DASLab/gpt
-000024d0: 7129 2e0a 2d20 5370 6563 6961 6c6c 7920  q)..- Specially 
-000024e0: 7468 616e 6b73 202a 2a71 776f 7071 776f  thanks **qwopqwo
-000024f0: 7032 3030 2a2a 2c20 666f 7220 636f 6465  p200**, for code
-00002500: 2069 6e20 7468 6973 2070 726f 6a65 6374   in this project
-00002510: 2074 6861 7420 7265 6c65 7661 6e74 2074   that relevant t
-00002520: 6f20 7175 616e 7469 7a61 7469 6f6e 2061  o quantization a
-00002530: 7265 206d 6169 6e6c 7920 7265 6665 7265  re mainly refere
-00002540: 6e63 6564 2066 726f 6d20 5b47 5054 512d  nced from [GPTQ-
-00002550: 666f 722d 4c4c 614d 615d 2868 7474 7073  for-LLaMa](https
-00002560: 3a2f 2f67 6974 6875 622e 636f 6d2f 7177  ://github.com/qw
-00002570: 6f70 7177 6f70 3230 302f 4750 5451 2d66  opqwop200/GPTQ-f
-00002580: 6f72 2d4c 4c61 4d61 2f74 7265 652f 6375  or-LLaMa/tree/cu
-00002590: 6461 292e 0a                             da)..
+00000000: 3c68 3120 616c 6967 6e3d 2263 656e 7465  <h1 align="cente
+00000010: 7222 3e41 7574 6f47 5054 513c 2f68 313e  r">AutoGPTQ</h1>
+00000020: 0d0a 3c70 2061 6c69 676e 3d22 6365 6e74  ..<p align="cent
+00000030: 6572 223e 416e 2065 6173 792d 746f 2d75  er">An easy-to-u
+00000040: 7365 204c 4c4d 7320 7175 616e 7469 7a61  se LLMs quantiza
+00000050: 7469 6f6e 2070 6163 6b61 6765 2077 6974  tion package wit
+00000060: 6820 7573 6572 2d66 7269 656e 646c 7920  h user-friendly 
+00000070: 6170 6973 2c20 6261 7365 6420 6f6e 2047  apis, based on G
+00000080: 5054 5120 616c 676f 7269 7468 6d2e 3c2f  PTQ algorithm.</
+00000090: 703e 0d0a 3c70 2061 6c69 676e 3d22 6365  p>..<p align="ce
+000000a0: 6e74 6572 223e 0d0a 2020 2020 3c61 2068  nter">..    <a h
+000000b0: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
+000000c0: 6875 622e 636f 6d2f 5061 6e51 6957 6569  hub.com/PanQiWei
+000000d0: 2f41 7574 6f47 5054 512f 7265 6c65 6173  /AutoGPTQ/releas
+000000e0: 6573 223e 0d0a 2020 2020 2020 2020 3c69  es">..        <i
+000000f0: 6d67 2061 6c74 3d22 4769 7448 7562 2072  mg alt="GitHub r
+00000100: 656c 6561 7365 2220 7372 633d 2268 7474  elease" src="htt
+00000110: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000120: 2e69 6f2f 6769 7468 7562 2f72 656c 6561  .io/github/relea
+00000130: 7365 2f50 616e 5169 5765 692f 4175 746f  se/PanQiWei/Auto
+00000140: 4750 5451 2e73 7667 223e 0d0a 2020 2020  GPTQ.svg">..    
+00000150: 3c2f 613e 0d0a 2020 2020 3c61 2068 7265  </a>..    <a hre
+00000160: 663d 2268 7474 7073 3a2f 2f70 7970 692e  f="https://pypi.
+00000170: 6f72 672f 7072 6f6a 6563 742f 6175 746f  org/project/auto
+00000180: 2d67 7074 712f 223e 0d0a 2020 2020 2020  -gptq/">..      
+00000190: 2020 3c69 6d67 2061 6c74 3d22 5079 5049    <img alt="PyPI
+000001a0: 202d 2044 6f77 6e6c 6f61 6473 2220 7372   - Downloads" sr
+000001b0: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
+000001c0: 6869 656c 6473 2e69 6f2f 7079 7069 2f64  hields.io/pypi/d
+000001d0: 642f 6175 746f 2d67 7074 7122 3e0d 0a20  d/auto-gptq">.. 
+000001e0: 2020 203c 2f61 3e0d 0a3c 2f70 3e0d 0a3c     </a>..</p>..<
+000001f0: 6834 2061 6c69 676e 3d22 6365 6e74 6572  h4 align="center
+00000200: 223e 0d0a 2020 2020 3c70 3e0d 0a20 2020  ">..    <p>..   
+00000210: 2020 2020 203c 623e 456e 676c 6973 683c       <b>English<
+00000220: 2f62 3e20 7c0d 0a20 2020 2020 2020 203c  /b> |..        <
+00000230: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000240: 6769 7468 7562 2e63 6f6d 2f50 616e 5169  github.com/PanQi
+00000250: 5765 692f 4175 746f 4750 5451 2f62 6c6f  Wei/AutoGPTQ/blo
+00000260: 622f 6d61 696e 2f52 4541 444d 455f 7a68  b/main/README_zh
+00000270: 2e6d 6422 3ee4 b8ad e696 873c 2f61 3e0d  .md">......</a>.
+00000280: 0a20 2020 203c 703e 0d0a 3c2f 6834 3e0d  .    <p>..</h4>.
+00000290: 0a0d 0a23 2320 4e65 7773 206f 7220 5570  ...## News or Up
+000002a0: 6461 7465 0d0a 2d20 3230 3233 2d30 352d  date..- 2023-05-
+000002b0: 3034 202d 2028 5570 6461 7465 2920 2d20  04 - (Update) - 
+000002c0: 5375 7070 6f72 7420 7573 696e 6720 6661  Support using fa
+000002d0: 7374 6572 2063 7564 6120 6b65 726e 656c  ster cuda kernel
+000002e0: 2077 6865 6e20 606e 6f74 2064 6573 635f   when `not desc_
+000002f0: 6163 7420 6f72 2067 726f 7570 5f73 697a  act or group_siz
+00000300: 6520 3d3d 202d 3160 2e0d 0a2d 2032 3032  e == -1`...- 202
+00000310: 332d 3034 2d32 3920 2d20 2855 7064 6174  3-04-29 - (Updat
+00000320: 6529 202d 2053 7570 706f 7274 206c 6f61  e) - Support loa
+00000330: 6469 6e67 2071 7561 6e74 697a 6564 206d  ding quantized m
+00000340: 6f64 656c 2066 726f 6d20 6172 6269 7472  odel from arbitr
+00000350: 6172 7920 7175 616e 7469 7a65 5f63 6f6e  ary quantize_con
+00000360: 6669 6720 616e 6420 6d6f 6465 6c5f 6261  fig and model_ba
+00000370: 7365 6e61 6d65 2e0d 0a2d 2032 3032 332d  sename...- 2023-
+00000380: 3034 2d32 3820 2d20 2855 7064 6174 6529  04-28 - (Update)
+00000390: 202d 2053 7570 706f 7274 2043 5055 206f   - Support CPU o
+000003a0: 6666 6c6f 6164 2061 6e64 2071 7561 6e74  ffload and quant
+000003b0: 697a 652f 696e 6665 7265 6e63 6520 6f6e  ize/inference on
+000003c0: 206d 756c 7469 706c 6520 6465 7669 6365   multiple device
+000003d0: 732c 2073 7570 706f 7274 2060 6770 7432  s, support `gpt2
+000003e0: 6020 7479 7065 206d 6f64 656c 732e 0d0a  ` type models...
+000003f0: 0d0a 2a46 6f72 206d 6f72 6520 6869 7374  ..*For more hist
+00000400: 6f72 6965 7320 706c 6561 7365 2074 7572  ories please tur
+00000410: 6e20 746f 205b 6865 7265 5d28 646f 6373  n to [here](docs
+00000420: 2f4e 4557 535f 4f52 5f55 5044 4154 452e  /NEWS_OR_UPDATE.
+00000430: 6d64 292a 0d0a 0d0a 2323 2049 6e73 7461  md)*....## Insta
+00000440: 6c6c 6174 696f 6e0d 0a0d 0a23 2323 2051  llation....### Q
+00000450: 7569 636b 2049 6e73 7461 6c6c 6174 696f  uick Installatio
+00000460: 6e0d 0a59 6f75 2063 616e 2069 6e73 7461  n..You can insta
+00000470: 6c6c 2074 6865 206c 6174 6573 7420 7374  ll the latest st
+00000480: 6162 6c65 2072 656c 6561 7365 206f 6620  able release of 
+00000490: 4175 746f 4750 5451 2066 726f 6d20 7069  AutoGPTQ from pi
+000004a0: 703a 0d0a 6060 6073 6865 6c6c 0d0a 7069  p:..```shell..pi
+000004b0: 7020 696e 7374 616c 6c20 6175 746f 2d67  p install auto-g
+000004c0: 7074 710d 0a60 6060 0d0a 2323 2323 2064  ptq..```..#### d
+000004d0: 6973 6162 6c65 2063 7564 6120 6578 7465  isable cuda exte
+000004e0: 6e73 696f 6e73 0d0a 4279 2064 6566 6175  nsions..By defau
+000004f0: 6c74 2c20 6375 6461 2065 7874 656e 7369  lt, cuda extensi
+00000500: 6f6e 7320 7769 6c6c 2062 6520 696e 7374  ons will be inst
+00000510: 616c 6c65 6420 7768 656e 2060 746f 7263  alled when `torc
+00000520: 6860 2061 6e64 2060 6375 6461 6020 6973  h` and `cuda` is
+00000530: 2061 6c72 6561 6479 2069 6e73 7461 6c6c   already install
+00000540: 6564 2069 6e20 796f 7572 206d 6163 6869  ed in your machi
+00000550: 6e65 2c20 6966 2079 6f75 2064 6f6e 2774  ne, if you don't
+00000560: 2077 616e 7420 746f 2075 7365 2074 6865   want to use the
+00000570: 6d2c 2075 7369 6e67 3a0d 0a60 6060 7368  m, using:..```sh
+00000580: 656c 6c0d 0a42 5549 4c44 5f43 5544 415f  ell..BUILD_CUDA_
+00000590: 4558 543d 3020 7069 7020 696e 7374 616c  EXT=0 pip instal
+000005a0: 6c20 6175 746f 2d67 7074 710d 0a60 6060  l auto-gptq..```
+000005b0: 0d0a 416e 6420 746f 206d 616b 6520 7375  ..And to make su
+000005c0: 7265 2060 7175 616e 745f 6375 6461 6020  re `quant_cuda` 
+000005d0: 6973 206e 6f74 2065 7665 7220 696e 2079  is not ever in y
+000005e0: 6f75 7220 7669 7274 7561 6c20 656e 7669  our virtual envi
+000005f0: 726f 6e6d 656e 742c 2072 756e 3a0d 0a60  ronment, run:..`
+00000600: 6060 7368 656c 6c0d 0a70 6970 2075 6e69  ``shell..pip uni
+00000610: 6e73 7461 6c6c 2071 7561 6e74 5f63 7564  nstall quant_cud
+00000620: 6120 2d79 0d0a 6060 600d 0a23 2323 2320  a -y..```..#### 
+00000630: 746f 2073 7570 706f 7274 204c 4c61 4d61  to support LLaMa
+00000640: 206d 6f64 656c 0d0a 466f 7220 736f 6d65   model..For some
+00000650: 2070 656f 706c 6520 7761 6e74 2074 6f20   people want to 
+00000660: 7472 7920 4c4c 614d 6120 616e 6420 7768  try LLaMa and wh
+00000670: 6f73 6520 6074 7261 6e73 666f 726d 6572  ose `transformer
+00000680: 7360 2076 6572 7369 6f6e 206e 6f74 206d  s` version not m
+00000690: 6565 7420 7468 6520 6e65 7765 7374 206f  eet the newest o
+000006a0: 6e65 2074 6861 7420 7375 7070 6f72 7473  ne that supports
+000006b0: 2069 742c 2075 7369 6e67 3a0d 0a60 6060   it, using:..```
+000006c0: 7368 656c 6c0d 0a70 6970 2069 6e73 7461  shell..pip insta
+000006d0: 6c6c 2061 7574 6f2d 6770 7471 5b6c 6c61  ll auto-gptq[lla
+000006e0: 6d61 5d0d 0a60 6060 0d0a 2323 2323 2074  ma]..```..#### t
+000006f0: 6f20 7375 7070 6f72 7420 7472 6974 6f6e  o support triton
+00000700: 2073 7065 6564 7570 0d0a 546f 2069 6e74   speedup..To int
+00000710: 6567 7261 7465 2077 6974 6820 6074 7269  egrate with `tri
+00000720: 746f 6e60 2c20 7573 696e 673a 0d0a 3e20  ton`, using:..> 
+00000730: 7761 726e 696e 673a 2063 7572 7265 6e74  warning: current
+00000740: 6c79 2074 7269 746f 6e20 6f6e 6c79 2073  ly triton only s
+00000750: 7570 706f 7274 7320 6c69 6e75 783b 2033  upports linux; 3
+00000760: 2d62 6974 2071 7561 6e74 697a 6174 696f  -bit quantizatio
+00000770: 6e20 6973 206e 6f74 2073 7570 706f 7274  n is not support
+00000780: 6564 2077 6865 6e20 7573 696e 6720 7472  ed when using tr
+00000790: 6974 6f6e 0d0a 0d0a 6060 6073 6865 6c6c  iton....```shell
+000007a0: 0d0a 7069 7020 696e 7374 616c 6c20 6175  ..pip install au
+000007b0: 746f 2d67 7074 715b 7472 6974 6f6e 5d0d  to-gptq[triton].
+000007c0: 0a60 6060 0d0a 0d0a 2323 2320 496e 7374  .```....### Inst
+000007d0: 616c 6c20 6672 6f6d 2073 6f75 7263 650d  all from source.
+000007e0: 0a43 6c6f 6e65 2074 6865 2073 6f75 7263  .Clone the sourc
+000007f0: 6520 636f 6465 3a0d 0a60 6060 7368 656c  e code:..```shel
+00000800: 6c0d 0a67 6974 2063 6c6f 6e65 2068 7474  l..git clone htt
+00000810: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000820: 5061 6e51 6957 6569 2f41 7574 6f47 5054  PanQiWei/AutoGPT
+00000830: 512e 6769 7420 2626 2063 6420 4175 746f  Q.git && cd Auto
+00000840: 4750 5451 0d0a 6060 600d 0a54 6865 6e2c  GPTQ..```..Then,
+00000850: 2069 6e73 7461 6c6c 2066 726f 6d20 736f   install from so
+00000860: 7572 6365 3a0d 0a60 6060 7368 656c 6c0d  urce:..```shell.
+00000870: 0a70 6970 2069 6e73 7461 6c6c 202e 0d0a  .pip install ...
+00000880: 6060 600d 0a4c 696b 6520 7175 6963 6b20  ```..Like quick 
+00000890: 696e 7374 616c 6c61 7469 6f6e 2c20 796f  installation, yo
+000008a0: 7520 6361 6e20 616c 736f 2073 6574 2060  u can also set `
+000008b0: 4255 494c 445f 4355 4441 5f45 5854 3d30  BUILD_CUDA_EXT=0
+000008c0: 6020 746f 2064 6973 6162 6c65 2070 7974  ` to disable pyt
+000008d0: 6f72 6368 2065 7874 656e 7369 6f6e 2062  orch extension b
+000008e0: 7569 6c64 696e 672e 0d0a 0d0a 5573 6520  uilding.....Use 
+000008f0: 602e 5b6c 6c61 6d61 5d60 2069 6620 796f  `.[llama]` if yo
+00000900: 7520 7761 6e74 2074 6f20 7472 7920 4c4c  u want to try LL
+00000910: 614d 6120 6d6f 6465 6c2e 0d0a 0d0a 5573  aMa model.....Us
+00000920: 6520 602e 5b74 7269 746f 6e5d 6020 6966  e `.[triton]` if
+00000930: 2079 6f75 2077 616e 7420 746f 2069 6e74   you want to int
+00000940: 6567 7261 7465 2077 6974 6820 7472 6974  egrate with trit
+00000950: 6f6e 2061 6e64 2069 7427 7320 6176 6169  on and it's avai
+00000960: 6c61 626c 6520 6f6e 2079 6f75 7220 6f70  lable on your op
+00000970: 6572 6174 696e 6720 7379 7374 656d 2e0d  erating system..
+00000980: 0a0d 0a0d 0a23 2320 5375 7070 6f72 7465  .....## Supporte
+00000990: 6420 4d6f 6465 6c73 0d0a 4375 7272 656e  d Models..Curren
+000009a0: 746c 792c 2060 6175 746f 5f67 7074 7160  tly, `auto_gptq`
+000009b0: 2073 7570 706f 7274 733a 2060 626c 6f6f   supports: `bloo
+000009c0: 6d60 2c20 6067 7074 3260 2c20 6067 7074  m`, `gpt2`, `gpt
+000009d0: 5f6e 656f 7860 2c20 6067 7074 6a60 2c20  _neox`, `gptj`, 
+000009e0: 606c 6c61 6d61 602c 2060 6d6f 7373 6020  `llama`, `moss` 
+000009f0: 616e 6420 606f 7074 603b 206d 6f72 6520  and `opt`; more 
+00000a00: 5472 616e 7366 6f72 6d65 7220 6d6f 6465  Transformer mode
+00000a10: 6c73 2077 696c 6c20 636f 6d65 2073 6f6f  ls will come soo
+00000a20: 6e21 0d0a 0d0a 2323 2053 7570 706f 7274  n!....## Support
+00000a30: 6564 2045 7661 6c75 6174 696f 6e20 5461  ed Evaluation Ta
+00000a40: 736b 730d 0a43 7572 7265 6e74 6c79 2c20  sks..Currently, 
+00000a50: 6061 7574 6f5f 6770 7471 6020 7375 7070  `auto_gptq` supp
+00000a60: 6f72 7473 3a20 604c 616e 6775 6167 654d  orts: `LanguageM
+00000a70: 6f64 656c 696e 6754 6173 6b60 2c20 6053  odelingTask`, `S
+00000a80: 6571 7565 6e63 6543 6c61 7373 6966 6963  equenceClassific
+00000a90: 6174 696f 6e54 6173 6b60 2061 6e64 2060  ationTask` and `
+00000aa0: 5465 7874 5375 6d6d 6172 697a 6174 696f  TextSummarizatio
+00000ab0: 6e54 6173 6b60 3b20 6d6f 7265 2054 6173  nTask`; more Tas
+00000ac0: 6b73 2077 696c 6c20 636f 6d65 2073 6f6f  ks will come soo
+00000ad0: 6e21 0d0a 0d0a 2323 2055 7361 6765 0d0a  n!....## Usage..
+00000ae0: 0d0a 2a2a 4865 7265 2061 7265 205b 7475  ..**Here are [tu
+00000af0: 746f 7269 616c 735d 2864 6f63 732f 7475  torials](docs/tu
+00000b00: 746f 7269 616c 2928 636f 6e74 696e 7565  torial)(continue
+00000b10: 2075 7064 6174 696e 672e 2e2e 2920 666f   updating...) fo
+00000b20: 7220 7573 696e 6720 6061 7574 6f2d 6770  r using `auto-gp
+00000b30: 7471 602c 2069 7427 7320 6869 6768 6c79  tq`, it's highly
+00000b40: 2072 6563 6f6d 6d65 6e64 6564 2066 6f72   recommended for
+00000b50: 206e 6577 636f 6d65 7273 2074 6f20 7265   newcomers to re
+00000b60: 6164 2074 6865 6d20 6669 7273 7420 6265  ad them first be
+00000b70: 666f 7265 2074 7279 696e 6720 6578 616d  fore trying exam
+00000b80: 706c 6520 7363 7269 7074 732e 2a2a 200d  ple scripts.** .
+00000b90: 0a0d 0a23 2323 2042 6173 6963 0d0a 3e20  ...### Basic..> 
+00000ba0: 7761 726e 696e 673a 2074 6869 7320 6973  warning: this is
+00000bb0: 206a 7573 7420 6120 7368 6f77 2063 6173   just a show cas
+00000bc0: 6520 6f66 2074 6865 2075 7361 6765 206f  e of the usage o
+00000bd0: 6620 6261 7369 6320 6170 6973 2069 6e20  f basic apis in 
+00000be0: 4175 746f 4750 5451 2c20 7768 6963 6820  AutoGPTQ, which 
+00000bf0: 7573 6573 206f 6e6c 7920 6f6e 6520 7361  uses only one sa
+00000c00: 6d70 6c65 2074 6f20 7175 616e 7469 7a65  mple to quantize
+00000c10: 2061 206d 7563 6820 736d 616c 6c20 6d6f   a much small mo
+00000c20: 6465 6c2c 2074 6875 7320 6d61 7920 6e6f  del, thus may no
+00000c30: 7420 7065 7266 6f72 6d73 2061 7320 7765  t performs as we
+00000c40: 6c6c 2061 7320 6578 7065 6374 6564 2069  ll as expected i
+00000c50: 6e20 4c4c 4d73 2e0d 0a0d 0a42 656c 6f77  n LLMs.....Below
+00000c60: 2069 7320 616e 2065 7861 6d70 6c65 2066   is an example f
+00000c70: 6f72 2074 6865 2073 696d 706c 6573 7420  or the simplest 
+00000c80: 7573 6520 6f66 2060 6175 746f 5f67 7074  use of `auto_gpt
+00000c90: 7160 3a20 0d0a 6060 6070 7974 686f 6e0d  q`: ..```python.
+00000ca0: 0a66 726f 6d20 7472 616e 7366 6f72 6d65  .from transforme
+00000cb0: 7273 2069 6d70 6f72 7420 4175 746f 546f  rs import AutoTo
+00000cc0: 6b65 6e69 7a65 722c 2054 6578 7447 656e  kenizer, TextGen
+00000cd0: 6572 6174 696f 6e50 6970 656c 696e 650d  erationPipeline.
+00000ce0: 0a66 726f 6d20 6175 746f 5f67 7074 7120  .from auto_gptq 
+00000cf0: 696d 706f 7274 2041 7574 6f47 5054 5146  import AutoGPTQF
+00000d00: 6f72 4361 7573 616c 4c4d 2c20 4261 7365  orCausalLM, Base
+00000d10: 5175 616e 7469 7a65 436f 6e66 6967 0d0a  QuantizeConfig..
+00000d20: 0d0a 0d0a 7072 6574 7261 696e 6564 5f6d  ....pretrained_m
+00000d30: 6f64 656c 5f64 6972 203d 2022 6661 6365  odel_dir = "face
+00000d40: 626f 6f6b 2f6f 7074 2d31 3235 6d22 0d0a  book/opt-125m"..
+00000d50: 7175 616e 7469 7a65 645f 6d6f 6465 6c5f  quantized_model_
+00000d60: 6469 7220 3d20 226f 7074 2d31 3235 6d2d  dir = "opt-125m-
+00000d70: 3462 6974 220d 0a0d 0a0d 0a74 6f6b 656e  4bit"......token
+00000d80: 697a 6572 203d 2041 7574 6f54 6f6b 656e  izer = AutoToken
+00000d90: 697a 6572 2e66 726f 6d5f 7072 6574 7261  izer.from_pretra
+00000da0: 696e 6564 2870 7265 7472 6169 6e65 645f  ined(pretrained_
+00000db0: 6d6f 6465 6c5f 6469 722c 2075 7365 5f66  model_dir, use_f
+00000dc0: 6173 743d 5472 7565 290d 0a65 7861 6d70  ast=True)..examp
+00000dd0: 6c65 7320 3d20 5b0d 0a20 2020 2074 6f6b  les = [..    tok
+00000de0: 656e 697a 6572 280d 0a20 2020 2020 2020  enizer(..       
+00000df0: 2022 6175 746f 2d67 7074 7120 6973 2061   "auto-gptq is a
+00000e00: 6e20 6561 7379 2d74 6f2d 7573 6520 6d6f  n easy-to-use mo
+00000e10: 6465 6c20 7175 616e 7469 7a61 7469 6f6e  del quantization
+00000e20: 206c 6962 7261 7279 2077 6974 6820 7573   library with us
+00000e30: 6572 2d66 7269 656e 646c 7920 6170 6973  er-friendly apis
+00000e40: 2c20 6261 7365 6420 6f6e 2047 5054 5120  , based on GPTQ 
+00000e50: 616c 676f 7269 7468 6d2e 220d 0a20 2020  algorithm."..   
+00000e60: 2029 0d0a 5d0d 0a0d 0a71 7561 6e74 697a   )..]....quantiz
+00000e70: 655f 636f 6e66 6967 203d 2042 6173 6551  e_config = BaseQ
+00000e80: 7561 6e74 697a 6543 6f6e 6669 6728 0d0a  uantizeConfig(..
+00000e90: 2020 2020 6269 7473 3d34 2c20 2023 2071      bits=4,  # q
+00000ea0: 7561 6e74 697a 6520 6d6f 6465 6c20 746f  uantize model to
+00000eb0: 2034 2d62 6974 0d0a 2020 2020 6772 6f75   4-bit..    grou
+00000ec0: 705f 7369 7a65 3d31 3238 2c20 2023 2069  p_size=128,  # i
+00000ed0: 7420 6973 2072 6563 6f6d 6d65 6e64 6564  t is recommended
+00000ee0: 2074 6f20 7365 7420 7468 6520 7661 6c75   to set the valu
+00000ef0: 6520 746f 2031 3238 0d0a 290d 0a0d 0a23  e to 128..)....#
+00000f00: 206c 6f61 6420 756e 2d71 7561 6e74 697a   load un-quantiz
+00000f10: 6564 206d 6f64 656c 2c20 6279 2064 6566  ed model, by def
+00000f20: 6175 6c74 2c20 7468 6520 6d6f 6465 6c20  ault, the model 
+00000f30: 7769 6c6c 2061 6c77 6179 7320 6265 206c  will always be l
+00000f40: 6f61 6465 6420 696e 746f 2043 5055 206d  oaded into CPU m
+00000f50: 656d 6f72 790d 0a6d 6f64 656c 203d 2041  emory..model = A
+00000f60: 7574 6f47 5054 5146 6f72 4361 7573 616c  utoGPTQForCausal
+00000f70: 4c4d 2e66 726f 6d5f 7072 6574 7261 696e  LM.from_pretrain
+00000f80: 6564 2870 7265 7472 6169 6e65 645f 6d6f  ed(pretrained_mo
+00000f90: 6465 6c5f 6469 722c 2071 7561 6e74 697a  del_dir, quantiz
+00000fa0: 655f 636f 6e66 6967 290d 0a0d 0a23 2071  e_config)....# q
+00000fb0: 7561 6e74 697a 6520 6d6f 6465 6c2c 2074  uantize model, t
+00000fc0: 6865 2065 7861 6d70 6c65 7320 7368 6f75  he examples shou
+00000fd0: 6c64 2062 6520 6c69 7374 206f 6620 6469  ld be list of di
+00000fe0: 6374 2077 686f 7365 206b 6579 7320 6361  ct whose keys ca
+00000ff0: 6e20 6f6e 6c79 2062 6520 2269 6e70 7574  n only be "input
+00001000: 5f69 6473 2220 616e 6420 2261 7474 656e  _ids" and "atten
+00001010: 7469 6f6e 5f6d 6173 6b22 0d0a 6d6f 6465  tion_mask"..mode
+00001020: 6c2e 7175 616e 7469 7a65 2865 7861 6d70  l.quantize(examp
+00001030: 6c65 732c 2075 7365 5f74 7269 746f 6e3d  les, use_triton=
+00001040: 4661 6c73 6529 0d0a 0d0a 2320 7361 7665  False)....# save
+00001050: 2071 7561 6e74 697a 6564 206d 6f64 656c   quantized model
+00001060: 0d0a 6d6f 6465 6c2e 7361 7665 5f71 7561  ..model.save_qua
+00001070: 6e74 697a 6564 2871 7561 6e74 697a 6564  ntized(quantized
+00001080: 5f6d 6f64 656c 5f64 6972 290d 0a0d 0a23  _model_dir)....#
+00001090: 2073 6176 6520 7175 616e 7469 7a65 6420   save quantized 
+000010a0: 6d6f 6465 6c20 7573 696e 6720 7361 6665  model using safe
+000010b0: 7465 6e73 6f72 730d 0a6d 6f64 656c 2e73  tensors..model.s
+000010c0: 6176 655f 7175 616e 7469 7a65 6428 7175  ave_quantized(qu
+000010d0: 616e 7469 7a65 645f 6d6f 6465 6c5f 6469  antized_model_di
+000010e0: 722c 2075 7365 5f73 6166 6574 656e 736f  r, use_safetenso
+000010f0: 7273 3d54 7275 6529 0d0a 0d0a 2320 6c6f  rs=True)....# lo
+00001100: 6164 2071 7561 6e74 697a 6564 206d 6f64  ad quantized mod
+00001110: 656c 2074 6f20 7468 6520 6669 7273 7420  el to the first 
+00001120: 4750 550d 0a6d 6f64 656c 203d 2041 7574  GPU..model = Aut
+00001130: 6f47 5054 5146 6f72 4361 7573 616c 4c4d  oGPTQForCausalLM
+00001140: 2e66 726f 6d5f 7175 616e 7469 7a65 6428  .from_quantized(
+00001150: 7175 616e 7469 7a65 645f 6d6f 6465 6c5f  quantized_model_
+00001160: 6469 722c 2064 6576 6963 653d 2263 7564  dir, device="cud
+00001170: 613a 3022 2c20 7573 655f 7472 6974 6f6e  a:0", use_triton
+00001180: 3d46 616c 7365 290d 0a0d 0a23 2069 6e66  =False)....# inf
+00001190: 6572 656e 6365 2077 6974 6820 6d6f 6465  erence with mode
+000011a0: 6c2e 6765 6e65 7261 7465 0d0a 7072 696e  l.generate..prin
+000011b0: 7428 746f 6b65 6e69 7a65 722e 6465 636f  t(tokenizer.deco
+000011c0: 6465 286d 6f64 656c 2e67 656e 6572 6174  de(model.generat
+000011d0: 6528 2a2a 746f 6b65 6e69 7a65 7228 2261  e(**tokenizer("a
+000011e0: 7574 6f5f 6770 7471 2069 7322 2c20 7265  uto_gptq is", re
+000011f0: 7475 726e 5f74 656e 736f 7273 3d22 7074  turn_tensors="pt
+00001200: 2229 2e74 6f28 2263 7564 613a 3022 2929  ").to("cuda:0"))
+00001210: 5b30 5d29 290d 0a0d 0a23 206f 7220 796f  [0]))....# or yo
+00001220: 7520 6361 6e20 616c 736f 2075 7365 2070  u can also use p
+00001230: 6970 656c 696e 650d 0a70 6970 656c 696e  ipeline..pipelin
+00001240: 6520 3d20 5465 7874 4765 6e65 7261 7469  e = TextGenerati
+00001250: 6f6e 5069 7065 6c69 6e65 286d 6f64 656c  onPipeline(model
+00001260: 3d6d 6f64 656c 2c20 746f 6b65 6e69 7a65  =model, tokenize
+00001270: 723d 746f 6b65 6e69 7a65 7229 0d0a 7072  r=tokenizer)..pr
+00001280: 696e 7428 7069 7065 6c69 6e65 2822 6175  int(pipeline("au
+00001290: 746f 2d67 7074 7120 6973 2229 5b30 5d5b  to-gptq is")[0][
+000012a0: 2267 656e 6572 6174 6564 5f74 6578 7422  "generated_text"
+000012b0: 5d29 0d0a 6060 600d 0a0d 0a46 6f72 206d  ])..```....For m
+000012c0: 6f72 6520 6164 7661 6e63 6564 2066 6561  ore advanced fea
+000012d0: 7475 7265 7320 6f66 206d 6f64 656c 2071  tures of model q
+000012e0: 7561 6e74 697a 6174 696f 6e2c 2070 6c65  uantization, ple
+000012f0: 6173 6520 7265 6665 7265 6e63 6520 746f  ase reference to
+00001300: 205b 7468 6973 2073 6372 6970 745d 2865   [this script](e
+00001310: 7861 6d70 6c65 732f 7175 616e 7469 7a61  xamples/quantiza
+00001320: 7469 6f6e 2f71 7561 6e74 5f77 6974 685f  tion/quant_with_
+00001330: 616c 7061 6361 2e70 7929 0d0a 0d0a 2323  alpaca.py)....##
+00001340: 2320 4375 7374 6f6d 697a 6520 4d6f 6465  # Customize Mode
+00001350: 6c0d 0a42 656c 6f77 2069 7320 616e 2065  l..Below is an e
+00001360: 7861 6d70 6c65 2074 6f20 6578 7465 6e64  xample to extend
+00001370: 2060 6175 746f 5f67 7074 7160 2074 6f20   `auto_gptq` to 
+00001380: 7375 7070 6f72 7420 604f 5054 6020 6d6f  support `OPT` mo
+00001390: 6465 6c2c 2061 7320 796f 7520 7769 6c6c  del, as you will
+000013a0: 2073 6565 2c20 6974 2773 2076 6572 7920   see, it's very 
+000013b0: 6561 7379 3a0d 0a60 6060 7079 7468 6f6e  easy:..```python
+000013c0: 0d0a 6672 6f6d 2061 7574 6f5f 6770 7471  ..from auto_gptq
+000013d0: 2e6d 6f64 656c 696e 6720 696d 706f 7274  .modeling import
+000013e0: 2042 6173 6547 5054 5146 6f72 4361 7573   BaseGPTQForCaus
+000013f0: 616c 4c4d 0d0a 0d0a 0d0a 636c 6173 7320  alLM......class 
+00001400: 4f50 5447 5054 5146 6f72 4361 7573 616c  OPTGPTQForCausal
+00001410: 4c4d 2842 6173 6547 5054 5146 6f72 4361  LM(BaseGPTQForCa
+00001420: 7573 616c 4c4d 293a 0d0a 2020 2020 2320  usalLM):..    # 
+00001430: 6368 6169 6e65 6420 6174 7472 6962 7574  chained attribut
+00001440: 6520 6e61 6d65 206f 6620 7472 616e 7366  e name of transf
+00001450: 6f72 6d65 7220 6c61 7965 7220 626c 6f63  ormer layer bloc
+00001460: 6b0d 0a20 2020 206c 6179 6572 735f 626c  k..    layers_bl
+00001470: 6f63 6b5f 6e61 6d65 203d 2022 6d6f 6465  ock_name = "mode
+00001480: 6c2e 6465 636f 6465 722e 6c61 7965 7273  l.decoder.layers
+00001490: 220d 0a20 2020 2023 2063 6861 696e 6564  "..    # chained
+000014a0: 2061 7474 7269 6275 7465 206e 616d 6573   attribute names
+000014b0: 206f 6620 6f74 6865 7220 6e6e 206d 6f64   of other nn mod
+000014c0: 756c 6573 2074 6861 7420 696e 2074 6865  ules that in the
+000014d0: 2073 616d 6520 6c65 7665 6c20 6173 2074   same level as t
+000014e0: 6865 2074 7261 6e73 666f 726d 6572 206c  he transformer l
+000014f0: 6179 6572 2062 6c6f 636b 0d0a 2020 2020  ayer block..    
+00001500: 6f75 7473 6964 655f 6c61 7965 725f 6d6f  outside_layer_mo
+00001510: 6475 6c65 7320 3d20 5b0d 0a20 2020 2020  dules = [..     
+00001520: 2020 2022 6d6f 6465 6c2e 6465 636f 6465     "model.decode
+00001530: 722e 656d 6265 645f 746f 6b65 6e73 222c  r.embed_tokens",
+00001540: 2022 6d6f 6465 6c2e 6465 636f 6465 722e   "model.decoder.
+00001550: 656d 6265 645f 706f 7369 7469 6f6e 7322  embed_positions"
+00001560: 2c20 226d 6f64 656c 2e64 6563 6f64 6572  , "model.decoder
+00001570: 2e70 726f 6a65 6374 5f6f 7574 222c 0d0a  .project_out",..
+00001580: 2020 2020 2020 2020 226d 6f64 656c 2e64          "model.d
+00001590: 6563 6f64 6572 2e70 726f 6a65 6374 5f69  ecoder.project_i
+000015a0: 6e22 2c20 226d 6f64 656c 2e64 6563 6f64  n", "model.decod
+000015b0: 6572 2e66 696e 616c 5f6c 6179 6572 5f6e  er.final_layer_n
+000015c0: 6f72 6d22 0d0a 2020 2020 5d0d 0a20 2020  orm"..    ]..   
+000015d0: 2023 2063 6861 696e 6564 2061 7474 7269   # chained attri
+000015e0: 6275 7465 206e 616d 6573 206f 6620 6c69  bute names of li
+000015f0: 6e65 6172 206c 6179 6572 7320 696e 2074  near layers in t
+00001600: 7261 6e73 666f 726d 6572 206c 6179 6572  ransformer layer
+00001610: 206d 6f64 756c 650d 0a20 2020 2023 206e   module..    # n
+00001620: 6f72 6d61 6c6c 792c 2074 6865 7265 2061  ormally, there a
+00001630: 7265 2066 6f75 7220 7375 6220 6c69 7374  re four sub list
+00001640: 732c 2066 6f72 2065 6163 6820 6f6e 6520  s, for each one 
+00001650: 7468 6520 6d6f 6475 6c65 7320 696e 2069  the modules in i
+00001660: 7420 6361 6e20 6265 2073 6565 6e20 6173  t can be seen as
+00001670: 206f 6e65 206f 7065 7261 7469 6f6e 2c20   one operation, 
+00001680: 0d0a 2020 2020 2320 616e 6420 7468 6520  ..    # and the 
+00001690: 6f72 6465 7220 7368 6f75 6c64 2062 6520  order should be 
+000016a0: 7468 6520 6f72 6465 7220 7768 656e 2074  the order when t
+000016b0: 6865 7920 6172 6520 7472 756c 7920 6578  hey are truly ex
+000016c0: 6563 7574 6564 2c20 696e 2074 6869 7320  ecuted, in this 
+000016d0: 6361 7365 2028 616e 6420 7573 7561 6c6c  case (and usuall
+000016e0: 7920 696e 206d 6f73 7420 6361 7365 7329  y in most cases)
+000016f0: 2c20 0d0a 2020 2020 2320 7468 6579 2061  , ..    # they a
+00001700: 7265 3a20 6174 7465 6e74 696f 6e20 715f  re: attention q_
+00001710: 6b5f 7620 7072 6f6a 6563 7469 6f6e 2c20  k_v projection, 
+00001720: 6174 7465 6e74 696f 6e20 6f75 7470 7574  attention output
+00001730: 2070 726f 6a65 6374 696f 6e2c 204d 4c50   projection, MLP
+00001740: 2070 726f 6a65 6374 2069 6e70 7574 2c20   project input, 
+00001750: 4d4c 5020 7072 6f6a 6563 7420 6f75 7470  MLP project outp
+00001760: 7574 0d0a 2020 2020 696e 7369 6465 5f6c  ut..    inside_l
+00001770: 6179 6572 5f6d 6f64 756c 6573 203d 205b  ayer_modules = [
+00001780: 0d0a 2020 2020 2020 2020 5b22 7365 6c66  ..        ["self
+00001790: 5f61 7474 6e2e 6b5f 7072 6f6a 222c 2022  _attn.k_proj", "
+000017a0: 7365 6c66 5f61 7474 6e2e 765f 7072 6f6a  self_attn.v_proj
+000017b0: 222c 2022 7365 6c66 5f61 7474 6e2e 715f  ", "self_attn.q_
+000017c0: 7072 6f6a 225d 2c0d 0a20 2020 2020 2020  proj"],..       
+000017d0: 205b 2273 656c 665f 6174 746e 2e6f 7574   ["self_attn.out
+000017e0: 5f70 726f 6a22 5d2c 0d0a 2020 2020 2020  _proj"],..      
+000017f0: 2020 5b22 6663 3122 5d2c 0d0a 2020 2020    ["fc1"],..    
+00001800: 2020 2020 5b22 6663 3222 5d0d 0a20 2020      ["fc2"]..   
+00001810: 205d 0d0a 6060 600d 0a41 6674 6572 2074   ]..```..After t
+00001820: 6869 732c 2079 6f75 2063 616e 2075 7365  his, you can use
+00001830: 2060 4f50 5447 5054 5146 6f72 4361 7573   `OPTGPTQForCaus
+00001840: 616c 4c4d 2e66 726f 6d5f 7072 6574 7261  alLM.from_pretra
+00001850: 696e 6564 6020 616e 6420 6f74 6865 7220  ined` and other 
+00001860: 6d65 7468 6f64 7320 6173 2073 686f 776e  methods as shown
+00001870: 2069 6e20 4261 7369 632e 0d0a 0d0a 2323   in Basic.....##
+00001880: 2320 4576 616c 7561 7469 6f6e 206f 6e20  # Evaluation on 
+00001890: 446f 776e 7374 7265 616d 2054 6173 6b73  Downstream Tasks
+000018a0: 0d0a 596f 7520 6361 6e20 7573 6520 7461  ..You can use ta
+000018b0: 736b 7320 6465 6669 6e65 6420 696e 2060  sks defined in `
+000018c0: 6175 746f 5f67 7074 712e 6576 616c 5f74  auto_gptq.eval_t
+000018d0: 6173 6b73 6020 746f 2065 7661 6c75 6174  asks` to evaluat
+000018e0: 6520 6d6f 6465 6c27 7320 7065 7266 6f72  e model's perfor
+000018f0: 6d61 6e63 6520 6f6e 2073 7065 6369 6669  mance on specifi
+00001900: 6320 646f 776e 2d73 7472 6561 6d20 7461  c down-stream ta
+00001910: 736b 2062 6566 6f72 6520 616e 6420 6166  sk before and af
+00001920: 7465 7220 7175 616e 7469 7a61 7469 6f6e  ter quantization
+00001930: 2e0d 0a0d 0a54 6865 2070 7265 6465 6669  .....The predefi
+00001940: 6e65 6420 7461 736b 7320 7375 7070 6f72  ned tasks suppor
+00001950: 7420 616c 6c20 6361 7573 616c 2d6c 616e  t all causal-lan
+00001960: 6775 6167 652d 6d6f 6465 6c73 2069 6d70  guage-models imp
+00001970: 6c65 6d65 6e74 6564 2069 6e20 5bf0 9fa4  lemented in [...
+00001980: 9720 7472 616e 7366 6f72 6d65 7273 5d28  . transformers](
+00001990: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000019a0: 6f6d 2f68 7567 6769 6e67 6661 6365 2f74  om/huggingface/t
+000019b0: 7261 6e73 666f 726d 6572 7329 2061 6e64  ransformers) and
+000019c0: 2069 6e20 7468 6973 2070 726f 6a65 6374   in this project
+000019d0: 2e0d 0a0d 0a42 656c 6f77 2069 7320 616e  .....Below is an
+000019e0: 2065 7861 6d70 6c65 2074 6f20 6576 616c   example to eval
+000019f0: 7561 7465 2060 456c 6575 7468 6572 4149  uate `EleutherAI
+00001a00: 2f67 7074 2d6a 2d36 6260 206f 6e20 7365  /gpt-j-6b` on se
+00001a10: 7175 656e 6365 2d63 6c61 7373 6966 6963  quence-classific
+00001a20: 6174 696f 6e20 7461 736b 2075 7369 6e67  ation task using
+00001a30: 2060 6361 7264 6966 666e 6c70 2f74 7765   `cardiffnlp/twe
+00001a40: 6574 5f73 656e 7469 6d65 6e74 5f6d 756c  et_sentiment_mul
+00001a50: 7469 6c69 6e67 7561 6c60 2064 6174 6173  tilingual` datas
+00001a60: 6574 3a0d 0a60 6060 7079 7468 6f6e 0d0a  et:..```python..
+00001a70: 6672 6f6d 2066 756e 6374 6f6f 6c73 2069  from functools i
+00001a80: 6d70 6f72 7420 7061 7274 6961 6c0d 0a0d  mport partial...
+00001a90: 0a69 6d70 6f72 7420 6461 7461 7365 7473  .import datasets
+00001aa0: 0d0a 6672 6f6d 2074 7261 6e73 666f 726d  ..from transform
+00001ab0: 6572 7320 696d 706f 7274 2041 7574 6f54  ers import AutoT
+00001ac0: 6f6b 656e 697a 6572 2c20 4175 746f 4d6f  okenizer, AutoMo
+00001ad0: 6465 6c46 6f72 4361 7573 616c 4c4d 2c20  delForCausalLM, 
+00001ae0: 4765 6e65 7261 7469 6f6e 436f 6e66 6967  GenerationConfig
+00001af0: 0d0a 0d0a 6672 6f6d 2061 7574 6f5f 6770  ....from auto_gp
+00001b00: 7471 2069 6d70 6f72 7420 4175 746f 4750  tq import AutoGP
+00001b10: 5451 466f 7243 6175 7361 6c4c 4d2c 2042  TQForCausalLM, B
+00001b20: 6173 6551 7561 6e74 697a 6543 6f6e 6669  aseQuantizeConfi
+00001b30: 670d 0a66 726f 6d20 6175 746f 5f67 7074  g..from auto_gpt
+00001b40: 712e 6576 616c 5f74 6173 6b73 2069 6d70  q.eval_tasks imp
+00001b50: 6f72 7420 5365 7175 656e 6365 436c 6173  ort SequenceClas
+00001b60: 7369 6669 6361 7469 6f6e 5461 736b 0d0a  sificationTask..
+00001b70: 0d0a 0d0a 4d4f 4445 4c20 3d20 2245 6c65  ....MODEL = "Ele
+00001b80: 7574 6865 7241 492f 6770 742d 6a2d 3662  utherAI/gpt-j-6b
+00001b90: 220d 0a44 4154 4153 4554 203d 2022 6361  "..DATASET = "ca
+00001ba0: 7264 6966 666e 6c70 2f74 7765 6574 5f73  rdiffnlp/tweet_s
+00001bb0: 656e 7469 6d65 6e74 5f6d 756c 7469 6c69  entiment_multili
+00001bc0: 6e67 7561 6c22 0d0a 5445 4d50 4c41 5445  ngual"..TEMPLATE
+00001bd0: 203d 2022 5175 6573 7469 6f6e 3a57 6861   = "Question:Wha
+00001be0: 7427 7320 7468 6520 7365 6e74 696d 656e  t's the sentimen
+00001bf0: 7420 6f66 2074 6865 2067 6976 656e 2074  t of the given t
+00001c00: 6578 743f 2043 686f 6963 6573 2061 7265  ext? Choices are
+00001c10: 207b 6c61 6265 6c73 7d2e 5c6e 5465 7874   {labels}.\nText
+00001c20: 3a20 7b74 6578 747d 5c6e 416e 7377 6572  : {text}\nAnswer
+00001c30: 3a22 0d0a 4944 324c 4142 454c 203d 207b  :"..ID2LABEL = {
+00001c40: 0d0a 2020 2020 303a 2022 6e65 6761 7469  ..    0: "negati
+00001c50: 7665 222c 0d0a 2020 2020 313a 2022 6e65  ve",..    1: "ne
+00001c60: 7574 7261 6c22 2c0d 0a20 2020 2032 3a20  utral",..    2: 
+00001c70: 2270 6f73 6974 6976 6522 0d0a 7d0d 0a4c  "positive"..}..L
+00001c80: 4142 454c 5320 3d20 6c69 7374 2849 4432  ABELS = list(ID2
+00001c90: 4c41 4245 4c2e 7661 6c75 6573 2829 290d  LABEL.values()).
+00001ca0: 0a0d 0a0d 0a64 6566 2064 735f 7265 6661  .....def ds_refa
+00001cb0: 6374 6f72 5f66 6e28 7361 6d70 6c65 7329  ctor_fn(samples)
+00001cc0: 3a0d 0a20 2020 2074 6578 745f 6461 7461  :..    text_data
+00001cd0: 203d 2073 616d 706c 6573 5b22 7465 7874   = samples["text
+00001ce0: 225d 0d0a 2020 2020 6c61 6265 6c5f 6461  "]..    label_da
+00001cf0: 7461 203d 2073 616d 706c 6573 5b22 6c61  ta = samples["la
+00001d00: 6265 6c22 5d0d 0a0d 0a20 2020 206e 6577  bel"]....    new
+00001d10: 5f73 616d 706c 6573 203d 207b 2270 726f  _samples = {"pro
+00001d20: 6d70 7422 3a20 5b5d 2c20 226c 6162 656c  mpt": [], "label
+00001d30: 223a 205b 5d7d 0d0a 2020 2020 666f 7220  ": []}..    for 
+00001d40: 7465 7874 2c20 6c61 6265 6c20 696e 207a  text, label in z
+00001d50: 6970 2874 6578 745f 6461 7461 2c20 6c61  ip(text_data, la
+00001d60: 6265 6c5f 6461 7461 293a 0d0a 2020 2020  bel_data):..    
+00001d70: 2020 2020 7072 6f6d 7074 203d 2054 454d      prompt = TEM
+00001d80: 504c 4154 452e 666f 726d 6174 286c 6162  PLATE.format(lab
+00001d90: 656c 733d 4c41 4245 4c53 2c20 7465 7874  els=LABELS, text
+00001da0: 3d74 6578 7429 0d0a 2020 2020 2020 2020  =text)..        
+00001db0: 6e65 775f 7361 6d70 6c65 735b 2270 726f  new_samples["pro
+00001dc0: 6d70 7422 5d2e 6170 7065 6e64 2870 726f  mpt"].append(pro
+00001dd0: 6d70 7429 0d0a 2020 2020 2020 2020 6e65  mpt)..        ne
+00001de0: 775f 7361 6d70 6c65 735b 226c 6162 656c  w_samples["label
+00001df0: 225d 2e61 7070 656e 6428 4944 324c 4142  "].append(ID2LAB
+00001e00: 454c 5b6c 6162 656c 5d29 0d0a 0d0a 2020  EL[label])....  
+00001e10: 2020 7265 7475 726e 206e 6577 5f73 616d    return new_sam
+00001e20: 706c 6573 0d0a 0d0a 0d0a 2320 206d 6f64  ples......#  mod
+00001e30: 656c 203d 2041 7574 6f4d 6f64 656c 466f  el = AutoModelFo
+00001e40: 7243 6175 7361 6c4c 4d2e 6672 6f6d 5f70  rCausalLM.from_p
+00001e50: 7265 7472 6169 6e65 6428 4d4f 4445 4c29  retrained(MODEL)
+00001e60: 2e65 7661 6c28 292e 6861 6c66 2829 2e74  .eval().half().t
+00001e70: 6f28 2263 7564 613a 3022 290d 0a6d 6f64  o("cuda:0")..mod
+00001e80: 656c 203d 2041 7574 6f47 5054 5146 6f72  el = AutoGPTQFor
+00001e90: 4361 7573 616c 4c4d 2e66 726f 6d5f 7072  CausalLM.from_pr
+00001ea0: 6574 7261 696e 6564 284d 4f44 454c 2c20  etrained(MODEL, 
+00001eb0: 4261 7365 5175 616e 7469 7a65 436f 6e66  BaseQuantizeConf
+00001ec0: 6967 2829 290d 0a74 6f6b 656e 697a 6572  ig())..tokenizer
+00001ed0: 203d 2041 7574 6f54 6f6b 656e 697a 6572   = AutoTokenizer
+00001ee0: 2e66 726f 6d5f 7072 6574 7261 696e 6564  .from_pretrained
+00001ef0: 284d 4f44 454c 290d 0a0d 0a74 6173 6b20  (MODEL)....task 
+00001f00: 3d20 5365 7175 656e 6365 436c 6173 7369  = SequenceClassi
+00001f10: 6669 6361 7469 6f6e 5461 736b 280d 0a20  ficationTask(.. 
+00001f20: 2020 2020 2020 206d 6f64 656c 3d6d 6f64         model=mod
+00001f30: 656c 2c0d 0a20 2020 2020 2020 2074 6f6b  el,..        tok
+00001f40: 656e 697a 6572 3d74 6f6b 656e 697a 6572  enizer=tokenizer
+00001f50: 2c0d 0a20 2020 2020 2020 2063 6c61 7373  ,..        class
+00001f60: 6573 3d4c 4142 454c 532c 0d0a 2020 2020  es=LABELS,..    
+00001f70: 2020 2020 6461 7461 5f6e 616d 655f 6f72      data_name_or
+00001f80: 5f70 6174 683d 4441 5441 5345 542c 0d0a  _path=DATASET,..
+00001f90: 2020 2020 2020 2020 7072 6f6d 7074 5f63          prompt_c
+00001fa0: 6f6c 5f6e 616d 653d 2270 726f 6d70 7422  ol_name="prompt"
+00001fb0: 2c0d 0a20 2020 2020 2020 206c 6162 656c  ,..        label
+00001fc0: 5f63 6f6c 5f6e 616d 653d 226c 6162 656c  _col_name="label
+00001fd0: 222c 0d0a 2020 2020 2020 2020 2a2a 7b0d  ",..        **{.
+00001fe0: 0a20 2020 2020 2020 2020 2020 2022 6e75  .            "nu
+00001ff0: 6d5f 7361 6d70 6c65 7322 3a20 3130 3030  m_samples": 1000
+00002000: 2c20 2023 2068 6f77 206d 616e 7920 7361  ,  # how many sa
+00002010: 6d70 6c65 7320 7769 6c6c 2062 6520 7361  mples will be sa
+00002020: 6d70 6c65 6420 746f 2065 7661 6c75 6174  mpled to evaluat
+00002030: 696f 6e0d 0a20 2020 2020 2020 2020 2020  ion..           
+00002040: 2022 7361 6d70 6c65 5f6d 6178 5f6c 656e   "sample_max_len
+00002050: 223a 2031 3032 342c 2020 2320 6d61 7820  ": 1024,  # max 
+00002060: 746f 6b65 6e73 2066 6f72 2065 6163 6820  tokens for each 
+00002070: 7361 6d70 6c65 0d0a 2020 2020 2020 2020  sample..        
+00002080: 2020 2020 2262 6c6f 636b 5f6d 6178 5f6c      "block_max_l
+00002090: 656e 223a 2032 3034 382c 2020 2320 6d61  en": 2048,  # ma
+000020a0: 7820 746f 6b65 6e73 2066 6f72 2065 6163  x tokens for eac
+000020b0: 6820 6461 7461 2062 6c6f 636b 0d0a 2020  h data block..  
+000020c0: 2020 2020 2020 2020 2020 2320 6675 6e63            # func
+000020d0: 7469 6f6e 2074 6f20 6c6f 6164 2064 6174  tion to load dat
+000020e0: 6173 6574 2c20 6f6e 6520 6d75 7374 206f  aset, one must o
+000020f0: 6e6c 7920 6163 6365 7074 2064 6174 615f  nly accept data_
+00002100: 6e61 6d65 5f6f 725f 7061 7468 2061 7320  name_or_path as 
+00002110: 696e 7075 7420 0d0a 2020 2020 2020 2020  input ..        
+00002120: 2020 2020 2320 616e 6420 7265 7475 726e      # and return
+00002130: 2064 6174 6173 6574 732e 4461 7461 7365   datasets.Datase
+00002140: 740d 0a20 2020 2020 2020 2020 2020 2022  t..            "
+00002150: 6c6f 6164 5f66 6e22 3a20 7061 7274 6961  load_fn": partia
+00002160: 6c28 6461 7461 7365 7473 2e6c 6f61 645f  l(datasets.load_
+00002170: 6461 7461 7365 742c 206e 616d 653d 2265  dataset, name="e
+00002180: 6e67 6c69 7368 2229 2c20 200d 0a20 2020  nglish"),  ..   
+00002190: 2020 2020 2020 2020 2023 2066 756e 6374           # funct
+000021a0: 696f 6e20 746f 2070 7265 7072 6f63 6573  ion to preproces
+000021b0: 7320 6461 7461 7365 742c 2077 6869 6368  s dataset, which
+000021c0: 2069 7320 7573 6564 2066 6f72 2064 6174   is used for dat
+000021d0: 6173 6574 732e 4461 7461 7365 742e 6d61  asets.Dataset.ma
+000021e0: 702c 200d 0a20 2020 2020 2020 2020 2020  p, ..           
+000021f0: 2023 206d 7573 7420 7265 7475 726e 2044   # must return D
+00002200: 6963 745b 7374 722c 206c 6973 745d 2077  ict[str, list] w
+00002210: 6974 6820 6f6e 6c79 2074 776f 206b 6579  ith only two key
+00002220: 733a 205b 7072 6f6d 7074 5f63 6f6c 5f6e  s: [prompt_col_n
+00002230: 616d 652c 206c 6162 656c 5f63 6f6c 5f6e  ame, label_col_n
+00002240: 616d 655d 0d0a 2020 2020 2020 2020 2020  ame]..          
+00002250: 2020 2270 7265 7072 6f63 6573 735f 666e    "preprocess_fn
+00002260: 223a 2064 735f 7265 6661 6374 6f72 5f66  ": ds_refactor_f
+00002270: 6e2c 2020 0d0a 2020 2020 2020 2020 2020  n,  ..          
+00002280: 2020 2320 7472 756e 6361 7465 206c 6162    # truncate lab
+00002290: 656c 2077 6865 6e20 7361 6d70 6c65 2773  el when sample's
+000022a0: 206c 656e 6774 6820 6578 6365 6564 2073   length exceed s
+000022b0: 616d 706c 655f 6d61 785f 6c65 6e0d 0a20  ample_max_len.. 
+000022c0: 2020 2020 2020 2020 2020 2022 7472 756e             "trun
+000022d0: 6361 7465 5f70 726f 6d70 7422 3a20 4661  cate_prompt": Fa
+000022e0: 6c73 6520 200d 0a20 2020 2020 2020 207d  lse  ..        }
+000022f0: 0d0a 2020 2020 290d 0a0d 0a23 206e 6f74  ..    )....# not
+00002300: 6520 7468 6174 206d 6178 5f6e 6577 5f74  e that max_new_t
+00002310: 6f6b 656e 7320 7769 6c6c 2062 6520 6175  okens will be au
+00002320: 746f 6d61 7469 6361 6c6c 7920 7370 6563  tomatically spec
+00002330: 6966 6965 6420 696e 7465 726e 616c 6c79  ified internally
+00002340: 2062 6173 6564 206f 6e20 6769 7665 6e20   based on given 
+00002350: 636c 6173 7365 730d 0a70 7269 6e74 2874  classes..print(t
+00002360: 6173 6b2e 7275 6e28 2929 0d0a 0d0a 2320  ask.run())....# 
+00002370: 7365 6c66 2d63 6f6e 7369 7374 656e 6379  self-consistency
+00002380: 0d0a 7072 696e 7428 0d0a 2020 2020 7461  ..print(..    ta
+00002390: 736b 2e72 756e 280d 0a20 2020 2020 2020  sk.run(..       
+000023a0: 2067 656e 6572 6174 696f 6e5f 636f 6e66   generation_conf
+000023b0: 6967 3d47 656e 6572 6174 696f 6e43 6f6e  ig=GenerationCon
+000023c0: 6669 6728 0d0a 2020 2020 2020 2020 2020  fig(..          
+000023d0: 2020 6e75 6d5f 6265 616d 733d 332c 0d0a    num_beams=3,..
+000023e0: 2020 2020 2020 2020 2020 2020 6e75 6d5f              num_
+000023f0: 7265 7475 726e 5f73 6571 7565 6e63 6573  return_sequences
+00002400: 3d33 2c0d 0a20 2020 2020 2020 2020 2020  =3,..           
+00002410: 2064 6f5f 7361 6d70 6c65 3d54 7275 650d   do_sample=True.
+00002420: 0a20 2020 2020 2020 2029 0d0a 2020 2020  .        )..    
+00002430: 290d 0a29 0d0a 6060 600d 0a0d 0a23 2323  )..)..```....###
+00002440: 204d 6f72 6520 4578 616d 706c 6573 0d0a   More Examples..
+00002450: 466f 7220 6d6f 7265 2065 7861 6d70 6c65  For more example
+00002460: 732c 2070 6c65 6173 6520 7475 726e 2074  s, please turn t
+00002470: 6f20 5b65 7861 6d70 6c65 735d 2865 7861  o [examples](exa
+00002480: 6d70 6c65 732f 5245 4144 4d45 2e6d 6429  mples/README.md)
+00002490: 0d0a 0d0a 2323 2041 636b 6e6f 776c 6564  ....## Acknowled
+000024a0: 6765 6d65 6e74 0d0a 2d20 5370 6563 6961  gement..- Specia
+000024b0: 6c6c 7920 7468 616e 6b73 202a 2a45 6c69  lly thanks **Eli
+000024c0: 6173 2046 7261 6e74 6172 2a2a 2c20 2a2a  as Frantar**, **
+000024d0: 5361 6c65 6820 4173 686b 626f 6f73 2a2a  Saleh Ashkboos**
+000024e0: 2c20 2a2a 546f 7273 7465 6e20 486f 6566  , **Torsten Hoef
+000024f0: 6c65 722a 2a20 616e 6420 2a2a 4461 6e20  ler** and **Dan 
+00002500: 416c 6973 7461 7268 2a2a 2066 6f72 2070  Alistarh** for p
+00002510: 726f 706f 7369 6e67 202a 2a47 5054 512a  roposing **GPTQ*
+00002520: 2a20 616c 676f 7269 7468 6d20 616e 6420  * algorithm and 
+00002530: 6f70 656e 2073 6f75 7263 6520 7468 6520  open source the 
+00002540: 5b63 6f64 655d 2868 7474 7073 3a2f 2f67  [code](https://g
+00002550: 6974 6875 622e 636f 6d2f 4953 542d 4441  ithub.com/IST-DA
+00002560: 534c 6162 2f67 7074 7129 2e0d 0a2d 2053  SLab/gptq)...- S
+00002570: 7065 6369 616c 6c79 2074 6861 6e6b 7320  pecially thanks 
+00002580: 2a2a 7177 6f70 7177 6f70 3230 302a 2a2c  **qwopqwop200**,
+00002590: 2066 6f72 2063 6f64 6520 696e 2074 6869   for code in thi
+000025a0: 7320 7072 6f6a 6563 7420 7468 6174 2072  s project that r
+000025b0: 656c 6576 616e 7420 746f 2071 7561 6e74  elevant to quant
+000025c0: 697a 6174 696f 6e20 6172 6520 6d61 696e  ization are main
+000025d0: 6c79 2072 6566 6572 656e 6365 6420 6672  ly referenced fr
+000025e0: 6f6d 205b 4750 5451 2d66 6f72 2d4c 4c61  om [GPTQ-for-LLa
+000025f0: 4d61 5d28 6874 7470 733a 2f2f 6769 7468  Ma](https://gith
+00002600: 7562 2e63 6f6d 2f71 776f 7071 776f 7032  ub.com/qwopqwop2
+00002610: 3030 2f47 5054 512d 666f 722d 4c4c 614d  00/GPTQ-for-LLaM
+00002620: 612f 7472 6565 2f63 7564 6129 2e0d 0a    a/tree/cuda)...
```

### Comparing `auto_gptq-0.0.5/auto_gptq/eval_tasks/_base.py` & `auto_gptq-0.1.0/auto_gptq/eval_tasks/_base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-from abc import abstractmethod
-from typing import Any, Dict, List, Optional, Union
-
-import torch
-from transformers import PreTrainedTokenizer, PreTrainedModel
-
-from ._utils.data_utils import get_dataloader
-from ..modeling import BaseGPTQForCausalLM
-
-
-class BaseTask:
-    def __init__(
-        self,
-        model: Union[BaseGPTQForCausalLM, PreTrainedModel],
-        tokenizer: PreTrainedTokenizer,
-        data_name_or_path: str,
-        prompt_col_name: str,
-        label_col_name: str,
-        device: Optional[str] = None,
-        **kwargs
-    ):
-        self.model = model
-        self.tokenizer = tokenizer
-        if self.tokenizer.pad_token_id is None:
-            self.tokenizer.pad_token = self.tokenizer.eos_token
-            self.tokenizer.pad_token_id = self.tokenizer.eos_token_id
-            self.model.config.pad_token_id = self.tokenizer.eos_token_id
-        self.dl = get_dataloader(
-            data_name_or_path,
-            prompt_col_name=prompt_col_name,
-            label_col_name=label_col_name,
-            tokenizer=tokenizer,
-            **kwargs
-        )
-
-        self.device = device
-        if not self.device:
-            self.device = self.model.device
-        if isinstance(self.device, str):
-            self.device = torch.device(self.device)
-
-    @abstractmethod
-    def _predict(self, batch_data: Dict[str, Any], **kwargs) -> List[Any]:
-        pass
-
-    @abstractmethod
-    def _parse_labels(self, label_ids: torch.LongTensor) -> List[Any]:
-        pass
-
-    @abstractmethod
-    def _metric(self, pred: List[Any], label: List[Any]) -> Dict[str, float]:
-        pass
-
-    def run(self, **predict_kwargs) -> Dict[str, float]:
-        with torch.inference_mode(), torch.amp.autocast(device_type=self.device.type):
-            predictions = []
-            labels = []
-            for batch_data in self.dl:
-                for k, v in batch_data.items():
-                    if isinstance(v, torch.Tensor):
-                        batch_data[k] = v.to(self.device)
-                labels += self._parse_labels(batch_data["labels"])
-                predictions += self._predict(batch_data, **predict_kwargs)
-
-        return self._metric(predictions, labels)
+from abc import abstractmethod
+from typing import Any, Dict, List, Optional, Union
+
+import torch
+from transformers import PreTrainedTokenizer, PreTrainedModel
+
+from ..modeling import BaseGPTQForCausalLM
+from ..utils.data_utils import get_dataloader
+
+
+class BaseTask:
+    def __init__(
+        self,
+        model: Union[BaseGPTQForCausalLM, PreTrainedModel],
+        tokenizer: PreTrainedTokenizer,
+        data_name_or_path: str,
+        prompt_col_name: str,
+        label_col_name: str,
+        device: Optional[str] = None,
+        **kwargs
+    ):
+        self.model = model
+        self.tokenizer = tokenizer
+        if self.tokenizer.pad_token_id is None:
+            self.tokenizer.pad_token = self.tokenizer.eos_token
+            self.tokenizer.pad_token_id = self.tokenizer.eos_token_id
+            self.model.config.pad_token_id = self.tokenizer.eos_token_id
+        self.dl = get_dataloader(
+            data_name_or_path,
+            prompt_col_name=prompt_col_name,
+            label_col_name=label_col_name,
+            tokenizer=tokenizer,
+            **kwargs
+        )
+
+        self.device = device
+        if not self.device:
+            self.device = self.model.device
+        if isinstance(self.device, str):
+            self.device = torch.device(self.device)
+
+    @abstractmethod
+    def _predict(self, batch_data: Dict[str, Any], **kwargs) -> List[Any]:
+        pass
+
+    @abstractmethod
+    def _parse_labels(self, label_ids: torch.LongTensor) -> List[Any]:
+        pass
+
+    @abstractmethod
+    def _metric(self, pred: List[Any], label: List[Any]) -> Dict[str, float]:
+        pass
+
+    def run(self, **predict_kwargs) -> Dict[str, float]:
+        with torch.inference_mode(), torch.amp.autocast(device_type=self.device.type):
+            predictions = []
+            labels = []
+            for batch_data in self.dl:
+                for k, v in batch_data.items():
+                    if isinstance(v, torch.Tensor):
+                        batch_data[k] = v.to(self.device)
+                labels += self._parse_labels(batch_data["labels"])
+                predictions += self._predict(batch_data, **predict_kwargs)
+
+        return self._metric(predictions, labels)
```

### Comparing `auto_gptq-0.0.5/auto_gptq/eval_tasks/_utils/classification_utils.py` & `auto_gptq-0.1.0/auto_gptq/eval_tasks/_utils/classification_utils.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-import sys
-from typing import List, Sequence
-
-import numpy as np
-
-
-def levenshtein_distance(seq1: Sequence, seq2: Sequence):
-    if seq1 == seq2:
-        return 0
-    num_rows = len(seq1) + 1
-    num_cols = len(seq2) + 1
-    dp_matrix = np.empty((num_rows, num_cols))
-    dp_matrix[0, :] = range(num_cols)
-    dp_matrix[:, 0] = range(num_rows)
-
-    for i in range(1, num_rows):
-        for j in range(1, num_cols):
-            if seq1[i - 1] == seq2[j - 1]:
-                dp_matrix[i, j] = dp_matrix[i - 1, j - 1]
-            else:
-                dp_matrix[i, j] = min(dp_matrix[i - 1, j - 1], dp_matrix[i - 1, j], dp_matrix[i, j - 1]) + 1
-
-    return dp_matrix[num_rows - 1, num_cols - 1]
-
-
-def get_closest_label(pred: Sequence, classes: List[Sequence]) -> int:
-    min_id = sys.maxsize
-    min_edit_distance = sys.maxsize
-    for i, class_label in enumerate(classes):
-        edit_distance = levenshtein_distance(pred, class_label)
-        if edit_distance < min_edit_distance:
-            min_id = i
-            min_edit_distance = edit_distance
-    return min_id
-
-
-__all__ = ["levenshtein_distance", "get_closest_label"]
+import sys
+from typing import List, Sequence
+
+import numpy as np
+
+
+def levenshtein_distance(seq1: Sequence, seq2: Sequence):
+    if seq1 == seq2:
+        return 0
+    num_rows = len(seq1) + 1
+    num_cols = len(seq2) + 1
+    dp_matrix = np.empty((num_rows, num_cols))
+    dp_matrix[0, :] = range(num_cols)
+    dp_matrix[:, 0] = range(num_rows)
+
+    for i in range(1, num_rows):
+        for j in range(1, num_cols):
+            if seq1[i - 1] == seq2[j - 1]:
+                dp_matrix[i, j] = dp_matrix[i - 1, j - 1]
+            else:
+                dp_matrix[i, j] = min(dp_matrix[i - 1, j - 1], dp_matrix[i - 1, j], dp_matrix[i, j - 1]) + 1
+
+    return dp_matrix[num_rows - 1, num_cols - 1]
+
+
+def get_closest_label(pred: Sequence, classes: List[Sequence]) -> int:
+    min_id = sys.maxsize
+    min_edit_distance = sys.maxsize
+    for i, class_label in enumerate(classes):
+        edit_distance = levenshtein_distance(pred, class_label)
+        if edit_distance < min_edit_distance:
+            min_id = i
+            min_edit_distance = edit_distance
+    return min_id
+
+
+__all__ = ["levenshtein_distance", "get_closest_label"]
```

### Comparing `auto_gptq-0.0.5/auto_gptq/eval_tasks/_utils/data_utils.py` & `auto_gptq-0.1.0/auto_gptq/utils/data_utils.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,267 +1,267 @@
-import copy
-import random
-from functools import partial
-from typing import Callable, Dict, List, Optional
-
-import torch
-from datasets import load_dataset, DatasetDict, IterableDatasetDict
-from torch import LongTensor
-from torch.utils.data import DataLoader
-from transformers import PreTrainedTokenizer
-
-
-def make_data_block(
-    samples: Dict[str, List[str]],
-    prompt_col_name: str,
-    label_col_name: str,
-    tokenizer: PreTrainedTokenizer,
-    preprocess_fn: Optional[Callable] = None,
-    sample_max_len: int = 1024,
-    block_max_len: int = 2048,
-    add_eos_token: bool = False,
-    truncate_prompt: bool = True,
-    merge_prompt_label: bool = False
-) -> Dict[str, List[LongTensor]]:
-    """A simple implementation of text generation oriented smart batching to maximize VRAM usage when evaluation
-
-    :param samples: Dict[str, List[str]], samples that used to make data blocks
-    :param prompt_col_name: str, name of the key in samples whose value stores prompt
-    :param label_col_name: str, name of the key in samples whose value stores label
-    :param tokenizer: transformers.PretrainedTokenizer, tokenizer that used to tokenize samples
-    :param preprocess_fn: Optional[Callable], optional function that used to preprocess samples such as
-        refactor the data structure of samples, note the output of this function must be a dict whose keys
-        at least contains `prompt_col_name` and `label_col_name`
-    :param sample_max_len: int, defaults to 1024, max tokens number of each sample (before padding)
-    :param block_max_len: int, defaults to 2048, max tokens number of each data block (after padding)
-    :param add_eos_token: bool, defaults to False, whether add eos_token or not to the label
-    :param truncate_prompt: bool, defaults to True, whether to truncate prompt if the sample's total tokens
-        number exceeds `sample_max_len`, if not, will truncate label and drop this sample when all tokens
-        in label are truncated
-    :param merge_prompt_label: bool, defaults to False, will merge label into prompt if set to True, usually
-        this only required when doing language modeling task
-    :return: Dict[str, List[torch.LongTensor]], a dict whose keys are `input_ids`, `attention_mask` and
-        `label` and values are a list of torch.LongTensor
-    """
-    if preprocess_fn:
-        samples = preprocess_fn(samples)
-
-    prompts = samples[prompt_col_name]
-    labels = samples[label_col_name]
-
-    # tokenize samples
-    tokenized_prompts = tokenizer(prompts, truncation=False)["input_ids"]
-    tokenized_labels = tokenizer(labels, truncation=False)["input_ids"]
-
-    # filter tokenized samples by length
-    dropped_indices = []
-    for idx, (tokenized_prompt, tokenized_label) in enumerate(zip(tokenized_prompts, tokenized_labels)):
-        if add_eos_token:
-            tokenized_label += [tokenizer.eos_token_id]
-        len_prompt = len(tokenized_prompt)
-        len_label = len(tokenized_label)
-        exceed_len = len_prompt + len_label - sample_max_len
-        if exceed_len > 0:
-            if truncate_prompt:
-                tokenized_prompt = tokenized_prompt[exceed_len:]
-            else:
-                tokenized_label = tokenized_label[: -exceed_len]
-        tokenized_prompts[idx] = tokenized_prompt
-        tokenized_labels[idx] = tokenized_label
-        if not tokenized_label:
-            dropped_indices.append(idx)
-
-    # make data blocks of samples
-    tokenized_samples = sorted(
-        [
-            (p, l) for idx, (p, l) in enumerate(zip(tokenized_prompts, tokenized_labels))
-            if idx not in dropped_indices
-        ],
-        key=lambda x: (len(x[0]) + len(x[1])) if merge_prompt_label else len(x[0])
-    )
-    sample_blocks = []
-    sample_block = []
-    blk_max_len = 0
-    blk_total_len = 0
-    for tokenized_sample in tokenized_samples:
-        prompt_ids, label_ids = tokenized_sample
-        ori_sample_len = len(prompt_ids)
-        if merge_prompt_label:
-            ori_sample_len += len(label_ids)
-        if ori_sample_len <= blk_max_len:
-            additional_len = blk_max_len
-            sample_len = blk_max_len
-        else:
-            additional_len = len(sample_block) * (ori_sample_len - blk_max_len) + ori_sample_len
-            sample_len = ori_sample_len
-
-        if blk_total_len + additional_len > block_max_len:
-            sample_blocks.append((copy.copy(sample_block), blk_max_len))
-            sample_block = []
-            blk_max_len = 0
-            blk_total_len = 0
-            sample_len = ori_sample_len
-            additional_len = ori_sample_len
-
-        sample_block.append(tokenized_sample)
-        blk_max_len = max(blk_max_len, sample_len)
-        blk_total_len += additional_len
-
-    if sample_block:
-        sample_blocks.append((copy.copy(sample_block), blk_max_len))
-    del sample_block
-    del blk_max_len
-    del blk_total_len
-
-    new_samples = {
-        "input_ids": [],
-        "attention_mask": [],
-        "labels": []
-    }
-    # padding each data block internally
-    for block, blk_max_len in sample_blocks:
-        input_ids = []
-        attention_mask = []
-        label_ids = []
-        label_max_len = max([len(sample[1]) for sample in block])
-
-        for sample in block:
-            tokenized_prompt, tokenized_label = sample
-            sample_len = len(tokenized_prompt)
-            if merge_prompt_label:
-                sample_len += len(tokenized_label)
-            pad_num = blk_max_len - sample_len
-            if merge_prompt_label:
-                input_ids.append([tokenizer.pad_token_id] * pad_num + tokenized_prompt + tokenized_label)
-                label_ids.append([-100] * (pad_num + len(tokenized_prompt)) + tokenized_label)
-            else:
-                input_ids.append([tokenizer.pad_token_id] * pad_num + tokenized_prompt)
-                label_ids.append([-100] * (label_max_len - len(tokenized_label)) + tokenized_label)
-            attention_mask.append([0] * pad_num + [1] * sample_len)
-
-        new_samples["input_ids"].append(input_ids)
-        new_samples["attention_mask"].append(attention_mask)
-        new_samples["labels"].append(label_ids)
-
-    return new_samples
-
-
-def collate_data(blocks: List[Dict[str, List[List[int]]]], pad_token_id: int) -> Dict[str, LongTensor]:
-    def pad_block(block, pads):
-        return torch.cat((pads.to(block.device), block), dim=-1)
-
-    input_ids_blocks = [LongTensor(block["input_ids"]) for block in blocks]
-    attention_mask_blocks = [LongTensor(block["attention_mask"]) for block in blocks]
-    label_blocks = [LongTensor(block["labels"]) for block in blocks]
-
-    bsz = len(blocks)
-    inp_max_len = max([block.size(-1) for block in input_ids_blocks])
-    label_max_len = max([block.size(-1) for block in label_blocks])
-
-    for i in range(bsz):
-        block_bsz, block_inp_len = input_ids_blocks[i].shape
-        block_label_len = label_blocks[i].shape[-1]
-        pad_num = inp_max_len - block_inp_len
-        if pad_num > 0:
-            input_ids_blocks[i] = pad_block(input_ids_blocks[i], torch.ones((block_bsz, pad_num)) * pad_token_id)
-            attention_mask_blocks[i] = pad_block(attention_mask_blocks[i], torch.zeros((block_bsz, pad_num)))
-        label_pad_num = label_max_len - block_label_len
-        if label_pad_num > 0:
-            label_blocks[i] = pad_block(label_blocks[i], torch.ones((block_bsz, label_pad_num)) * -100)
-
-    return {
-        "input_ids": torch.cat(input_ids_blocks, dim=0).long(),
-        "attention_mask": torch.cat(attention_mask_blocks, dim=0).long(),
-        "labels": torch.cat(label_blocks, dim=0).long()
-    }
-
-
-def get_dataloader(
-    data_path_or_name: str,
-    prompt_col_name: str,
-    label_col_name: str,
-    tokenizer: PreTrainedTokenizer,
-    load_fn: Optional[Callable] = None,
-    preprocess_fn: Optional[Callable] = None,
-    num_samples: int = 128,
-    sample_max_len: int = 1024,
-    block_max_len: int = 2048,
-    add_eos_token: bool = False,
-    truncate_prompt: bool = True,
-    merge_prompt_label: bool = False,
-    load_fn_kwargs: Optional[dict] = None,
-    preprocess_fn_kwargs: Optional[dict] = None,
-    **kwargs
-) -> DataLoader:
-    """load dataset and build dataloader
-
-    :param data_path_or_name: str, dataset name in hf-hub or local file path
-    :param prompt_col_name: str, see `make_data_block`
-    :param label_col_name: str, see `make_data_block`
-    :param tokenizer: str, see `make_data_block`
-    :param load_fn: Optional[Callable], defaults to None, function used to load dataset, if not specified,
-        use `datasets.load_dataset`
-    :param preprocess_fn: Optional[Callable], see `make_data_block`
-    :param num_samples: int, defaults to 128, total samples used to evaluation
-    :param sample_max_len: int, see `make_data_block`
-    :param block_max_len: int, see `make_data_block`
-    :param add_eos_token: bool, see `make_data_block`
-    :param truncate_prompt: bool, see `make_data_block`
-    :param merge_prompt_label: bool, see `make_data_block`
-    :param load_fn_kwargs: Optional[dict], defaults to None, keyword arguments used
-        for `load_fn` or `datasets.load_dataset`
-    :param preprocess_fn_kwargs: Optional[dict], defaults to None, keyword arguments used
-        for `preprocess_fn`
-    :param kwargs: additional keyword arguments will be passed to torch's `DataLoader` initialization,
-        note values of `batch_size`, `shuffle` and `collate_fn` will always be overridden to fixed value
-    :return: torch.utils.data.DataLoader
-    """
-
-    if not load_fn_kwargs:
-        load_fn_kwargs = dict()
-    if not preprocess_fn_kwargs:
-        preprocess_fn_kwargs = dict()
-
-    if load_fn:
-        ds = load_fn(data_path_or_name, **load_fn_kwargs)
-    else:
-        ds = load_dataset(data_path_or_name, **load_fn_kwargs)
-    if isinstance(ds, (DatasetDict, IterableDatasetDict)):
-        if "evaluation" in ds:
-            ds = ds["evaluation"]
-        elif "test" in ds:
-            ds = ds["test"]
-        else:
-            ds = ds["train"]
-
-    ds = ds.select(indices=random.sample(range(len(ds)), min(len(ds), num_samples)), keep_in_memory=True)
-    ds = ds.map(
-        make_data_block,
-        batched=True,
-        batch_size=len(ds),
-        num_proc=1,
-        remove_columns=ds.column_names,
-        keep_in_memory=True,
-        load_from_cache_file=False,
-        fn_kwargs={
-            "prompt_col_name": prompt_col_name,
-            "label_col_name": label_col_name,
-            "tokenizer": tokenizer,
-            "preprocess_fn": partial(preprocess_fn, **preprocess_fn_kwargs),
-            "sample_max_len": sample_max_len,
-            "block_max_len": block_max_len,
-            "add_eos_token": add_eos_token,
-            "truncate_prompt": truncate_prompt,
-            "merge_prompt_label": merge_prompt_label
-        }
-    )
-
-    # override some arguments' values in kwargs despite user specified
-    kwargs["batch_size"] = 1
-    kwargs["shuffle"] = False
-    kwargs["collate_fn"] = partial(collate_data, pad_token_id=tokenizer.pad_token_id)
-    dl = DataLoader(ds, **kwargs)
-
-    return dl
-
-
-__all__ = ["make_data_block", "collate_data", "get_dataloader"]
+import copy
+import random
+from functools import partial
+from typing import Callable, Dict, List, Optional
+
+import torch
+from datasets import load_dataset, DatasetDict, IterableDatasetDict
+from torch import LongTensor
+from torch.utils.data import DataLoader
+from transformers import PreTrainedTokenizer
+
+
+def make_data_block(
+    samples: Dict[str, List[str]],
+    prompt_col_name: str,
+    label_col_name: str,
+    tokenizer: PreTrainedTokenizer,
+    preprocess_fn: Optional[Callable] = None,
+    sample_max_len: int = 1024,
+    block_max_len: int = 2048,
+    add_eos_token: bool = False,
+    truncate_prompt: bool = True,
+    merge_prompt_label: bool = False
+) -> Dict[str, List[LongTensor]]:
+    """A simple implementation of text generation oriented smart batching to maximize VRAM usage when evaluation
+
+    :param samples: Dict[str, List[str]], samples that used to make data blocks
+    :param prompt_col_name: str, name of the key in samples whose value stores prompt
+    :param label_col_name: str, name of the key in samples whose value stores label
+    :param tokenizer: transformers.PretrainedTokenizer, tokenizer that used to tokenize samples
+    :param preprocess_fn: Optional[Callable], optional function that used to preprocess samples such as
+        refactor the data structure of samples, note the output of this function must be a dict whose keys
+        at least contains `prompt_col_name` and `label_col_name`
+    :param sample_max_len: int, defaults to 1024, max tokens number of each sample (before padding)
+    :param block_max_len: int, defaults to 2048, max tokens number of each data block (after padding)
+    :param add_eos_token: bool, defaults to False, whether add eos_token or not to the label
+    :param truncate_prompt: bool, defaults to True, whether to truncate prompt if the sample's total tokens
+        number exceeds `sample_max_len`, if not, will truncate label and drop this sample when all tokens
+        in label are truncated
+    :param merge_prompt_label: bool, defaults to False, will merge label into prompt if set to True, usually
+        this only required when doing language modeling task
+    :return: Dict[str, List[torch.LongTensor]], a dict whose keys are `input_ids`, `attention_mask` and
+        `label` and values are a list of torch.LongTensor
+    """
+    if preprocess_fn:
+        samples = preprocess_fn(samples)
+
+    prompts = samples[prompt_col_name]
+    labels = samples[label_col_name]
+
+    # tokenize samples
+    tokenized_prompts = tokenizer(prompts, truncation=False)["input_ids"]
+    tokenized_labels = tokenizer(labels, truncation=False)["input_ids"]
+
+    # filter tokenized samples by length
+    dropped_indices = []
+    for idx, (tokenized_prompt, tokenized_label) in enumerate(zip(tokenized_prompts, tokenized_labels)):
+        if add_eos_token:
+            tokenized_label += [tokenizer.eos_token_id]
+        len_prompt = len(tokenized_prompt)
+        len_label = len(tokenized_label)
+        exceed_len = len_prompt + len_label - sample_max_len
+        if exceed_len > 0:
+            if truncate_prompt:
+                tokenized_prompt = tokenized_prompt[exceed_len:]
+            else:
+                tokenized_label = tokenized_label[: -exceed_len]
+        tokenized_prompts[idx] = tokenized_prompt
+        tokenized_labels[idx] = tokenized_label
+        if not tokenized_label:
+            dropped_indices.append(idx)
+
+    # make data blocks of samples
+    tokenized_samples = sorted(
+        [
+            (p, l) for idx, (p, l) in enumerate(zip(tokenized_prompts, tokenized_labels))
+            if idx not in dropped_indices
+        ],
+        key=lambda x: (len(x[0]) + len(x[1])) if merge_prompt_label else len(x[0])
+    )
+    sample_blocks = []
+    sample_block = []
+    blk_max_len = 0
+    blk_total_len = 0
+    for tokenized_sample in tokenized_samples:
+        prompt_ids, label_ids = tokenized_sample
+        ori_sample_len = len(prompt_ids)
+        if merge_prompt_label:
+            ori_sample_len += len(label_ids)
+        if ori_sample_len <= blk_max_len:
+            additional_len = blk_max_len
+            sample_len = blk_max_len
+        else:
+            additional_len = len(sample_block) * (ori_sample_len - blk_max_len) + ori_sample_len
+            sample_len = ori_sample_len
+
+        if blk_total_len + additional_len > block_max_len:
+            sample_blocks.append((copy.copy(sample_block), blk_max_len))
+            sample_block = []
+            blk_max_len = 0
+            blk_total_len = 0
+            sample_len = ori_sample_len
+            additional_len = ori_sample_len
+
+        sample_block.append(tokenized_sample)
+        blk_max_len = max(blk_max_len, sample_len)
+        blk_total_len += additional_len
+
+    if sample_block:
+        sample_blocks.append((copy.copy(sample_block), blk_max_len))
+    del sample_block
+    del blk_max_len
+    del blk_total_len
+
+    new_samples = {
+        "input_ids": [],
+        "attention_mask": [],
+        "labels": []
+    }
+    # padding each data block internally
+    for block, blk_max_len in sample_blocks:
+        input_ids = []
+        attention_mask = []
+        label_ids = []
+        label_max_len = max([len(sample[1]) for sample in block])
+
+        for sample in block:
+            tokenized_prompt, tokenized_label = sample
+            sample_len = len(tokenized_prompt)
+            if merge_prompt_label:
+                sample_len += len(tokenized_label)
+            pad_num = blk_max_len - sample_len
+            if merge_prompt_label:
+                input_ids.append([tokenizer.pad_token_id] * pad_num + tokenized_prompt + tokenized_label)
+                label_ids.append([-100] * (pad_num + len(tokenized_prompt)) + tokenized_label)
+            else:
+                input_ids.append([tokenizer.pad_token_id] * pad_num + tokenized_prompt)
+                label_ids.append([-100] * (label_max_len - len(tokenized_label)) + tokenized_label)
+            attention_mask.append([0] * pad_num + [1] * sample_len)
+
+        new_samples["input_ids"].append(input_ids)
+        new_samples["attention_mask"].append(attention_mask)
+        new_samples["labels"].append(label_ids)
+
+    return new_samples
+
+
+def collate_data(blocks: List[Dict[str, List[List[int]]]], pad_token_id: int) -> Dict[str, LongTensor]:
+    def pad_block(block, pads):
+        return torch.cat((pads.to(block.device), block), dim=-1)
+
+    input_ids_blocks = [LongTensor(block["input_ids"]) for block in blocks]
+    attention_mask_blocks = [LongTensor(block["attention_mask"]) for block in blocks]
+    label_blocks = [LongTensor(block["labels"]) for block in blocks]
+
+    bsz = len(blocks)
+    inp_max_len = max([block.size(-1) for block in input_ids_blocks])
+    label_max_len = max([block.size(-1) for block in label_blocks])
+
+    for i in range(bsz):
+        block_bsz, block_inp_len = input_ids_blocks[i].shape
+        block_label_len = label_blocks[i].shape[-1]
+        pad_num = inp_max_len - block_inp_len
+        if pad_num > 0:
+            input_ids_blocks[i] = pad_block(input_ids_blocks[i], torch.ones((block_bsz, pad_num)) * pad_token_id)
+            attention_mask_blocks[i] = pad_block(attention_mask_blocks[i], torch.zeros((block_bsz, pad_num)))
+        label_pad_num = label_max_len - block_label_len
+        if label_pad_num > 0:
+            label_blocks[i] = pad_block(label_blocks[i], torch.ones((block_bsz, label_pad_num)) * -100)
+
+    return {
+        "input_ids": torch.cat(input_ids_blocks, dim=0).long(),
+        "attention_mask": torch.cat(attention_mask_blocks, dim=0).long(),
+        "labels": torch.cat(label_blocks, dim=0).long()
+    }
+
+
+def get_dataloader(
+    data_path_or_name: str,
+    prompt_col_name: str,
+    label_col_name: str,
+    tokenizer: PreTrainedTokenizer,
+    load_fn: Optional[Callable] = None,
+    preprocess_fn: Optional[Callable] = None,
+    num_samples: int = 128,
+    sample_max_len: int = 1024,
+    block_max_len: int = 2048,
+    add_eos_token: bool = False,
+    truncate_prompt: bool = True,
+    merge_prompt_label: bool = False,
+    load_fn_kwargs: Optional[dict] = None,
+    preprocess_fn_kwargs: Optional[dict] = None,
+    **kwargs
+) -> DataLoader:
+    """load dataset and build dataloader
+
+    :param data_path_or_name: str, dataset name in hf-hub or local file path
+    :param prompt_col_name: str, see `make_data_block`
+    :param label_col_name: str, see `make_data_block`
+    :param tokenizer: str, see `make_data_block`
+    :param load_fn: Optional[Callable], defaults to None, function used to load dataset, if not specified,
+        use `datasets.load_dataset`
+    :param preprocess_fn: Optional[Callable], see `make_data_block`
+    :param num_samples: int, defaults to 128, total samples used to evaluation
+    :param sample_max_len: int, see `make_data_block`
+    :param block_max_len: int, see `make_data_block`
+    :param add_eos_token: bool, see `make_data_block`
+    :param truncate_prompt: bool, see `make_data_block`
+    :param merge_prompt_label: bool, see `make_data_block`
+    :param load_fn_kwargs: Optional[dict], defaults to None, keyword arguments used
+        for `load_fn` or `datasets.load_dataset`
+    :param preprocess_fn_kwargs: Optional[dict], defaults to None, keyword arguments used
+        for `preprocess_fn`
+    :param kwargs: additional keyword arguments will be passed to torch's `DataLoader` initialization,
+        note values of `batch_size`, `shuffle` and `collate_fn` will always be overridden to fixed value
+    :return: torch.utils.data.DataLoader
+    """
+
+    if not load_fn_kwargs:
+        load_fn_kwargs = dict()
+    if not preprocess_fn_kwargs:
+        preprocess_fn_kwargs = dict()
+
+    if load_fn:
+        ds = load_fn(data_path_or_name, **load_fn_kwargs)
+    else:
+        ds = load_dataset(data_path_or_name, **load_fn_kwargs)
+    if isinstance(ds, (DatasetDict, IterableDatasetDict)):
+        if "evaluation" in ds:
+            ds = ds["evaluation"]
+        elif "test" in ds:
+            ds = ds["test"]
+        else:
+            ds = ds["train"]
+
+    ds = ds.select(indices=random.sample(range(len(ds)), min(len(ds), num_samples)), keep_in_memory=True)
+    ds = ds.map(
+        make_data_block,
+        batched=True,
+        batch_size=len(ds),
+        num_proc=1,
+        remove_columns=ds.column_names,
+        keep_in_memory=True,
+        load_from_cache_file=False,
+        fn_kwargs={
+            "prompt_col_name": prompt_col_name,
+            "label_col_name": label_col_name,
+            "tokenizer": tokenizer,
+            "preprocess_fn": partial(preprocess_fn, **preprocess_fn_kwargs),
+            "sample_max_len": sample_max_len,
+            "block_max_len": block_max_len,
+            "add_eos_token": add_eos_token,
+            "truncate_prompt": truncate_prompt,
+            "merge_prompt_label": merge_prompt_label
+        }
+    )
+
+    # override some arguments' values in kwargs despite user specified
+    kwargs["batch_size"] = 1
+    kwargs["shuffle"] = False
+    kwargs["collate_fn"] = partial(collate_data, pad_token_id=tokenizer.pad_token_id)
+    dl = DataLoader(ds, **kwargs)
+
+    return dl
+
+
+__all__ = ["make_data_block", "collate_data", "get_dataloader"]
```

### Comparing `auto_gptq-0.0.5/auto_gptq/eval_tasks/_utils/generation_utils.py` & `auto_gptq-0.1.0/auto_gptq/eval_tasks/_utils/generation_utils.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from typing import List, Optional, Union
-
-from torch import LongTensor
-from transformers import PreTrainedTokenizer
-
-
-def postprocess_generation_ids(
-    input_ids: LongTensor,
-    output_ids: LongTensor,
-    num_return_sequences: int,
-    tokenizer: Optional[PreTrainedTokenizer] = None,
-    pad_token_ids: Optional[int] = None,
-) -> List[List[Union[str, List[int]]]]:
-    outputs = []
-    for idx, start in enumerate(range(0, len(output_ids), num_return_sequences)):
-        sub_output_ids = output_ids[start: start + num_return_sequences]
-        sub_generated_ids = sub_output_ids[..., input_ids[idx].size(0):]
-        if tokenizer:
-            outputs.append(
-                [
-                    generated_text for generated_text in tokenizer.batch_decode(
-                        sub_generated_ids,
-                        clean_up_tokenization_spaces=True
-                    )
-                ]
-            )
-        else:
-            sub_generated_ids = sub_output_ids.cpu().numpy().tolist()
-            for i, one_sub_generated_ids in enumerate(sub_generated_ids):
-                if pad_token_ids is not None and pad_token_ids in one_sub_generated_ids:
-                    one_sub_generated_ids = one_sub_generated_ids[: one_sub_generated_ids.index(pad_token_ids)]
-                sub_generated_ids[i] = one_sub_generated_ids
-            outputs.append(sub_generated_ids)
-
-    return outputs
-
-
-__all__ = ["postprocess_generation_ids"]
+from typing import List, Optional, Union
+
+from torch import LongTensor
+from transformers import PreTrainedTokenizer
+
+
+def postprocess_generation_ids(
+    input_ids: LongTensor,
+    output_ids: LongTensor,
+    num_return_sequences: int,
+    tokenizer: Optional[PreTrainedTokenizer] = None,
+    pad_token_ids: Optional[int] = None,
+) -> List[List[Union[str, List[int]]]]:
+    outputs = []
+    for idx, start in enumerate(range(0, len(output_ids), num_return_sequences)):
+        sub_output_ids = output_ids[start: start + num_return_sequences]
+        sub_generated_ids = sub_output_ids[..., input_ids[idx].size(0):]
+        if tokenizer:
+            outputs.append(
+                [
+                    generated_text for generated_text in tokenizer.batch_decode(
+                        sub_generated_ids,
+                        clean_up_tokenization_spaces=True
+                    )
+                ]
+            )
+        else:
+            sub_generated_ids = sub_output_ids.cpu().numpy().tolist()
+            for i, one_sub_generated_ids in enumerate(sub_generated_ids):
+                if pad_token_ids is not None and pad_token_ids in one_sub_generated_ids:
+                    one_sub_generated_ids = one_sub_generated_ids[: one_sub_generated_ids.index(pad_token_ids)]
+                sub_generated_ids[i] = one_sub_generated_ids
+            outputs.append(sub_generated_ids)
+
+    return outputs
+
+
+__all__ = ["postprocess_generation_ids"]
```

### Comparing `auto_gptq-0.0.5/auto_gptq/eval_tasks/language_modeling_task.py` & `auto_gptq-0.1.0/auto_gptq/eval_tasks/language_modeling_task.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-import math
-from typing import Any, Dict, List, Optional
-
-from torch import LongTensor
-
-from ._base import BaseTask
-
-
-class LanguageModelingTask(BaseTask):
-    def __init__(
-        self,
-        model,
-        tokenizer,
-        data_name_or_path: str,
-        prompt_col_name: str,
-        label_col_name: str,
-        device: Optional[str] = None,
-        **kwargs
-    ):
-        kwargs["merge_prompt_label"] = True
-        super().__init__(
-            model=model,
-            tokenizer=tokenizer,
-            data_name_or_path=data_name_or_path,
-            prompt_col_name=prompt_col_name,
-            label_col_name=label_col_name,
-            device=device,
-            **kwargs
-        )
-
-    def _predict(self, batch_data: Dict[str, Any], *args, **kwargs) -> List[float]:
-        outputs = self.model(**batch_data)
-        loss = outputs.loss.cpu().item()
-
-        return [loss]
-
-    def _parse_labels(self, label_ids: LongTensor) -> List[Any]:
-        return []
-
-    def _metric(self, pred: List[Any], label: List[Any]) -> Dict[str, float]:
-        return {"ppl": math.exp(sum(pred) / len(pred))}
-
-    def run(self) -> Dict[str, float]:
-        return super().run()
-
-
-__all__ = ["LanguageModelingTask"]
+import math
+from typing import Any, Dict, List, Optional
+
+from torch import LongTensor
+
+from ._base import BaseTask
+
+
+class LanguageModelingTask(BaseTask):
+    def __init__(
+        self,
+        model,
+        tokenizer,
+        data_name_or_path: str,
+        prompt_col_name: str,
+        label_col_name: str,
+        device: Optional[str] = None,
+        **kwargs
+    ):
+        kwargs["merge_prompt_label"] = True
+        super().__init__(
+            model=model,
+            tokenizer=tokenizer,
+            data_name_or_path=data_name_or_path,
+            prompt_col_name=prompt_col_name,
+            label_col_name=label_col_name,
+            device=device,
+            **kwargs
+        )
+
+    def _predict(self, batch_data: Dict[str, Any], *args, **kwargs) -> List[float]:
+        outputs = self.model(**batch_data)
+        loss = outputs.loss.cpu().item()
+
+        return [loss]
+
+    def _parse_labels(self, label_ids: LongTensor) -> List[Any]:
+        return []
+
+    def _metric(self, pred: List[Any], label: List[Any]) -> Dict[str, float]:
+        return {"ppl": math.exp(sum(pred) / len(pred))}
+
+    def run(self) -> Dict[str, float]:
+        return super().run()
+
+
+__all__ = ["LanguageModelingTask"]
```

### Comparing `auto_gptq-0.0.5/auto_gptq/modeling/auto.py` & `auto_gptq-0.1.0/auto_gptq/modeling/auto.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,62 +1,76 @@
-from ._base import BaseQuantizeConfig, BaseGPTQForCausalLM
-from ._utils import check_and_get_model_type
-from .bloom import BloomGPTQForCausalLM
-from .gpt_neox import GPTNeoXGPTQForCausalLM
-from .gptj import GPTJGPTQForCausalLM
-from .llama import LlamaGPTQForCausalLM
-from .moss import MOSSGPTQForCausalLM
-from .opt import OPTGPTQForCausalLM
-
-
-GPTQ_CAUSAL_LM_MODEL_MAP = {
-    "bloom": BloomGPTQForCausalLM,
-    "gpt_neox": GPTNeoXGPTQForCausalLM,
-    "gptj": GPTJGPTQForCausalLM,
-    "llama": LlamaGPTQForCausalLM,
-    "opt": OPTGPTQForCausalLM,
-    "moss": MOSSGPTQForCausalLM
-}
-
-
-class AutoGPTQForCausalLM:
-    def __init__(self):
-        raise EnvironmentError(
-            "AutoGPTQModelForCausalLM is designed to be instantiated\n"
-            "using `AutoGPTQModelForCausalLM.from_pretrained` if want to quantize a pretrained model.\n"
-            "using `AutoGPTQModelForCausalLM.from_quantized` if want to inference with quantized model."
-        )
-
-    @classmethod
-    def from_pretrained(
-        cls,
-        pretrained_model_name_or_path: str,
-        quantize_config: BaseQuantizeConfig,
-        bf16: bool = False,
-        **model_init_kwargs
-    ) -> BaseGPTQForCausalLM:
-        model_type = check_and_get_model_type(pretrained_model_name_or_path)
-        return GPTQ_CAUSAL_LM_MODEL_MAP[model_type].from_pretrained(
-            pretrained_model_name_or_path=pretrained_model_name_or_path,
-            quantize_config=quantize_config,
-            bf16=bf16,
-            **model_init_kwargs
-        )
-
-    @classmethod
-    def from_quantized(
-        cls,
-        save_dir: str,
-        device: str = "cpu",
-        use_safetensors: bool = False,
-        use_triton: bool = False
-    ) -> BaseGPTQForCausalLM:
-        model_type = check_and_get_model_type(save_dir)
-        return GPTQ_CAUSAL_LM_MODEL_MAP[model_type].from_quantized(
-            save_dir=save_dir,
-            device=device,
-            use_safetensors=use_safetensors,
-            use_triton=use_triton
-        )
-
-
-__all__ = ["AutoGPTQForCausalLM"]
+from typing import Optional
+
+from ._base import BaseQuantizeConfig, BaseGPTQForCausalLM
+from ._utils import check_and_get_model_type
+from .bloom import BloomGPTQForCausalLM
+from .gpt_neox import GPTNeoXGPTQForCausalLM
+from .gptj import GPTJGPTQForCausalLM
+from .gpt2 import GPT2GPTQForCausalLM
+from .llama import LlamaGPTQForCausalLM
+from .moss import MOSSGPTQForCausalLM
+from .opt import OPTGPTQForCausalLM
+
+
+GPTQ_CAUSAL_LM_MODEL_MAP = {
+    "bloom": BloomGPTQForCausalLM,
+    "gpt_neox": GPTNeoXGPTQForCausalLM,
+    "gptj": GPTJGPTQForCausalLM,
+    "gpt2": GPT2GPTQForCausalLM,
+    "llama": LlamaGPTQForCausalLM,
+    "opt": OPTGPTQForCausalLM,
+    "moss": MOSSGPTQForCausalLM
+}
+
+
+class AutoGPTQForCausalLM:
+    def __init__(self):
+        raise EnvironmentError(
+            "AutoGPTQModelForCausalLM is designed to be instantiated\n"
+            "using `AutoGPTQModelForCausalLM.from_pretrained` if want to quantize a pretrained model.\n"
+            "using `AutoGPTQModelForCausalLM.from_quantized` if want to inference with quantized model."
+        )
+
+    @classmethod
+    def from_pretrained(
+        cls,
+        pretrained_model_name_or_path: str,
+        quantize_config: BaseQuantizeConfig,
+        max_memory: Optional[dict] = None,
+        **model_init_kwargs
+    ) -> BaseGPTQForCausalLM:
+        model_type = check_and_get_model_type(pretrained_model_name_or_path)
+        return GPTQ_CAUSAL_LM_MODEL_MAP[model_type].from_pretrained(
+            pretrained_model_name_or_path=pretrained_model_name_or_path,
+            quantize_config=quantize_config,
+            max_memory=max_memory,
+            **model_init_kwargs
+        )
+
+    @classmethod
+    def from_quantized(
+        cls,
+        save_dir: str,
+        device: str = "cpu",
+        use_safetensors: bool = False,
+        use_triton: bool = False,
+        max_memory: Optional[dict] = None,
+        device_map: Optional[str] = None,
+        quantize_config: Optional[BaseQuantizeConfig] = None,
+        model_basename: Optional[str] = None,
+        trust_remote_code: bool = False
+    ) -> BaseGPTQForCausalLM:
+        model_type = check_and_get_model_type(save_dir)
+        return GPTQ_CAUSAL_LM_MODEL_MAP[model_type].from_quantized(
+            save_dir=save_dir,
+            device=device,
+            use_safetensors=use_safetensors,
+            use_triton=use_triton,
+            max_memory=max_memory,
+            device_map=device_map,
+            quantize_config=quantize_config,
+            model_basename=model_basename,
+            trust_remote_code=trust_remote_code
+        )
+
+
+__all__ = ["AutoGPTQForCausalLM"]
```

### Comparing `auto_gptq-0.0.5/auto_gptq/nn_modules/qlinear.py` & `auto_gptq-0.1.0/auto_gptq/nn_modules/qlinear_old.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,244 +1,277 @@
-import math
-from logging import getLogger
-
-import numpy as np
-import torch
-import torch.nn as nn
-
-logger = getLogger(__name__)
-
-try:
-    import quant_cuda
-
-    _quant_cuda_available = True
-except ImportError:
-    logger.warning('CUDA extension not installed.')
-    _quant_cuda_available = False
-
-
-class QuantLinear(nn.Module):
-    def __init__(
-        self,
-        bits,
-        groupsize,
-        infeatures,
-        outfeatures,
-        bias,
-        kernel_switch_threshold=128,
-    ):
-        super().__init__()
-        if bits not in [2, 3, 4, 8]:
-            raise NotImplementedError("Only 2,3,4,8 bits are supported.")
-
-        self.infeatures = infeatures
-        self.outfeatures = outfeatures
-        self.bits = bits
-        self.groupsize = groupsize if groupsize != -1 else infeatures
-        self.maxq = 2 ** self.bits - 1
-
-        self.register_buffer(
-            'qweight',
-            torch.zeros((infeatures // 32 * self.bits, outfeatures), dtype=torch.int32)
-        )
-        self.register_buffer(
-            'qzeros',
-            torch.zeros((math.ceil(infeatures / self.groupsize), outfeatures // 32 * self.bits), dtype=torch.int32)
-        )
-        self.register_buffer(
-            'scales',
-            torch.zeros((math.ceil(infeatures / self.groupsize), outfeatures), dtype=torch.float16)
-        )
-        self.register_buffer(
-            'g_idx',
-            torch.tensor([i // self.groupsize for i in range(infeatures)], dtype=torch.int32)
-        )
-        if bias:
-            self.register_buffer('bias', torch.zeros((outfeatures), dtype=torch.float16))
-        else:
-            self.bias = None
-
-        # is performed by unpacking the weights and using torch.matmul
-        if self.bits in [2, 4, 8]:
-            self.register_buffer(
-                'wf',
-                torch.tensor(list(range(0, 32, self.bits)), dtype=torch.int32).unsqueeze(0),
-                persistent=False
-            )
-        elif self.bits == 3:
-            self.register_buffer(
-                'wf',
-                torch.tensor(
-                    [
-                        [0, 3, 6, 9, 12, 15, 18, 21, 24, 27, 30, 0],
-                        [0, 1, 4, 7, 10, 13, 16, 19, 22, 25, 28, 31],
-                        [0, 2, 5, 8, 11, 14, 17, 20, 23, 26, 29, 0],
-                    ],
-                    dtype=torch.int32).reshape(1, 3, 12),
-                persistent=False
-            )
-
-        self.kernel_switch_threshold = kernel_switch_threshold
-        self.quant_cuda_available = _quant_cuda_available
-
-    def pack(self, linear, scales, zeros, g_idx=None):
-        self.g_idx = g_idx.clone() if g_idx is not None else self.g_idx
-
-        scales = scales.t().contiguous()
-        zeros = zeros.t().contiguous()
-        scale_zeros = zeros * scales
-        self.scales = scales.clone().half()
-        if linear.bias is not None:
-            self.bias = linear.bias.clone().half()
-
-        intweight = []
-        for idx in range(self.infeatures):
-            intweight.append(
-                torch.round(
-                    (
-                        linear.weight.data[:, idx] + scale_zeros[self.g_idx[idx]]) / self.scales[self.g_idx[idx]]
-                ).to(torch.int)[:, None]
-            )
-        intweight = torch.cat(intweight, dim=1)
-        intweight = intweight.t().contiguous()
-        intweight = intweight.numpy().astype(np.uint32)
-
-        i = 0
-        row = 0
-        qweight = np.zeros(
-            (intweight.shape[0] // 32 * self.bits, intweight.shape[1]), dtype=np.uint32
-        )
-        while row < qweight.shape[0]:
-            if self.bits in [2, 4, 8]:
-                for j in range(i, i + (32 // self.bits)):
-                    qweight[row] |= intweight[j] << (self.bits * (j - i))
-                i += 32 // self.bits
-                row += 1
-            elif self.bits == 3:
-                for j in range(i, i + 10):
-                    qweight[row] |= intweight[j] << (3 * (j - i))
-                i += 10
-                qweight[row] |= intweight[i] << 30
-                row += 1
-                qweight[row] |= (intweight[i] >> 2) & 1
-                i += 1
-                for j in range(i, i + 10):
-                    qweight[row] |= intweight[j] << (3 * (j - i) + 1)
-                i += 10
-                qweight[row] |= intweight[i] << 31
-                row += 1
-                qweight[row] |= (intweight[i] >> 1) & 0x3
-                i += 1
-                for j in range(i, i + 10):
-                    qweight[row] |= intweight[j] << (3 * (j - i) + 2)
-                i += 10
-                row += 1
-            else:
-                raise NotImplementedError("Only 2,3,4,8 bits are supported.")
-
-        qweight = qweight.astype(np.int32)
-        self.qweight = torch.from_numpy(qweight)
-
-        zeros -= 1
-        zeros = zeros.numpy().astype(np.uint32)
-        qzeros = np.zeros((zeros.shape[0], zeros.shape[1] // 32 * self.bits), dtype=np.uint32)
-        i = 0
-        col = 0
-        while col < qzeros.shape[1]:
-            if self.bits in [2, 4, 8]:
-                for j in range(i, i + (32 // self.bits)):
-                    qzeros[:, col] |= zeros[:, j] << (self.bits * (j - i))
-                i += 32 // self.bits
-                col += 1
-            elif self.bits == 3:
-                for j in range(i, i + 10):
-                    qzeros[:, col] |= zeros[:, j] << (3 * (j - i))
-                i += 10
-                qzeros[:, col] |= zeros[:, i] << 30
-                col += 1
-                qzeros[:, col] |= (zeros[:, i] >> 2) & 1
-                i += 1
-                for j in range(i, i + 10):
-                    qzeros[:, col] |= zeros[:, j] << (3 * (j - i) + 1)
-                i += 10
-                qzeros[:, col] |= zeros[:, i] << 31
-                col += 1
-                qzeros[:, col] |= (zeros[:, i] >> 1) & 0x3
-                i += 1
-                for j in range(i, i + 10):
-                    qzeros[:, col] |= zeros[:, j] << (3 * (j - i) + 2)
-                i += 10
-                col += 1
-            else:
-                raise NotImplementedError("Only 2,3,4,8 bits are supported.")
-
-        qzeros = qzeros.astype(np.int32)
-        self.qzeros = torch.from_numpy(qzeros)
-
-    def forward(self, x: torch.Tensor):
-        out_shape = x.shape[:-1] + (self.outfeatures,)
-        x = x.reshape(-1, x.shape[-1])
-        if self.quant_cuda_available and (
-            self.kernel_switch_threshold == 0 or x.shape[0] < self.kernel_switch_threshold
-        ):
-            out = torch.zeros((x.shape[0], self.outfeatures), device='cuda', dtype=torch.float32)
-            if self.bits == 2:
-                quant_cuda.vecquant2matmul(x.float(), self.qweight, out, self.scales.float(), self.qzeros, self.g_idx)
-            elif self.bits == 3:
-                quant_cuda.vecquant3matmul(x.float(), self.qweight, out, self.scales.float(), self.qzeros, self.g_idx)
-            elif self.bits == 4:
-                quant_cuda.vecquant4matmul(x.float(), self.qweight, out, self.scales.float(), self.qzeros, self.g_idx)
-            elif self.bits == 8:
-                quant_cuda.vecquant8matmul(x.float(), self.qweight, out, self.scales.float(), self.qzeros, self.g_idx)
-            else:
-                raise NotImplementedError("Only 2,3,4,8 bits are supported.")
-            out = out.half()
-        else:
-            if self.bits in [2, 4, 8]:
-                zeros = torch.bitwise_right_shift(
-                    torch.unsqueeze(self.qzeros, 2).expand(-1, -1, 32 // self.bits),
-                    self.wf.unsqueeze(0)
-                ).to(torch.int16 if self.bits == 8 else torch.int8)
-                torch.bitwise_and(zeros, (2 ** self.bits) - 1, out=zeros)
-
-                zeros = zeros + 1
-                zeros = zeros.reshape(self.scales.shape)
-
-                weight = torch.bitwise_right_shift(
-                    torch.unsqueeze(self.qweight, 1).expand(-1, 32 // self.bits, -1),
-                    self.wf.unsqueeze(-1)
-                ).to(torch.int16 if self.bits == 8 else torch.int8)
-                torch.bitwise_and(weight, (2 ** self.bits) - 1, out=weight)
-            elif self.bits == 3:
-                zeros = self.qzeros.reshape(
-                    self.qzeros.shape[0], self.qzeros.shape[1] // 3, 3, 1
-                ).expand(-1, -1, -1, 12)
-                zeros = (zeros >> self.wf.unsqueeze(0))
-                zeros[:, :, 0, 10] = (zeros[:, :, 0, 10] & 0x3) | ((zeros[:, :, 1, 0] << 2) & 0x4)
-                zeros[:, :, 1, 11] = (zeros[:, :, 1, 11] & 0x1) | ((zeros[:, :, 2, 0] << 1) & 0x6)
-                zeros = zeros & 0x7
-                zeros = torch.cat([zeros[:, :, 0, :11], zeros[:, :, 1, 1:12], zeros[:, :, 2, 1:11]], dim=2)
-
-                zeros = zeros + 1
-                zeros = zeros.reshape(self.scales.shape)
-
-                weight = self.qweight.reshape(
-                    self.qweight.shape[0] // 3, 3, 1, self.qweight.shape[1]
-                ).expand(-1, -1, 12, -1)
-                weight = (weight >> self.wf.unsqueeze(-1)) & 0x7
-                weight[:, 0, 10] = (weight[:, 0, 10] & 0x3) | ((weight[:, 1, 0] << 2) & 0x4)
-                weight[:, 1, 11] = (weight[:, 1, 11] & 0x1) | ((weight[:, 2, 0] << 1) & 0x6)
-                weight = weight & 0x7
-                weight = torch.cat([weight[:, 0, :11], weight[:, 1, 1:12], weight[:, 2, 1:11]], dim=1)
-            else:
-                raise NotImplementedError("Only 2,3,4,8 bits are supported.")
-
-            weight = weight.reshape(weight.shape[0] * weight.shape[1], weight.shape[2])
-
-            weights = (self.scales[self.g_idx.long()] * (weight - zeros[self.g_idx.long()]))
-            out = torch.matmul(x.half(), weights)
-        out = out.reshape(out_shape)
-        out = out + self.bias if self.bias is not None else out
-        return out
-
-
-__all__ = ["QuantLinear"]
+import math
+from logging import getLogger
+
+import numpy as np
+import torch
+import torch.nn as nn
+import transformers
+
+logger = getLogger(__name__)
+
+try:
+    import quant_cuda
+
+    _quant_cuda_available = True
+except ImportError:
+    logger.warning('CUDA extension not installed.')
+    _quant_cuda_available = False
+
+
+class QuantLinear(nn.Module):
+    def __init__(
+        self,
+        bits,
+        groupsize,
+        infeatures,
+        outfeatures,
+        bias,
+        faster=True,
+        kernel_switch_threshold=128
+    ):
+        super().__init__()
+        if bits not in [2, 3, 4, 8]:
+            raise NotImplementedError("Only 2,3,4,8 bits are supported.")
+        self.infeatures = infeatures
+        self.outfeatures = outfeatures
+        self.bits = bits
+        self.groupsize = groupsize if groupsize != -1 else infeatures
+        self.maxq = 2 ** self.bits - 1
+
+        self.register_buffer(
+            'qweight',
+            torch.zeros((infeatures // 32 * self.bits, outfeatures), dtype=torch.int32)
+        )
+        self.register_buffer(
+            'qzeros',
+            torch.zeros((math.ceil(infeatures / self.groupsize), outfeatures // 32 * self.bits), dtype=torch.int32)
+        )
+        self.register_buffer(
+            'scales',
+            torch.zeros((math.ceil(infeatures / self.groupsize), outfeatures), dtype=torch.float16)
+        )
+        self.register_buffer(
+            'g_idx',
+            torch.tensor([i // self.groupsize for i in range(infeatures)], dtype=torch.int32)
+        )
+        if bias:
+            self.register_buffer('bias', torch.zeros((outfeatures), dtype=torch.float16))
+        else:
+            self.bias = None
+        self.half_indim = self.infeatures // 2
+        self.faster = faster if bits != 8 else False
+
+        # is performed by unpacking the weights and using torch.matmul
+        if self.bits in [2, 4, 8]:
+            self.wf = torch.tensor(list(range(0, 32, self.bits)), dtype=torch.int32).unsqueeze(0)
+        elif self.bits == 3:
+            self.wf = torch.tensor(
+                [
+                    [0, 3, 6, 9, 12, 15, 18, 21, 24, 27, 30, 0],
+                    [0, 1, 4, 7, 10, 13, 16, 19, 22, 25, 28, 31],
+                    [0, 2, 5, 8, 11, 14, 17, 20, 23, 26, 29, 0],
+                ],
+                dtype=torch.int32
+            ).reshape(1, 3, 12)
+
+        self.kernel_switch_threshold = kernel_switch_threshold
+        self.quant_cuda_available = _quant_cuda_available
+        if infeatures % 256 != 0 or outfeatures % 256 != 0:
+            self.quant_cuda_available = False
+
+    def pack(self, linear, scales, zeros, g_idx):
+        scales = scales.t().contiguous()
+        zeros = zeros.t().contiguous()
+        scale_zeros = zeros * scales
+        self.scales = scales.clone().half()
+        if linear.bias is not None:
+            self.bias = linear.bias.clone().half()
+
+        intweight = []
+        for idx in range(self.infeatures):
+            g_idx = idx // self.groupsize
+            intweight.append(
+                torch.round(
+                    (linear.weight.data[:, idx] + scale_zeros[g_idx]) / self.scales[g_idx]
+                ).to(torch.int)[:, None]
+            )
+        intweight = torch.cat(intweight, dim=1)
+        intweight = intweight.t().contiguous()
+        intweight = intweight.numpy().astype(np.uint32)
+
+        i = 0
+        row = 0
+        qweight = np.zeros(
+            (intweight.shape[0] // 32 * self.bits, intweight.shape[1]), dtype=np.uint32
+        )
+        while row < qweight.shape[0]:
+            if self.bits in [2, 4, 8]:
+                for j in range(i, i + (32 // self.bits)):
+                    qweight[row] |= intweight[j] << (self.bits * (j - i))
+                i += 32 // self.bits
+                row += 1
+            elif self.bits == 3:
+                for j in range(i, i + 10):
+                    qweight[row] |= intweight[j] << (3 * (j - i))
+                i += 10
+                qweight[row] |= intweight[i] << 30
+                row += 1
+                qweight[row] |= (intweight[i] >> 2) & 1
+                i += 1
+                for j in range(i, i + 10):
+                    qweight[row] |= intweight[j] << (3 * (j - i) + 1)
+                i += 10
+                qweight[row] |= intweight[i] << 31
+                row += 1
+                qweight[row] |= (intweight[i] >> 1) & 0x3
+                i += 1
+                for j in range(i, i + 10):
+                    qweight[row] |= intweight[j] << (3 * (j - i) + 2)
+                i += 10
+                row += 1
+            else:
+                raise NotImplementedError("Only 2,3,4,8 bits are supported.")
+
+        qweight = qweight.astype(np.int32)
+        self.qweight = torch.from_numpy(qweight)
+
+        zeros -= 1
+        zeros = zeros.numpy().astype(np.uint32)
+        qzeros = np.zeros((zeros.shape[0], zeros.shape[1] // 32 * self.bits), dtype=np.uint32)
+        i = 0
+        col = 0
+        while col < qzeros.shape[1]:
+            if self.bits in [2, 4, 8]:
+                for j in range(i, i + (32 // self.bits)):
+                    qzeros[:, col] |= zeros[:, j] << (self.bits * (j - i))
+                i += 32 // self.bits
+                col += 1
+            elif self.bits == 3:
+                for j in range(i, i + 10):
+                    qzeros[:, col] |= zeros[:, j] << (3 * (j - i))
+                i += 10
+                qzeros[:, col] |= zeros[:, i] << 30
+                col += 1
+                qzeros[:, col] |= (zeros[:, i] >> 2) & 1
+                i += 1
+                for j in range(i, i + 10):
+                    qzeros[:, col] |= zeros[:, j] << (3 * (j - i) + 1)
+                i += 10
+                qzeros[:, col] |= zeros[:, i] << 31
+                col += 1
+                qzeros[:, col] |= (zeros[:, i] >> 1) & 0x3
+                i += 1
+                for j in range(i, i + 10):
+                    qzeros[:, col] |= zeros[:, j] << (3 * (j - i) + 2)
+                i += 10
+                col += 1
+            else:
+                raise NotImplementedError("Only 2,3,4,8 bits are supported.")
+
+        qzeros = qzeros.astype(np.int32)
+        self.qzeros = torch.from_numpy(qzeros)
+
+    def forward(self, x):
+        out_shape = x.shape[:-1] + (self.outfeatures,)
+        x = x.reshape(-1, x.shape[-1])
+        if self.quant_cuda_available is True and (
+            self.kernel_switch_threshold is False or x.shape[0] < self.kernel_switch_threshold
+        ):
+            out = torch.zeros(x.shape[0], out_shape[-1], dtype=torch.float, device=x.device)
+
+            if self.faster:
+                x = x.half()
+                if self.bits == 2:
+                    quant_cuda.vecquant2matmul_faster_old(
+                        x, self.qweight, out, self.scales.float(), self.qzeros, self.groupsize, self.half_indim
+                    )
+                elif self.bits == 3:
+                    quant_cuda.vecquant3matmul_faster_old(
+                        x, self.qweight, out, self.scales.float(), self.qzeros, self.groupsize, self.half_indim
+                    )
+                elif self.bits == 4:
+                    quant_cuda.vecquant4matmul_faster_old(
+                        x, self.qweight, out, self.scales.float(), self.qzeros, self.groupsize, self.half_indim
+                    )
+                else:
+                    raise NotImplementedError("Only 2,3,4 bits are supported.")
+            else:
+                x = x.float()
+                if self.bits == 2:
+                    quant_cuda.vecquant2matmul_old(
+                        x, self.qweight, out, self.scales.float(), self.qzeros, self.groupsize
+                    )
+                elif self.bits == 3:
+                    quant_cuda.vecquant3matmul_old(
+                        x, self.qweight, out, self.scales.float(), self.qzeros, self.groupsize
+                    )
+                elif self.bits == 4:
+                    quant_cuda.vecquant4matmul_old(
+                        x, self.qweight, out, self.scales.float(), self.qzeros, self.groupsize
+                    )
+                elif self.bits == 8:
+                    quant_cuda.vecquant8matmul_old(
+                        x, self.qweight, out, self.scales.float(), self.qzeros, self.groupsize
+                    )
+                else:
+                    raise NotImplementedError("Only 2,3,4,8 bits are supported.")
+        else:
+            if self.wf.device != self.qzeros.device:
+                self.wf = self.wf.to(self.qzeros.device)
+
+            if self.bits in [2, 4, 8]:
+                zeros = torch.bitwise_right_shift(
+                    torch.unsqueeze(self.qzeros, 2).expand(-1, -1, 32 // self.bits),
+                    self.wf.unsqueeze(0)
+                ).to(torch.int16 if self.bits == 8 else torch.int8)
+                torch.bitwise_and(zeros, (2 ** self.bits) - 1, out=zeros)
+
+                zeros = zeros + 1
+                zeros = zeros.reshape(-1, 1, zeros.shape[1] * zeros.shape[2])
+
+                scales = self.scales
+                scales = scales.reshape(-1, 1, scales.shape[-1])
+
+                weight = torch.bitwise_right_shift(
+                    torch.unsqueeze(self.qweight, 1).expand(-1, 32 // self.bits, -1),
+                    self.wf.unsqueeze(-1)
+                ).to(torch.int16 if self.bits == 8 else torch.int8)
+                torch.bitwise_and(weight, (2 ** self.bits) - 1, out=weight)
+                weight = weight.reshape(-1, self.groupsize, weight.shape[2])
+            elif self.bits == 3:
+                zeros = self.qzeros.reshape(
+                    self.qzeros.shape[0], self.qzeros.shape[1] // 3, 3, 1
+                ).expand(-1, -1, -1, 12)
+                zeros = (zeros >> self.wf.unsqueeze(0))
+                zeros[:, :, 0, 10] = (zeros[:, :, 0, 10] & 0x3) | ((zeros[:, :, 1, 0] << 2) & 0x4)
+                zeros[:, :, 1, 11] = (zeros[:, :, 1, 11] & 0x1) | ((zeros[:, :, 2, 0] << 1) & 0x6)
+                zeros = zeros & 0x7
+                zeros = torch.cat([zeros[:, :, 0, :11], zeros[:, :, 1, 1:12], zeros[:, :, 2, 1:11]], dim=2)
+
+                zeros = zeros + 1
+                zeros = zeros.reshape(-1, 1, zeros.shape[1] * zeros.shape[2])
+
+                scales = self.scales
+                scales = scales.reshape(-1, 1, scales.shape[-1])
+
+                weight = self.qweight.reshape(
+                    self.qweight.shape[0] // 3, 3, 1, self.qweight.shape[1]
+                ).expand(-1, -1, 12, -1)
+                weight = (weight >> self.wf.unsqueeze(-1)) & 0x7
+                weight[:, 0, 10] = (weight[:, 0, 10] & 0x3) | ((weight[:, 1, 0] << 2) & 0x4)
+                weight[:, 1, 11] = (weight[:, 1, 11] & 0x1) | ((weight[:, 2, 0] << 1) & 0x6)
+                weight = weight & 0x7
+                weight = torch.cat([weight[:, 0, :11], weight[:, 1, 1:12], weight[:, 2, 1:11]], dim=1)
+                weight = weight.reshape(-1, self.groupsize, weight.shape[2])
+            else:
+                raise NotImplementedError("Only 2,3,4,8 bits are supported.")
+
+            weight = (scales * (weight - zeros))
+            weight = weight.reshape(weight.shape[0] * weight.shape[1], weight.shape[2])
+
+            out = torch.matmul(x.half(), weight)
+        out = out.reshape(out_shape)
+        out = out + self.bias if self.bias is not None else out
+        return out
+
+
+__all__ = ["QuantLinear"]
```

### Comparing `auto_gptq-0.0.5/auto_gptq/nn_modules/qlinear_triton.py` & `auto_gptq-0.1.0/auto_gptq/nn_modules/qlinear_triton.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,485 +1,493 @@
-import math
-import numpy as np
-import torch
-import torch.nn as nn
-from torch.cuda.amp import custom_bwd, custom_fwd
-from logging import getLogger
-
-logger = getLogger(__name__)
-
-try:
-    import triton
-    import triton.language as tl
-    from .triton_utils import custom_autotune
-
-    # code based https://github.com/fpgaminer/GPTQ-triton
-
-    @custom_autotune.autotune(
-        configs=[
-            triton.Config(
-                {'BLOCK_SIZE_M': 64, 'BLOCK_SIZE_N': 256, 'BLOCK_SIZE_K': 32, 'GROUP_SIZE_M': 8},
-                num_stages=4,
-                num_warps=4
-            ),
-            triton.Config(
-                {'BLOCK_SIZE_M': 128, 'BLOCK_SIZE_N': 128, 'BLOCK_SIZE_K': 32, 'GROUP_SIZE_M': 8},
-                num_stages=4,
-                num_warps=4
-            ),
-            triton.Config(
-                {'BLOCK_SIZE_M': 64, 'BLOCK_SIZE_N': 128, 'BLOCK_SIZE_K': 32, 'GROUP_SIZE_M': 8},
-                num_stages=4,
-                num_warps=4
-            ),
-            triton.Config(
-                {'BLOCK_SIZE_M': 128, 'BLOCK_SIZE_N': 32, 'BLOCK_SIZE_K': 32, 'GROUP_SIZE_M': 8},
-                num_stages=4,
-                num_warps=4
-            ),
-            triton.Config(
-                {'BLOCK_SIZE_M': 64, 'BLOCK_SIZE_N': 64, 'BLOCK_SIZE_K': 32, 'GROUP_SIZE_M': 8},
-                num_stages=4,
-                num_warps=4
-            ),
-            triton.Config(
-                {'BLOCK_SIZE_M': 64, 'BLOCK_SIZE_N': 128, 'BLOCK_SIZE_K': 32, 'GROUP_SIZE_M': 8},
-                num_stages=2,
-                num_warps=8
-            ),
-            triton.Config(
-                {'BLOCK_SIZE_M': 64, 'BLOCK_SIZE_N': 64, 'BLOCK_SIZE_K': 64, 'GROUP_SIZE_M': 8},
-                num_stages=3,
-                num_warps=8
-            ),
-            triton.Config(
-                {'BLOCK_SIZE_M': 32, 'BLOCK_SIZE_N': 32, 'BLOCK_SIZE_K': 128, 'GROUP_SIZE_M': 8},
-                num_stages=2,
-                num_warps=4
-            ),
-        ],
-        key=['M', 'N', 'K'],
-        nearest_power_of_two=True,
-        prune_configs_by={
-            'early_config_prune': custom_autotune.matmul248_kernel_config_pruner,
-            'perf_model': None,
-            'top_k': None,
-        },
-    )
-    @triton.jit
-    def matmul_248_kernel(
-        a_ptr, b_ptr, c_ptr,
-        scales_ptr, zeros_ptr, g_ptr,
-        M, N, K,
-        bits, maxq,
-        stride_am, stride_ak,
-        stride_bk, stride_bn,
-        stride_cm, stride_cn,
-        stride_scales, stride_zeros,
-        BLOCK_SIZE_M: tl.constexpr, BLOCK_SIZE_N: tl.constexpr, BLOCK_SIZE_K: tl.constexpr,
-        GROUP_SIZE_M: tl.constexpr
-    ):
-        """
-        Compute the matrix multiplication C = A x B.
-        A is of shape (M, K) float16
-        B is of shape (K//8, N) int32
-        C is of shape (M, N) float16
-        scales is of shape (G, N) float16
-        zeros is of shape (G, N) float16
-        g_ptr is of shape (K) int32
-        """
-        infearure_per_bits = 32 // bits
-
-        pid = tl.program_id(axis=0)
-        num_pid_m = tl.cdiv(M, BLOCK_SIZE_M)
-        num_pid_n = tl.cdiv(N, BLOCK_SIZE_N)
-        num_pid_k = tl.cdiv(K, BLOCK_SIZE_K)
-        num_pid_in_group = GROUP_SIZE_M * num_pid_n
-        group_id = pid // num_pid_in_group
-        first_pid_m = group_id * GROUP_SIZE_M
-        group_size_m = min(num_pid_m - first_pid_m, GROUP_SIZE_M)
-        pid_m = first_pid_m + (pid % group_size_m)
-        pid_n = (pid % num_pid_in_group) // group_size_m
-
-        offs_am = pid_m * BLOCK_SIZE_M + tl.arange(0, BLOCK_SIZE_M)
-        offs_bn = pid_n * BLOCK_SIZE_N + tl.arange(0, BLOCK_SIZE_N)
-        offs_k = tl.arange(0, BLOCK_SIZE_K)
-        a_ptrs = a_ptr + (offs_am[:, None] * stride_am + offs_k[None, :] * stride_ak)  # (BLOCK_SIZE_M, BLOCK_SIZE_K)
-        a_mask = (offs_am[:, None] < M)
-        # b_ptrs is set up such that it repeats elements along the K axis 8 times
-        b_ptrs = b_ptr + (
-            (offs_k[:, None] // infearure_per_bits) * stride_bk + offs_bn[None, :] * stride_bn
-        )  # (BLOCK_SIZE_K, BLOCK_SIZE_N)
-        g_ptrs = g_ptr + offs_k
-        # shifter is used to extract the N bits of each element in the 32-bit word from B
-        scales_ptrs = scales_ptr + offs_bn[None, :]
-        zeros_ptrs = zeros_ptr + (offs_bn[None, :] // infearure_per_bits)
-
-        shifter = (offs_k % infearure_per_bits) * bits
-        zeros_shifter = (offs_bn % infearure_per_bits) * bits
-        accumulator = tl.zeros((BLOCK_SIZE_M, BLOCK_SIZE_N), dtype=tl.float32)
-
-        for k in range(0, num_pid_k):
-            g_idx = tl.load(g_ptrs)
-
-            # Fetch scales and zeros; these are per-outfeature and thus reused in the inner loop
-            scales = tl.load(scales_ptrs + g_idx[:, None] * stride_scales)  # (BLOCK_SIZE_K, BLOCK_SIZE_N,)
-            zeros = tl.load(zeros_ptrs + g_idx[:, None] * stride_zeros)  # (BLOCK_SIZE_K, BLOCK_SIZE_N,)
-
-            zeros = (zeros >> zeros_shifter[None, :]) & maxq
-            zeros = (zeros + 1)
-
-            a = tl.load(a_ptrs, mask=a_mask, other=0.)  # (BLOCK_SIZE_M, BLOCK_SIZE_K)
-            b = tl.load(b_ptrs)  # (BLOCK_SIZE_K, BLOCK_SIZE_N), but repeated
-
-            # Now we need to unpack b (which is N-bit values) into 32-bit values
-            b = (b >> shifter[:, None]) & maxq  # Extract the N-bit values
-            b = (b - zeros) * scales  # Scale and shift
-
-            accumulator += tl.dot(a, b)
-            a_ptrs += BLOCK_SIZE_K
-            b_ptrs += (BLOCK_SIZE_K // infearure_per_bits) * stride_bk
-            g_ptrs += BLOCK_SIZE_K
-
-        c_ptrs = c_ptr + stride_cm * offs_am[:, None] + stride_cn * offs_bn[None, :]
-        c_mask = (offs_am[:, None] < M) & (offs_bn[None, :] < N)
-        tl.store(c_ptrs, accumulator, mask=c_mask)
-
-
-    @custom_autotune.autotune(configs=[
-        triton.Config(
-            {'BLOCK_SIZE_M': 64, 'BLOCK_SIZE_N': 32, 'BLOCK_SIZE_K': 256, 'GROUP_SIZE_M': 8},
-            num_stages=4,
-            num_warps=4
-        ),
-        triton.Config(
-            {'BLOCK_SIZE_M': 128, 'BLOCK_SIZE_N': 32, 'BLOCK_SIZE_K': 128, 'GROUP_SIZE_M': 8},
-            num_stages=4,
-            num_warps=4
-        ),
-        triton.Config(
-            {'BLOCK_SIZE_M': 64, 'BLOCK_SIZE_N': 32, 'BLOCK_SIZE_K': 128, 'GROUP_SIZE_M': 8},
-            num_stages=4,
-            num_warps=4
-        ),
-        triton.Config(
-            {'BLOCK_SIZE_M': 128, 'BLOCK_SIZE_N': 32, 'BLOCK_SIZE_K': 32, 'GROUP_SIZE_M': 8},
-            num_stages=4,
-            num_warps=4
-        ),
-        triton.Config(
-            {'BLOCK_SIZE_M': 64, 'BLOCK_SIZE_N': 32, 'BLOCK_SIZE_K': 64, 'GROUP_SIZE_M': 8},
-            num_stages=4,
-            num_warps=4
-        ),
-        triton.Config(
-            {'BLOCK_SIZE_M': 64, 'BLOCK_SIZE_N': 32, 'BLOCK_SIZE_K': 128, 'GROUP_SIZE_M': 8},
-            num_stages=2,
-            num_warps=8
-        ),
-        triton.Config(
-            {'BLOCK_SIZE_M': 64, 'BLOCK_SIZE_N': 64, 'BLOCK_SIZE_K': 64, 'GROUP_SIZE_M': 8},
-            num_stages=3,
-            num_warps=8
-        ),
-        triton.Config(
-            {'BLOCK_SIZE_M': 32, 'BLOCK_SIZE_N': 128, 'BLOCK_SIZE_K': 32, 'GROUP_SIZE_M': 8},
-            num_stages=2,
-            num_warps=4
-        ),
-    ],
-        key=['M', 'N', 'K'],
-        nearest_power_of_two=True
-    )
-    @triton.jit
-    def transpose_matmul_248_kernel(
-        a_ptr, b_ptr, c_ptr,
-        scales_ptr, zeros_ptr, g_ptr,
-        M, N, K,
-        bits, maxq,
-        stride_am, stride_ak,
-        stride_bk, stride_bn,
-        stride_cm, stride_cn,
-        stride_scales, stride_zeros,
-        BLOCK_SIZE_M: tl.constexpr, BLOCK_SIZE_N: tl.constexpr, BLOCK_SIZE_K: tl.constexpr,
-        GROUP_SIZE_M: tl.constexpr
-    ):
-        """
-        Compute the matrix multiplication C = A x B.
-        A is of shape (M, N) float16
-        B is of shape (K//8, N) int32
-        C is of shape (M, K) float16
-        scales is of shape (G, N) float16
-        zeros is of shape (G, N) float16
-        g_ptr is of shape (K) int32
-        """
-        infearure_per_bits = 32 // bits
-
-        pid = tl.program_id(axis=0)
-        num_pid_m = tl.cdiv(M, BLOCK_SIZE_M)
-        num_pid_k = tl.cdiv(K, BLOCK_SIZE_K)
-        num_pid_n = tl.cdiv(N, BLOCK_SIZE_N)
-        num_pid_in_group = GROUP_SIZE_M * num_pid_k
-        group_id = pid // num_pid_in_group
-        first_pid_m = group_id * GROUP_SIZE_M
-        group_size_m = min(num_pid_m - first_pid_m, GROUP_SIZE_M)
-        pid_m = first_pid_m + (pid % group_size_m)
-        pid_k = (pid % num_pid_in_group) // group_size_m
-
-        offs_am = pid_m * BLOCK_SIZE_M + tl.arange(0, BLOCK_SIZE_M)
-        offs_bk = pid_k * BLOCK_SIZE_K + tl.arange(0, BLOCK_SIZE_K)
-        offs_n = tl.arange(0, BLOCK_SIZE_N)
-        a_ptrs = a_ptr + (offs_am[:, None] * stride_am + offs_n[None, :] * stride_ak)  # (BLOCK_SIZE_M, BLOCK_SIZE_N)
-        a_mask = (offs_am[:, None] < M)
-        # b_ptrs is set up such that it repeats elements along the K axis 8 times
-        b_ptrs = b_ptr + (
-            (offs_bk[:, None] // infearure_per_bits) * stride_bk + offs_n[None, :] * stride_bn
-        )  # (BLOCK_SIZE_K, BLOCK_SIZE_N)
-        g_ptrs = g_ptr + offs_bk
-        g_idx = tl.load(g_ptrs)
-
-        # shifter is used to extract the N bits of each element in the 32-bit word from B
-        scales_ptrs = scales_ptr + offs_n[None, :] + g_idx[:, None] * stride_scales
-        zeros_ptrs = zeros_ptr + (offs_n[None, :] // infearure_per_bits) + g_idx[:, None] * stride_zeros
-
-        shifter = (offs_bk % infearure_per_bits) * bits
-        zeros_shifter = (offs_n % infearure_per_bits) * bits
-        accumulator = tl.zeros((BLOCK_SIZE_M, BLOCK_SIZE_K), dtype=tl.float32)
-
-        for k in range(0, num_pid_n):
-            # Fetch scales and zeros; these are per-outfeature and thus reused in the inner loop
-            scales = tl.load(scales_ptrs)  # (BLOCK_SIZE_K, BLOCK_SIZE_N,)
-            zeros = tl.load(zeros_ptrs)  # (BLOCK_SIZE_K, BLOCK_SIZE_N,)
-
-            zeros = (zeros >> zeros_shifter[None, :]) & maxq
-            zeros = (zeros + 1)
-
-            a = tl.load(a_ptrs, mask=a_mask, other=0.)  # (BLOCK_SIZE_M, BLOCK_SIZE_N)
-            b = tl.load(b_ptrs)  # (BLOCK_SIZE_K, BLOCK_SIZE_N), but repeated
-
-            # Now we need to unpack b (which is N-bit values) into 32-bit values
-            b = (b >> shifter[:, None]) & maxq  # Extract the N-bit values
-            b = (b - zeros) * scales  # Scale and shift
-            b = tl.trans(b)
-
-            accumulator += tl.dot(a, b)
-            a_ptrs += BLOCK_SIZE_N
-            b_ptrs += BLOCK_SIZE_N
-            scales_ptrs += BLOCK_SIZE_N
-            zeros_ptrs += (BLOCK_SIZE_N // infearure_per_bits)
-
-        c_ptrs = c_ptr + stride_cm * offs_am[:, None] + stride_cn * offs_bk[None, :]
-        c_mask = (offs_am[:, None] < M) & (offs_bk[None, :] < K)
-        tl.store(c_ptrs, accumulator, mask=c_mask)
-except ImportError:
-    logger.warning('triton not installed.')
-    raise
-
-
-def matmul248(input, qweight, scales, qzeros, g_idx, bits, maxq):
-    with torch.cuda.device(input.device):
-        output = torch.empty((input.shape[0], qweight.shape[1]), device='cuda', dtype=torch.float16)
-        grid = lambda META: (
-            triton.cdiv(input.shape[0], META['BLOCK_SIZE_M']) * triton.cdiv(qweight.shape[1], META['BLOCK_SIZE_N']),
-        )
-        matmul_248_kernel[grid](
-            input, qweight, output,
-            scales, qzeros, g_idx,
-            input.shape[0], qweight.shape[1], input.shape[1],
-            bits, maxq,
-            input.stride(0), input.stride(1),
-            qweight.stride(0), qweight.stride(1),
-            output.stride(0), output.stride(1),
-            scales.stride(0), qzeros.stride(0)
-        )
-        return output
-
-
-def transpose_matmul248(input, qweight, scales, qzeros, g_idx, bits, maxq):
-    with torch.cuda.device(input.device):
-        output_dim = (qweight.shape[0] * 32) // bits
-        output = torch.empty((input.shape[0], output_dim), device='cuda', dtype=torch.float16)
-        grid = lambda META: (
-            triton.cdiv(input.shape[0], META['BLOCK_SIZE_M']) * triton.cdiv(output_dim, META['BLOCK_SIZE_K']),)
-        transpose_matmul_248_kernel[grid](
-            input, qweight, output,
-            scales, qzeros, g_idx,
-            input.shape[0], qweight.shape[1], output_dim,
-            bits, maxq,
-            input.stride(0), input.stride(1),
-            qweight.stride(0), qweight.stride(1),
-            output.stride(0), output.stride(1),
-            scales.stride(0), qzeros.stride(0)
-        )
-        return output
-
-
-class QuantLinearFunction(torch.autograd.Function):
-
-    @staticmethod
-    @custom_fwd(cast_inputs=torch.float16)
-    def forward(ctx, input, qweight, scales, qzeros, g_idx, bits, maxq):
-        output = matmul248(input, qweight, scales, qzeros, g_idx, bits, maxq)
-        ctx.save_for_backward(qweight, scales, qzeros, g_idx)
-        ctx.bits, ctx.maxq = bits, maxq
-        return output
-
-    @staticmethod
-    @custom_bwd
-    def backward(ctx, grad_output):
-        qweight, scales, qzeros, g_idx = ctx.saved_tensors
-        bits, maxq = ctx.bits, ctx.maxq
-        grad_input = None
-
-        if ctx.needs_input_grad[0]:
-            grad_input = transpose_matmul248(grad_output, qweight, scales, qzeros, g_idx, bits, maxq)
-        return grad_input, None, None, None, None, None, None
-
-
-class QuantLinear(nn.Module):
-    def __init__(
-        self,
-        bits,
-        groupsize,
-        infeatures,
-        outfeatures,
-        bias
-    ):
-        super().__init__()
-        if bits not in [2, 4, 8]:
-            raise NotImplementedError("Only 2,4,8 bits are supported.")
-
-        self.infeatures = infeatures
-        self.outfeatures = outfeatures
-        self.bits = bits
-        self.groupsize = groupsize if groupsize != -1 else infeatures
-        self.maxq = 2 ** self.bits - 1
-
-        self.register_buffer(
-            'qweight',
-            torch.zeros((infeatures // 32 * self.bits, outfeatures), dtype=torch.int32)
-        )
-        self.register_buffer(
-            'qzeros',
-            torch.zeros((math.ceil(infeatures / self.groupsize), outfeatures // 32 * self.bits), dtype=torch.int32)
-        )
-        self.register_buffer(
-            'scales',
-            torch.zeros((math.ceil(infeatures / self.groupsize), outfeatures), dtype=torch.float16)
-        )
-        self.register_buffer(
-            'g_idx',
-            torch.tensor([i // self.groupsize for i in range(infeatures)], dtype=torch.int32)
-        )
-        if bias:
-            self.register_buffer('bias', torch.zeros((outfeatures), dtype=torch.float16))
-        else:
-            self.bias = None
-
-    def pack(self, linear, scales, zeros, g_idx=None):
-        self.g_idx = g_idx.clone() if g_idx is not None else self.g_idx
-
-        scales = scales.t().contiguous()
-        zeros = zeros.t().contiguous()
-        scale_zeros = zeros * scales
-        self.scales = scales.clone().half()
-        if linear.bias is not None:
-            self.bias = linear.bias.clone().half()
-
-        intweight = []
-        for idx in range(self.infeatures):
-            intweight.append(
-                torch.round(
-                    (
-                        linear.weight.data[:, idx] + scale_zeros[self.g_idx[idx]]) / self.scales[self.g_idx[idx]]
-                ).to(torch.int)[:, None]
-            )
-        intweight = torch.cat(intweight, dim=1)
-        intweight = intweight.t().contiguous()
-        intweight = intweight.numpy().astype(np.uint32)
-
-        i = 0
-        row = 0
-        qweight = np.zeros(
-            (intweight.shape[0] // 32 * self.bits, intweight.shape[1]), dtype=np.uint32
-        )
-        while row < qweight.shape[0]:
-            if self.bits in [2, 4, 8]:
-                for j in range(i, i + (32 // self.bits)):
-                    qweight[row] |= intweight[j] << (self.bits * (j - i))
-                i += 32 // self.bits
-                row += 1
-            else:
-                raise NotImplementedError("Only 2,4,8 bits are supported.")
-
-        qweight = qweight.astype(np.int32)
-        self.qweight = torch.from_numpy(qweight)
-
-        zeros -= 1
-        zeros = zeros.numpy().astype(np.uint32)
-        qzeros = np.zeros((zeros.shape[0], zeros.shape[1] // 32 * self.bits), dtype=np.uint32)
-        i = 0
-        col = 0
-        while col < qzeros.shape[1]:
-            if self.bits in [2, 4, 8]:
-                for j in range(i, i + (32 // self.bits)):
-                    qzeros[:, col] |= zeros[:, j] << (self.bits * (j - i))
-                i += 32 // self.bits
-                col += 1
-            else:
-                raise NotImplementedError("Only 2,4,8 bits are supported.")
-
-        qzeros = qzeros.astype(np.int32)
-        self.qzeros = torch.from_numpy(qzeros)
-
-    def forward(self, x):
-        out_shape = x.shape[:-1] + (self.outfeatures,)
-        out = QuantLinearFunction.apply(
-            x.reshape(-1, x.shape[-1]),
-            self.qweight,
-            self.scales,
-            self.qzeros,
-            self.g_idx,
-            self.bits,
-            self.maxq
-        )
-        out = out.reshape(out_shape)
-        out = out + self.bias if self.bias is not None else out
-        return out
-
-
-def autotune_warmup_linear(model, transpose=False, seqlen=2048):
-    """
-    Pre-tunes the quantized kernel
-    """
-    from tqdm import tqdm
-
-    kn_values = {}
-
-    for _, m in model.named_modules():
-        if not isinstance(m, QuantLinear):
-            continue
-
-        k = m.infeatures
-        n = m.outfeatures
-
-        if (k, n) not in kn_values:
-            kn_values[(k, n)] = (m.qweight.cuda(), m.scales.cuda(), m.qzeros.cuda(), m.g_idx.cuda(), m.bits, m.maxq)
-
-    logger.info(f'Found {len(kn_values)} unique KN Linear values.')
-    logger.info('Warming up autotune cache ...')
-    with torch.no_grad():
-        for m in tqdm(range(0, math.ceil(math.log2(seqlen)) + 1)):
-            m = 2 ** m
-            for (k, n), (qweight, scales, qzeros, g_idx, bits, maxq) in kn_values.items():
-                a = torch.randn(m, k, dtype=torch.float16, device='cuda')
-                matmul248(a, qweight, scales, qzeros, g_idx, bits, maxq)
-                if transpose:
-                    a = torch.randn(m, n, dtype=torch.float16, device='cuda')
-                    transpose_matmul248(a, qweight, scales, qzeros, g_idx, bits, maxq)
-    del kn_values
-
-
-__all__ = [
-    "QuantLinear",
-    "autotune_warmup_linear"
-]
+import math
+import numpy as np
+import torch
+import torch.nn as nn
+import transformers
+from torch.cuda.amp import custom_bwd, custom_fwd
+from logging import getLogger
+
+logger = getLogger(__name__)
+
+try:
+    import triton
+    import triton.language as tl
+    from .triton_utils import custom_autotune
+
+    # code based https://github.com/fpgaminer/GPTQ-triton
+
+    @custom_autotune.autotune(
+        configs=[
+            triton.Config(
+                {'BLOCK_SIZE_M': 64, 'BLOCK_SIZE_N': 256, 'BLOCK_SIZE_K': 32, 'GROUP_SIZE_M': 8},
+                num_stages=4,
+                num_warps=4
+            ),
+            triton.Config(
+                {'BLOCK_SIZE_M': 128, 'BLOCK_SIZE_N': 128, 'BLOCK_SIZE_K': 32, 'GROUP_SIZE_M': 8},
+                num_stages=4,
+                num_warps=4
+            ),
+            triton.Config(
+                {'BLOCK_SIZE_M': 64, 'BLOCK_SIZE_N': 128, 'BLOCK_SIZE_K': 32, 'GROUP_SIZE_M': 8},
+                num_stages=4,
+                num_warps=4
+            ),
+            triton.Config(
+                {'BLOCK_SIZE_M': 128, 'BLOCK_SIZE_N': 32, 'BLOCK_SIZE_K': 32, 'GROUP_SIZE_M': 8},
+                num_stages=4,
+                num_warps=4
+            ),
+            triton.Config(
+                {'BLOCK_SIZE_M': 64, 'BLOCK_SIZE_N': 64, 'BLOCK_SIZE_K': 32, 'GROUP_SIZE_M': 8},
+                num_stages=4,
+                num_warps=4
+            ),
+            triton.Config(
+                {'BLOCK_SIZE_M': 64, 'BLOCK_SIZE_N': 128, 'BLOCK_SIZE_K': 32, 'GROUP_SIZE_M': 8},
+                num_stages=2,
+                num_warps=8
+            ),
+            triton.Config(
+                {'BLOCK_SIZE_M': 64, 'BLOCK_SIZE_N': 64, 'BLOCK_SIZE_K': 64, 'GROUP_SIZE_M': 8},
+                num_stages=3,
+                num_warps=8
+            ),
+            triton.Config(
+                {'BLOCK_SIZE_M': 32, 'BLOCK_SIZE_N': 32, 'BLOCK_SIZE_K': 128, 'GROUP_SIZE_M': 8},
+                num_stages=2,
+                num_warps=4
+            ),
+        ],
+        key=['M', 'N', 'K'],
+        nearest_power_of_two=True,
+        prune_configs_by={
+            'early_config_prune': custom_autotune.matmul248_kernel_config_pruner,
+            'perf_model': None,
+            'top_k': None,
+        },
+    )
+    @triton.jit
+    def matmul_248_kernel(
+        a_ptr, b_ptr, c_ptr,
+        scales_ptr, zeros_ptr, g_ptr,
+        M, N, K,
+        bits, maxq,
+        stride_am, stride_ak,
+        stride_bk, stride_bn,
+        stride_cm, stride_cn,
+        stride_scales, stride_zeros,
+        BLOCK_SIZE_M: tl.constexpr, BLOCK_SIZE_N: tl.constexpr, BLOCK_SIZE_K: tl.constexpr,
+        GROUP_SIZE_M: tl.constexpr
+    ):
+        """
+        Compute the matrix multiplication C = A x B.
+        A is of shape (M, K) float16
+        B is of shape (K//8, N) int32
+        C is of shape (M, N) float16
+        scales is of shape (G, N) float16
+        zeros is of shape (G, N) float16
+        g_ptr is of shape (K) int32
+        """
+        infearure_per_bits = 32 // bits
+
+        pid = tl.program_id(axis=0)
+        num_pid_m = tl.cdiv(M, BLOCK_SIZE_M)
+        num_pid_n = tl.cdiv(N, BLOCK_SIZE_N)
+        num_pid_k = tl.cdiv(K, BLOCK_SIZE_K)
+        num_pid_in_group = GROUP_SIZE_M * num_pid_n
+        group_id = pid // num_pid_in_group
+        first_pid_m = group_id * GROUP_SIZE_M
+        group_size_m = min(num_pid_m - first_pid_m, GROUP_SIZE_M)
+        pid_m = first_pid_m + (pid % group_size_m)
+        pid_n = (pid % num_pid_in_group) // group_size_m
+
+        offs_am = pid_m * BLOCK_SIZE_M + tl.arange(0, BLOCK_SIZE_M)
+        offs_bn = pid_n * BLOCK_SIZE_N + tl.arange(0, BLOCK_SIZE_N)
+        offs_k = tl.arange(0, BLOCK_SIZE_K)
+        a_ptrs = a_ptr + (offs_am[:, None] * stride_am + offs_k[None, :] * stride_ak)  # (BLOCK_SIZE_M, BLOCK_SIZE_K)
+        a_mask = (offs_am[:, None] < M)
+        # b_ptrs is set up such that it repeats elements along the K axis 8 times
+        b_ptrs = b_ptr + (
+            (offs_k[:, None] // infearure_per_bits) * stride_bk + offs_bn[None, :] * stride_bn
+        )  # (BLOCK_SIZE_K, BLOCK_SIZE_N)
+        g_ptrs = g_ptr + offs_k
+        # shifter is used to extract the N bits of each element in the 32-bit word from B
+        scales_ptrs = scales_ptr + offs_bn[None, :]
+        zeros_ptrs = zeros_ptr + (offs_bn[None, :] // infearure_per_bits)
+
+        shifter = (offs_k % infearure_per_bits) * bits
+        zeros_shifter = (offs_bn % infearure_per_bits) * bits
+        accumulator = tl.zeros((BLOCK_SIZE_M, BLOCK_SIZE_N), dtype=tl.float32)
+
+        for k in range(0, num_pid_k):
+            g_idx = tl.load(g_ptrs)
+
+            # Fetch scales and zeros; these are per-outfeature and thus reused in the inner loop
+            scales = tl.load(scales_ptrs + g_idx[:, None] * stride_scales)  # (BLOCK_SIZE_K, BLOCK_SIZE_N,)
+            zeros = tl.load(zeros_ptrs + g_idx[:, None] * stride_zeros)  # (BLOCK_SIZE_K, BLOCK_SIZE_N,)
+
+            zeros = (zeros >> zeros_shifter[None, :]) & maxq
+            zeros = (zeros + 1)
+
+            a = tl.load(a_ptrs, mask=a_mask, other=0.)  # (BLOCK_SIZE_M, BLOCK_SIZE_K)
+            b = tl.load(b_ptrs)  # (BLOCK_SIZE_K, BLOCK_SIZE_N), but repeated
+
+            # Now we need to unpack b (which is N-bit values) into 32-bit values
+            b = (b >> shifter[:, None]) & maxq  # Extract the N-bit values
+            b = (b - zeros) * scales  # Scale and shift
+
+            accumulator += tl.dot(a, b)
+            a_ptrs += BLOCK_SIZE_K
+            b_ptrs += (BLOCK_SIZE_K // infearure_per_bits) * stride_bk
+            g_ptrs += BLOCK_SIZE_K
+
+        c_ptrs = c_ptr + stride_cm * offs_am[:, None] + stride_cn * offs_bn[None, :]
+        c_mask = (offs_am[:, None] < M) & (offs_bn[None, :] < N)
+        tl.store(c_ptrs, accumulator, mask=c_mask)
+
+
+    @custom_autotune.autotune(configs=[
+        triton.Config(
+            {'BLOCK_SIZE_M': 64, 'BLOCK_SIZE_N': 32, 'BLOCK_SIZE_K': 256, 'GROUP_SIZE_M': 8},
+            num_stages=4,
+            num_warps=4
+        ),
+        triton.Config(
+            {'BLOCK_SIZE_M': 128, 'BLOCK_SIZE_N': 32, 'BLOCK_SIZE_K': 128, 'GROUP_SIZE_M': 8},
+            num_stages=4,
+            num_warps=4
+        ),
+        triton.Config(
+            {'BLOCK_SIZE_M': 64, 'BLOCK_SIZE_N': 32, 'BLOCK_SIZE_K': 128, 'GROUP_SIZE_M': 8},
+            num_stages=4,
+            num_warps=4
+        ),
+        triton.Config(
+            {'BLOCK_SIZE_M': 128, 'BLOCK_SIZE_N': 32, 'BLOCK_SIZE_K': 32, 'GROUP_SIZE_M': 8},
+            num_stages=4,
+            num_warps=4
+        ),
+        triton.Config(
+            {'BLOCK_SIZE_M': 64, 'BLOCK_SIZE_N': 32, 'BLOCK_SIZE_K': 64, 'GROUP_SIZE_M': 8},
+            num_stages=4,
+            num_warps=4
+        ),
+        triton.Config(
+            {'BLOCK_SIZE_M': 64, 'BLOCK_SIZE_N': 32, 'BLOCK_SIZE_K': 128, 'GROUP_SIZE_M': 8},
+            num_stages=2,
+            num_warps=8
+        ),
+        triton.Config(
+            {'BLOCK_SIZE_M': 64, 'BLOCK_SIZE_N': 64, 'BLOCK_SIZE_K': 64, 'GROUP_SIZE_M': 8},
+            num_stages=3,
+            num_warps=8
+        ),
+        triton.Config(
+            {'BLOCK_SIZE_M': 32, 'BLOCK_SIZE_N': 128, 'BLOCK_SIZE_K': 32, 'GROUP_SIZE_M': 8},
+            num_stages=2,
+            num_warps=4
+        ),
+    ],
+        key=['M', 'N', 'K'],
+        nearest_power_of_two=True
+    )
+    @triton.jit
+    def transpose_matmul_248_kernel(
+        a_ptr, b_ptr, c_ptr,
+        scales_ptr, zeros_ptr, g_ptr,
+        M, N, K,
+        bits, maxq,
+        stride_am, stride_ak,
+        stride_bk, stride_bn,
+        stride_cm, stride_cn,
+        stride_scales, stride_zeros,
+        BLOCK_SIZE_M: tl.constexpr, BLOCK_SIZE_N: tl.constexpr, BLOCK_SIZE_K: tl.constexpr,
+        GROUP_SIZE_M: tl.constexpr
+    ):
+        """
+        Compute the matrix multiplication C = A x B.
+        A is of shape (M, N) float16
+        B is of shape (K//8, N) int32
+        C is of shape (M, K) float16
+        scales is of shape (G, N) float16
+        zeros is of shape (G, N) float16
+        g_ptr is of shape (K) int32
+        """
+        infearure_per_bits = 32 // bits
+
+        pid = tl.program_id(axis=0)
+        num_pid_m = tl.cdiv(M, BLOCK_SIZE_M)
+        num_pid_k = tl.cdiv(K, BLOCK_SIZE_K)
+        num_pid_n = tl.cdiv(N, BLOCK_SIZE_N)
+        num_pid_in_group = GROUP_SIZE_M * num_pid_k
+        group_id = pid // num_pid_in_group
+        first_pid_m = group_id * GROUP_SIZE_M
+        group_size_m = min(num_pid_m - first_pid_m, GROUP_SIZE_M)
+        pid_m = first_pid_m + (pid % group_size_m)
+        pid_k = (pid % num_pid_in_group) // group_size_m
+
+        offs_am = pid_m * BLOCK_SIZE_M + tl.arange(0, BLOCK_SIZE_M)
+        offs_bk = pid_k * BLOCK_SIZE_K + tl.arange(0, BLOCK_SIZE_K)
+        offs_n = tl.arange(0, BLOCK_SIZE_N)
+        a_ptrs = a_ptr + (offs_am[:, None] * stride_am + offs_n[None, :] * stride_ak)  # (BLOCK_SIZE_M, BLOCK_SIZE_N)
+        a_mask = (offs_am[:, None] < M)
+        # b_ptrs is set up such that it repeats elements along the K axis 8 times
+        b_ptrs = b_ptr + (
+            (offs_bk[:, None] // infearure_per_bits) * stride_bk + offs_n[None, :] * stride_bn
+        )  # (BLOCK_SIZE_K, BLOCK_SIZE_N)
+        g_ptrs = g_ptr + offs_bk
+        g_idx = tl.load(g_ptrs)
+
+        # shifter is used to extract the N bits of each element in the 32-bit word from B
+        scales_ptrs = scales_ptr + offs_n[None, :] + g_idx[:, None] * stride_scales
+        zeros_ptrs = zeros_ptr + (offs_n[None, :] // infearure_per_bits) + g_idx[:, None] * stride_zeros
+
+        shifter = (offs_bk % infearure_per_bits) * bits
+        zeros_shifter = (offs_n % infearure_per_bits) * bits
+        accumulator = tl.zeros((BLOCK_SIZE_M, BLOCK_SIZE_K), dtype=tl.float32)
+
+        for k in range(0, num_pid_n):
+            # Fetch scales and zeros; these are per-outfeature and thus reused in the inner loop
+            scales = tl.load(scales_ptrs)  # (BLOCK_SIZE_K, BLOCK_SIZE_N,)
+            zeros = tl.load(zeros_ptrs)  # (BLOCK_SIZE_K, BLOCK_SIZE_N,)
+
+            zeros = (zeros >> zeros_shifter[None, :]) & maxq
+            zeros = (zeros + 1)
+
+            a = tl.load(a_ptrs, mask=a_mask, other=0.)  # (BLOCK_SIZE_M, BLOCK_SIZE_N)
+            b = tl.load(b_ptrs)  # (BLOCK_SIZE_K, BLOCK_SIZE_N), but repeated
+
+            # Now we need to unpack b (which is N-bit values) into 32-bit values
+            b = (b >> shifter[:, None]) & maxq  # Extract the N-bit values
+            b = (b - zeros) * scales  # Scale and shift
+            b = tl.trans(b)
+
+            accumulator += tl.dot(a, b)
+            a_ptrs += BLOCK_SIZE_N
+            b_ptrs += BLOCK_SIZE_N
+            scales_ptrs += BLOCK_SIZE_N
+            zeros_ptrs += (BLOCK_SIZE_N // infearure_per_bits)
+
+        c_ptrs = c_ptr + stride_cm * offs_am[:, None] + stride_cn * offs_bk[None, :]
+        c_mask = (offs_am[:, None] < M) & (offs_bk[None, :] < K)
+        tl.store(c_ptrs, accumulator, mask=c_mask)
+except ImportError:
+    logger.warning('triton not installed.')
+    raise
+
+
+def matmul248(input, qweight, scales, qzeros, g_idx, bits, maxq):
+    with torch.cuda.device(input.device):
+        output = torch.empty((input.shape[0], qweight.shape[1]), device='cuda', dtype=torch.float16)
+        grid = lambda META: (
+            triton.cdiv(input.shape[0], META['BLOCK_SIZE_M']) * triton.cdiv(qweight.shape[1], META['BLOCK_SIZE_N']),
+        )
+        matmul_248_kernel[grid](
+            input, qweight, output,
+            scales, qzeros, g_idx,
+            input.shape[0], qweight.shape[1], input.shape[1],
+            bits, maxq,
+            input.stride(0), input.stride(1),
+            qweight.stride(0), qweight.stride(1),
+            output.stride(0), output.stride(1),
+            scales.stride(0), qzeros.stride(0)
+        )
+        return output
+
+
+def transpose_matmul248(input, qweight, scales, qzeros, g_idx, bits, maxq):
+    with torch.cuda.device(input.device):
+        output_dim = (qweight.shape[0] * 32) // bits
+        output = torch.empty((input.shape[0], output_dim), device='cuda', dtype=torch.float16)
+        grid = lambda META: (
+            triton.cdiv(input.shape[0], META['BLOCK_SIZE_M']) * triton.cdiv(output_dim, META['BLOCK_SIZE_K']),)
+        transpose_matmul_248_kernel[grid](
+            input, qweight, output,
+            scales, qzeros, g_idx,
+            input.shape[0], qweight.shape[1], output_dim,
+            bits, maxq,
+            input.stride(0), input.stride(1),
+            qweight.stride(0), qweight.stride(1),
+            output.stride(0), output.stride(1),
+            scales.stride(0), qzeros.stride(0)
+        )
+        return output
+
+
+class QuantLinearFunction(torch.autograd.Function):
+
+    @staticmethod
+    @custom_fwd(cast_inputs=torch.float16)
+    def forward(ctx, input, qweight, scales, qzeros, g_idx, bits, maxq):
+        output = matmul248(input, qweight, scales, qzeros, g_idx, bits, maxq)
+        ctx.save_for_backward(qweight, scales, qzeros, g_idx)
+        ctx.bits, ctx.maxq = bits, maxq
+        return output
+
+    @staticmethod
+    @custom_bwd
+    def backward(ctx, grad_output):
+        qweight, scales, qzeros, g_idx = ctx.saved_tensors
+        bits, maxq = ctx.bits, ctx.maxq
+        grad_input = None
+
+        if ctx.needs_input_grad[0]:
+            grad_input = transpose_matmul248(grad_output, qweight, scales, qzeros, g_idx, bits, maxq)
+        return grad_input, None, None, None, None, None, None
+
+
+class QuantLinear(nn.Module):
+    def __init__(
+        self,
+        bits,
+        groupsize,
+        infeatures,
+        outfeatures,
+        bias
+    ):
+        super().__init__()
+        if bits not in [2, 4, 8]:
+            raise NotImplementedError("Only 2,4,8 bits are supported.")
+        if infeatures % 256 != 0 or outfeatures % 256 != 0:
+            raise NotImplementedError("in_feature or out_feature must be divisible by 256.")
+        self.infeatures = infeatures
+        self.outfeatures = outfeatures
+        self.bits = bits
+        self.groupsize = groupsize if groupsize != -1 else infeatures
+        self.maxq = 2 ** self.bits - 1
+
+        self.register_buffer(
+            'qweight',
+            torch.zeros((infeatures // 32 * self.bits, outfeatures), dtype=torch.int32)
+        )
+        self.register_buffer(
+            'qzeros',
+            torch.zeros((math.ceil(infeatures / self.groupsize), outfeatures // 32 * self.bits), dtype=torch.int32)
+        )
+        self.register_buffer(
+            'scales',
+            torch.zeros((math.ceil(infeatures / self.groupsize), outfeatures), dtype=torch.float16)
+        )
+        self.register_buffer(
+            'g_idx',
+            torch.tensor([i // self.groupsize for i in range(infeatures)], dtype=torch.int32)
+        )
+        if bias:
+            self.register_buffer('bias', torch.zeros((outfeatures), dtype=torch.float16))
+        else:
+            self.bias = None
+
+    def pack(self, linear, scales, zeros, g_idx=None):
+        W = linear.weight.data.clone()
+        if isinstance(linear, nn.Conv2d):
+            W = W.flatten(1)
+        if isinstance(linear, transformers.pytorch_utils.Conv1D):
+            W = W.t()
+    
+        self.g_idx = g_idx.clone() if g_idx is not None else self.g_idx
+
+        scales = scales.t().contiguous()
+        zeros = zeros.t().contiguous()
+        scale_zeros = zeros * scales
+        self.scales = scales.clone().half()
+        if linear.bias is not None:
+            self.bias = linear.bias.clone().half()
+
+        intweight = []
+        for idx in range(self.infeatures):
+            intweight.append(
+                torch.round(
+                    (
+                        W[:, idx] + scale_zeros[self.g_idx[idx]]) / self.scales[self.g_idx[idx]]
+                ).to(torch.int)[:, None]
+            )
+        intweight = torch.cat(intweight, dim=1)
+        intweight = intweight.t().contiguous()
+        intweight = intweight.numpy().astype(np.uint32)
+
+        i = 0
+        row = 0
+        qweight = np.zeros(
+            (intweight.shape[0] // 32 * self.bits, intweight.shape[1]), dtype=np.uint32
+        )
+        while row < qweight.shape[0]:
+            if self.bits in [2, 4, 8]:
+                for j in range(i, i + (32 // self.bits)):
+                    qweight[row] |= intweight[j] << (self.bits * (j - i))
+                i += 32 // self.bits
+                row += 1
+            else:
+                raise NotImplementedError("Only 2,4,8 bits are supported.")
+
+        qweight = qweight.astype(np.int32)
+        self.qweight = torch.from_numpy(qweight)
+
+        zeros -= 1
+        zeros = zeros.numpy().astype(np.uint32)
+        qzeros = np.zeros((zeros.shape[0], zeros.shape[1] // 32 * self.bits), dtype=np.uint32)
+        i = 0
+        col = 0
+        while col < qzeros.shape[1]:
+            if self.bits in [2, 4, 8]:
+                for j in range(i, i + (32 // self.bits)):
+                    qzeros[:, col] |= zeros[:, j] << (self.bits * (j - i))
+                i += 32 // self.bits
+                col += 1
+            else:
+                raise NotImplementedError("Only 2,4,8 bits are supported.")
+
+        qzeros = qzeros.astype(np.int32)
+        self.qzeros = torch.from_numpy(qzeros)
+
+    def forward(self, x):
+        out_shape = x.shape[:-1] + (self.outfeatures,)
+        out = QuantLinearFunction.apply(
+            x.reshape(-1, x.shape[-1]),
+            self.qweight,
+            self.scales,
+            self.qzeros,
+            self.g_idx,
+            self.bits,
+            self.maxq
+        )
+        out = out.reshape(out_shape)
+        out = out + self.bias if self.bias is not None else out
+        return out
+
+
+def autotune_warmup_linear(model, transpose=False, seqlen=2048):
+    """
+    Pre-tunes the quantized kernel
+    """
+    from tqdm import tqdm
+
+    kn_values = {}
+
+    for _, m in model.named_modules():
+        if not isinstance(m, QuantLinear):
+            continue
+
+        k = m.infeatures
+        n = m.outfeatures
+
+        if (k, n) not in kn_values:
+            kn_values[(k, n)] = (m.qweight.cuda(), m.scales.cuda(), m.qzeros.cuda(), m.g_idx.cuda(), m.bits, m.maxq)
+
+    logger.info(f'Found {len(kn_values)} unique KN Linear values.')
+    logger.info('Warming up autotune cache ...')
+    with torch.no_grad():
+        for m in tqdm(range(0, math.ceil(math.log2(seqlen)) + 1)):
+            m = 2 ** m
+            for (k, n), (qweight, scales, qzeros, g_idx, bits, maxq) in kn_values.items():
+                a = torch.randn(m, k, dtype=torch.float16, device='cuda')
+                matmul248(a, qweight, scales, qzeros, g_idx, bits, maxq)
+                if transpose:
+                    a = torch.randn(m, n, dtype=torch.float16, device='cuda')
+                    transpose_matmul248(a, qweight, scales, qzeros, g_idx, bits, maxq)
+    del kn_values
+
+
+__all__ = [
+    "QuantLinear",
+    "autotune_warmup_linear"
+]
```

### Comparing `auto_gptq-0.0.5/auto_gptq/nn_modules/triton_utils/custom_autotune.py` & `auto_gptq-0.1.0/auto_gptq/nn_modules/triton_utils/custom_autotune.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,174 +1,174 @@
-import builtins
-import math
-import time
-from typing import Dict
-
-import triton
-
-
-#  code based https://github.com/fpgaminer/GPTQ-triton
-"""
-Mostly the same as the autotuner in Triton, but with a few changes like using 40 runs instead of 100.
-"""
-
-
-class CustomizedTritonAutoTuner(triton.KernelInterface):
-    def __init__(
-        self,
-        fn,
-        arg_names,
-        configs,
-        key,
-        reset_to_zero,
-        prune_configs_by: Dict = None,
-        nearest_power_of_two: bool = False
-    ):
-        if not configs:
-            self.configs = [triton.Config({}, num_warps=4, num_stages=2)]
-        else:
-            self.configs = configs
-        self.key_idx = [arg_names.index(k) for k in key]
-        self.nearest_power_of_two = nearest_power_of_two
-        self.cache = {}
-        # hook to reset all required tensor to zeros before relaunching a kernel
-        self.hook = lambda args: 0
-        if reset_to_zero is not None:
-            self.reset_idx = [arg_names.index(k) for k in reset_to_zero]
-
-            def _hook(args):
-                for i in self.reset_idx:
-                    args[i].zero_()
-
-            self.hook = _hook
-        self.arg_names = arg_names
-        # prune configs
-        if prune_configs_by:
-            perf_model, top_k = prune_configs_by['perf_model'], prune_configs_by['top_k']
-            if 'early_config_prune' in prune_configs_by:
-                early_config_prune = prune_configs_by['early_config_prune']
-        else:
-            perf_model, top_k, early_config_prune = None, None, None
-        self.perf_model, self.configs_top_k = perf_model, top_k
-        self.early_config_prune = early_config_prune
-        self.fn = fn
-
-    def _bench(self, *args, config, **meta):
-        # check for conflicts, i.e. meta-parameters both provided
-        # as kwargs and by the autotuner
-        conflicts = meta.keys() & config.kwargs.keys()
-        if conflicts:
-            raise ValueError(f"Conflicting meta-parameters: {', '.join(conflicts)}."
-                             " Make sure that you don't re-define auto-tuned symbols.")
-        # augment meta-parameters with tunable ones
-        current = dict(meta, **config.kwargs)
-
-        def kernel_call():
-            if config.pre_hook:
-                config.pre_hook(self.nargs)
-            self.hook(args)
-            self.fn.run(*args, num_warps=config.num_warps, num_stages=config.num_stages, **current)
-
-        try:
-            # In testings using only 40 reps seems to be close enough and it appears to be what PyTorch uses
-            # PyTorch also sets fast_flush to True, but I didn't see any speedup so I'll leave the default
-            return triton.testing.do_bench(kernel_call, percentiles=(0.5, 0.2, 0.8), rep=40)
-        except triton.compiler.OutOfResources:
-            return (float('inf'), float('inf'), float('inf'))
-
-    def run(self, *args, **kwargs):
-        self.nargs = dict(zip(self.arg_names, args))
-        if len(self.configs) > 1:
-            key = tuple(args[i] for i in self.key_idx)
-
-            # This reduces the amount of autotuning by rounding the keys to the nearest power of two
-            # In my testing this gives decent results, and greatly reduces the amount of tuning required
-            if self.nearest_power_of_two:
-                key = tuple([2 ** int(math.log2(x) + 0.5) for x in key])
-
-            if key not in self.cache:
-                # prune configs
-                pruned_configs = self.prune_configs(kwargs)
-                bench_start = time.time()
-                timings = {config: self._bench(*args, config=config, **kwargs) for config in pruned_configs}
-                bench_end = time.time()
-                self.bench_time = bench_end - bench_start
-                self.cache[key] = builtins.min(timings, key=timings.get)
-                self.hook(args)
-                self.configs_timings = timings
-            config = self.cache[key]
-        else:
-            config = self.configs[0]
-        self.best_config = config
-        if config.pre_hook is not None:
-            config.pre_hook(self.nargs)
-        return self.fn.run(*args, num_warps=config.num_warps, num_stages=config.num_stages, **kwargs, **config.kwargs)
-
-    def prune_configs(self, kwargs):
-        pruned_configs = self.configs
-        if self.early_config_prune:
-            pruned_configs = self.early_config_prune(self.configs, self.nargs)
-        if self.perf_model:
-            top_k = self.configs_top_k
-            if isinstance(top_k, float) and top_k <= 1.0:
-                top_k = int(len(self.configs) * top_k)
-            if len(pruned_configs) > top_k:
-                est_timing = {
-                    config: self.perf_model(**self.nargs, **kwargs, **config.kwargs, num_stages=config.num_stages,
-                                            num_warps=config.num_warps) for config in pruned_configs}
-                pruned_configs = sorted(est_timing.keys(), key=lambda x: est_timing[x])[:top_k]
-        return pruned_configs
-
-    def warmup(self, *args, **kwargs):
-        self.nargs = dict(zip(self.arg_names, args))
-        for config in self.prune_configs(kwargs):
-            self.fn.warmup(
-                *args,
-                num_warps=config.num_warps,
-                num_stages=config.num_stages,
-                **kwargs,
-                **config.kwargs,
-            )
-        self.nargs = None
-
-
-def autotune(configs, key, prune_configs_by=None, reset_to_zero=None, nearest_power_of_two=False):
-    def decorator(fn):
-        return CustomizedTritonAutoTuner(
-            fn, fn.arg_names, configs, key, reset_to_zero, prune_configs_by, nearest_power_of_two
-        )
-
-    return decorator
-
-
-def matmul248_kernel_config_pruner(configs, nargs):
-    """
-    The main purpose of this function is to shrink BLOCK_SIZE_* when the corresponding dimension is smaller.
-    """
-    m = max(2 ** int(math.ceil(math.log2(nargs['M']))), 16)
-    n = max(2 ** int(math.ceil(math.log2(nargs['N']))), 16)
-    k = max(2 ** int(math.ceil(math.log2(nargs['K']))), 16)
-
-    used = set()
-    for config in configs:
-        block_size_m = min(m, config.kwargs['BLOCK_SIZE_M'])
-        block_size_n = min(n, config.kwargs['BLOCK_SIZE_N'])
-        block_size_k = min(k, config.kwargs['BLOCK_SIZE_K'])
-        group_size_m = config.kwargs['GROUP_SIZE_M']
-
-        if (block_size_m, block_size_n, block_size_k, group_size_m, config.num_stages, config.num_warps) in used:
-            continue
-
-        used.add((block_size_m, block_size_n, block_size_k, group_size_m, config.num_stages, config.num_warps))
-        yield triton.Config(
-            {
-                'BLOCK_SIZE_M': block_size_m,
-                'BLOCK_SIZE_N': block_size_n,
-                'BLOCK_SIZE_K': block_size_k,
-                'GROUP_SIZE_M': group_size_m
-            },
-            num_stages=config.num_stages,
-            num_warps=config.num_warps
-        )
-
-
-__all__ = ["autotune"]
+import builtins
+import math
+import time
+from typing import Dict
+
+import triton
+
+
+#  code based https://github.com/fpgaminer/GPTQ-triton
+"""
+Mostly the same as the autotuner in Triton, but with a few changes like using 40 runs instead of 100.
+"""
+
+
+class CustomizedTritonAutoTuner(triton.KernelInterface):
+    def __init__(
+        self,
+        fn,
+        arg_names,
+        configs,
+        key,
+        reset_to_zero,
+        prune_configs_by: Dict = None,
+        nearest_power_of_two: bool = False
+    ):
+        if not configs:
+            self.configs = [triton.Config({}, num_warps=4, num_stages=2)]
+        else:
+            self.configs = configs
+        self.key_idx = [arg_names.index(k) for k in key]
+        self.nearest_power_of_two = nearest_power_of_two
+        self.cache = {}
+        # hook to reset all required tensor to zeros before relaunching a kernel
+        self.hook = lambda args: 0
+        if reset_to_zero is not None:
+            self.reset_idx = [arg_names.index(k) for k in reset_to_zero]
+
+            def _hook(args):
+                for i in self.reset_idx:
+                    args[i].zero_()
+
+            self.hook = _hook
+        self.arg_names = arg_names
+        # prune configs
+        if prune_configs_by:
+            perf_model, top_k = prune_configs_by['perf_model'], prune_configs_by['top_k']
+            if 'early_config_prune' in prune_configs_by:
+                early_config_prune = prune_configs_by['early_config_prune']
+        else:
+            perf_model, top_k, early_config_prune = None, None, None
+        self.perf_model, self.configs_top_k = perf_model, top_k
+        self.early_config_prune = early_config_prune
+        self.fn = fn
+
+    def _bench(self, *args, config, **meta):
+        # check for conflicts, i.e. meta-parameters both provided
+        # as kwargs and by the autotuner
+        conflicts = meta.keys() & config.kwargs.keys()
+        if conflicts:
+            raise ValueError(f"Conflicting meta-parameters: {', '.join(conflicts)}."
+                             " Make sure that you don't re-define auto-tuned symbols.")
+        # augment meta-parameters with tunable ones
+        current = dict(meta, **config.kwargs)
+
+        def kernel_call():
+            if config.pre_hook:
+                config.pre_hook(self.nargs)
+            self.hook(args)
+            self.fn.run(*args, num_warps=config.num_warps, num_stages=config.num_stages, **current)
+
+        try:
+            # In testings using only 40 reps seems to be close enough and it appears to be what PyTorch uses
+            # PyTorch also sets fast_flush to True, but I didn't see any speedup so I'll leave the default
+            return triton.testing.do_bench(kernel_call, percentiles=(0.5, 0.2, 0.8), rep=40)
+        except triton.compiler.OutOfResources:
+            return (float('inf'), float('inf'), float('inf'))
+
+    def run(self, *args, **kwargs):
+        self.nargs = dict(zip(self.arg_names, args))
+        if len(self.configs) > 1:
+            key = tuple(args[i] for i in self.key_idx)
+
+            # This reduces the amount of autotuning by rounding the keys to the nearest power of two
+            # In my testing this gives decent results, and greatly reduces the amount of tuning required
+            if self.nearest_power_of_two:
+                key = tuple([2 ** int(math.log2(x) + 0.5) for x in key])
+
+            if key not in self.cache:
+                # prune configs
+                pruned_configs = self.prune_configs(kwargs)
+                bench_start = time.time()
+                timings = {config: self._bench(*args, config=config, **kwargs) for config in pruned_configs}
+                bench_end = time.time()
+                self.bench_time = bench_end - bench_start
+                self.cache[key] = builtins.min(timings, key=timings.get)
+                self.hook(args)
+                self.configs_timings = timings
+            config = self.cache[key]
+        else:
+            config = self.configs[0]
+        self.best_config = config
+        if config.pre_hook is not None:
+            config.pre_hook(self.nargs)
+        return self.fn.run(*args, num_warps=config.num_warps, num_stages=config.num_stages, **kwargs, **config.kwargs)
+
+    def prune_configs(self, kwargs):
+        pruned_configs = self.configs
+        if self.early_config_prune:
+            pruned_configs = self.early_config_prune(self.configs, self.nargs)
+        if self.perf_model:
+            top_k = self.configs_top_k
+            if isinstance(top_k, float) and top_k <= 1.0:
+                top_k = int(len(self.configs) * top_k)
+            if len(pruned_configs) > top_k:
+                est_timing = {
+                    config: self.perf_model(**self.nargs, **kwargs, **config.kwargs, num_stages=config.num_stages,
+                                            num_warps=config.num_warps) for config in pruned_configs}
+                pruned_configs = sorted(est_timing.keys(), key=lambda x: est_timing[x])[:top_k]
+        return pruned_configs
+
+    def warmup(self, *args, **kwargs):
+        self.nargs = dict(zip(self.arg_names, args))
+        for config in self.prune_configs(kwargs):
+            self.fn.warmup(
+                *args,
+                num_warps=config.num_warps,
+                num_stages=config.num_stages,
+                **kwargs,
+                **config.kwargs,
+            )
+        self.nargs = None
+
+
+def autotune(configs, key, prune_configs_by=None, reset_to_zero=None, nearest_power_of_two=False):
+    def decorator(fn):
+        return CustomizedTritonAutoTuner(
+            fn, fn.arg_names, configs, key, reset_to_zero, prune_configs_by, nearest_power_of_two
+        )
+
+    return decorator
+
+
+def matmul248_kernel_config_pruner(configs, nargs):
+    """
+    The main purpose of this function is to shrink BLOCK_SIZE_* when the corresponding dimension is smaller.
+    """
+    m = max(2 ** int(math.ceil(math.log2(nargs['M']))), 16)
+    n = max(2 ** int(math.ceil(math.log2(nargs['N']))), 16)
+    k = max(2 ** int(math.ceil(math.log2(nargs['K']))), 16)
+
+    used = set()
+    for config in configs:
+        block_size_m = min(m, config.kwargs['BLOCK_SIZE_M'])
+        block_size_n = min(n, config.kwargs['BLOCK_SIZE_N'])
+        block_size_k = min(k, config.kwargs['BLOCK_SIZE_K'])
+        group_size_m = config.kwargs['GROUP_SIZE_M']
+
+        if (block_size_m, block_size_n, block_size_k, group_size_m, config.num_stages, config.num_warps) in used:
+            continue
+
+        used.add((block_size_m, block_size_n, block_size_k, group_size_m, config.num_stages, config.num_warps))
+        yield triton.Config(
+            {
+                'BLOCK_SIZE_M': block_size_m,
+                'BLOCK_SIZE_N': block_size_n,
+                'BLOCK_SIZE_K': block_size_k,
+                'GROUP_SIZE_M': group_size_m
+            },
+            num_stages=config.num_stages,
+            num_warps=config.num_warps
+        )
+
+
+__all__ = ["autotune"]
```

### Comparing `auto_gptq-0.0.5/auto_gptq/quantization/gptq.py` & `auto_gptq-0.1.0/auto_gptq/quantization/gptq.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,181 +1,181 @@
-import math
-import os
-import time
-from logging import getLogger
-
-import torch
-import torch.nn as nn
-import transformers
-
-from .quantizer import Quantizer
-
-
-logger = getLogger(__name__)
-
-torch.backends.cuda.matmul.allow_tf32 = False
-torch.backends.cudnn.allow_tf32 = False
-
-
-class GPTQ:
-    def __init__(self, layer):
-        self.layer = layer
-        self.dev = self.layer.weight.device
-        W = layer.weight.data.clone()
-        if isinstance(self.layer, nn.Conv2d):
-            W = W.flatten(1)
-        if isinstance(self.layer, transformers.Conv1D):
-            W = W.t()
-        self.rows = W.shape[0]
-        self.columns = W.shape[1]
-        self.H = torch.zeros((self.columns, self.columns), device=self.dev)
-        self.nsamples = 0
-        self.quantizer = Quantizer()
-
-    def add_batch(self, inp, out):
-        if os.environ.get("DEBUG"):
-            self.inp1 = inp
-            self.out1 = out
-        if len(inp.shape) == 2:
-            inp = inp.unsqueeze(0)
-        tmp = inp.shape[0]
-        if isinstance(self.layer, nn.Linear) or isinstance(self.layer, transformers.Conv1D):
-            if len(inp.shape) == 3:
-                inp = inp.reshape((-1, inp.shape[-1]))
-            inp = inp.t()
-        if isinstance(self.layer, nn.Conv2d):
-            unfold = nn.Unfold(
-                self.layer.kernel_size,
-                dilation=self.layer.dilation,
-                padding=self.layer.padding,
-                stride=self.layer.stride
-            )
-            inp = unfold(inp)
-            inp = inp.permute([1, 0, 2])
-            inp = inp.flatten(1)
-        self.H *= self.nsamples / (self.nsamples + tmp)
-        self.nsamples += tmp
-        # inp = inp.float()
-        inp = math.sqrt(2 / self.nsamples) * inp.float()
-        # self.H += 2 / self.nsamples * inp.matmul(inp.t())
-        self.H += inp.matmul(inp.t())
-
-    def fasterquant(
-        self, blocksize=128, percdamp=.01, groupsize=-1, actorder=False
-    ):
-        W = self.layer.weight.data.clone()
-        if isinstance(self.layer, nn.Conv2d):
-            W = W.flatten(1)
-        if isinstance(self.layer, transformers.Conv1D):
-            W = W.t()
-        W = W.float()
-
-        tick = time.time()
-
-        if not self.quantizer.ready():
-            self.quantizer.find_params(W, weight=True)
-
-        H = self.H
-        del self.H
-        dead = torch.diag(H) == 0
-        H[dead, dead] = 1
-        W[:, dead] = 0
-
-        if actorder:
-            perm = torch.argsort(torch.diag(H), descending=True)
-            W = W[:, perm]
-            H = H[perm][:, perm]
-
-        Losses = torch.zeros_like(W)
-        Q = torch.zeros_like(W)
-
-        damp = percdamp * torch.mean(torch.diag(H))
-        diag = torch.arange(self.columns, device=self.dev)
-        H[diag, diag] += damp
-        H = torch.linalg.cholesky(H)
-        H = torch.cholesky_inverse(H)
-        H = torch.linalg.cholesky(H, upper=True)
-        Hinv = H
-
-        g_idx = []
-        scale = []
-        zero = []
-        now_idx = 1
-
-        for i1 in range(0, self.columns, blocksize):
-            i2 = min(i1 + blocksize, self.columns)
-            count = i2 - i1
-
-            W1 = W[:, i1:i2].clone()
-            Q1 = torch.zeros_like(W1)
-            Err1 = torch.zeros_like(W1)
-            Losses1 = torch.zeros_like(W1)
-            Hinv1 = Hinv[i1:i2, i1:i2]
-
-            for i in range(count):
-                w = W1[:, i]
-                d = Hinv1[i, i]
-
-                if groupsize != -1:
-                    if (i1 + i) % groupsize == 0:
-                        self.quantizer.find_params(W[:, (i1 + i):(i1 + i + groupsize)], weight=True)
-
-                    if ((i1 + i) // groupsize) - now_idx == -1:
-                        scale.append(self.quantizer.scale)
-                        zero.append(self.quantizer.zero)
-                        now_idx += 1
-
-                q = self.quantizer.quantize(w.unsqueeze(1)).flatten()
-                Q1[:, i] = q
-                Losses1[:, i] = (w - q) ** 2 / d ** 2
-
-                err1 = (w - q) / d
-                W1[:, i:] -= err1.unsqueeze(1).matmul(Hinv1[i, i:].unsqueeze(0))
-                Err1[:, i] = err1
-
-            Q[:, i1:i2] = Q1
-            Losses[:, i1:i2] = Losses1 / 2
-
-            W[:, i2:] -= Err1.matmul(Hinv[i1:i2, i2:])
-
-            if os.environ.get("DEBUG"):
-                self.layer.weight.data[:, :i2] = Q[:, :i2]
-                self.layer.weight.data[:, i2:] = W[:, i2:]
-                logger.debug(torch.sum((self.layer(self.inp1) - self.out1) ** 2))
-                logger.debug(torch.sum(Losses))
-
-        torch.cuda.synchronize()
-        logger.info(f'duration: {(time.time() - tick)}')
-        logger.info(f'avg loss: {torch.sum(Losses).item() / self.nsamples}')
-
-        groupsize = groupsize if groupsize != -1 else self.columns
-        g_idx = [i // groupsize for i in range(self.columns)]
-        g_idx = torch.tensor(g_idx, dtype=torch.int32, device=Q.device)
-        if actorder:
-            invperm = torch.argsort(perm)
-            Q = Q[:, invperm]
-            g_idx = g_idx[invperm]
-
-        if isinstance(self.layer, transformers.Conv1D):
-            Q = Q.t()
-        self.layer.weight.data = Q.reshape(self.layer.weight.shape).to(self.layer.weight.data.dtype)
-        if os.environ.get("DEBUG"):
-            logger.debug(torch.sum((self.layer(self.inp1) - self.out1) ** 2))
-
-        if scale == []:
-            scale.append(self.quantizer.scale)
-            zero.append(self.quantizer.zero)
-        scale = torch.cat(scale, dim=1)
-        zero = torch.cat(zero, dim=1)
-        return scale, zero, g_idx
-
-    def free(self):
-        if os.environ.get("DEBUG"):
-            self.inp1 = None
-            self.out1 = None
-        self.H = None
-        self.Losses = None
-        self.Trace = None
-        torch.cuda.empty_cache()
-
-
-__all__ = ["GPTQ"]
+import math
+import os
+import time
+from logging import getLogger
+
+import torch
+import torch.nn as nn
+import transformers
+
+from .quantizer import Quantizer
+
+
+logger = getLogger(__name__)
+
+torch.backends.cuda.matmul.allow_tf32 = False
+torch.backends.cudnn.allow_tf32 = False
+
+
+class GPTQ:
+    def __init__(self, layer):
+        self.layer = layer
+        self.dev = self.layer.weight.device
+        W = layer.weight.data.clone()
+        if isinstance(self.layer, nn.Conv2d):
+            W = W.flatten(1)
+        if isinstance(self.layer, transformers.pytorch_utils.Conv1D):
+            W = W.t()
+        self.rows = W.shape[0]
+        self.columns = W.shape[1]
+        self.H = torch.zeros((self.columns, self.columns), device=self.dev)
+        self.nsamples = 0
+        self.quantizer = Quantizer()
+
+    def add_batch(self, inp, out):
+        if os.environ.get("DEBUG"):
+            self.inp1 = inp
+            self.out1 = out
+        if len(inp.shape) == 2:
+            inp = inp.unsqueeze(0)
+        tmp = inp.shape[0]
+        if isinstance(self.layer, nn.Linear) or isinstance(self.layer, transformers.Conv1D):
+            if len(inp.shape) == 3:
+                inp = inp.reshape((-1, inp.shape[-1]))
+            inp = inp.t()
+        if isinstance(self.layer, nn.Conv2d):
+            unfold = nn.Unfold(
+                self.layer.kernel_size,
+                dilation=self.layer.dilation,
+                padding=self.layer.padding,
+                stride=self.layer.stride
+            )
+            inp = unfold(inp)
+            inp = inp.permute([1, 0, 2])
+            inp = inp.flatten(1)
+        self.H *= self.nsamples / (self.nsamples + tmp)
+        self.nsamples += tmp
+        # inp = inp.float()
+        inp = math.sqrt(2 / self.nsamples) * inp.float()
+        # self.H += 2 / self.nsamples * inp.matmul(inp.t())
+        self.H += inp.matmul(inp.t())
+
+    def fasterquant(
+        self, blocksize=128, percdamp=.01, groupsize=-1, actorder=False
+    ):
+        W = self.layer.weight.data.clone()
+        if isinstance(self.layer, nn.Conv2d):
+            W = W.flatten(1)
+        if isinstance(self.layer, transformers.Conv1D):
+            W = W.t()
+        W = W.float()
+
+        tick = time.time()
+
+        if not self.quantizer.ready():
+            self.quantizer.find_params(W, weight=True)
+
+        H = self.H
+        del self.H
+        dead = torch.diag(H) == 0
+        H[dead, dead] = 1
+        W[:, dead] = 0
+
+        if actorder:
+            perm = torch.argsort(torch.diag(H), descending=True)
+            W = W[:, perm]
+            H = H[perm][:, perm]
+
+        Losses = torch.zeros_like(W)
+        Q = torch.zeros_like(W)
+
+        damp = percdamp * torch.mean(torch.diag(H))
+        diag = torch.arange(self.columns, device=self.dev)
+        H[diag, diag] += damp
+        H = torch.linalg.cholesky(H)
+        H = torch.cholesky_inverse(H)
+        H = torch.linalg.cholesky(H, upper=True)
+        Hinv = H
+
+        g_idx = []
+        scale = []
+        zero = []
+        now_idx = 1
+
+        for i1 in range(0, self.columns, blocksize):
+            i2 = min(i1 + blocksize, self.columns)
+            count = i2 - i1
+
+            W1 = W[:, i1:i2].clone()
+            Q1 = torch.zeros_like(W1)
+            Err1 = torch.zeros_like(W1)
+            Losses1 = torch.zeros_like(W1)
+            Hinv1 = Hinv[i1:i2, i1:i2]
+
+            for i in range(count):
+                w = W1[:, i]
+                d = Hinv1[i, i]
+
+                if groupsize != -1:
+                    if (i1 + i) % groupsize == 0:
+                        self.quantizer.find_params(W[:, (i1 + i):(i1 + i + groupsize)], weight=True)
+
+                    if ((i1 + i) // groupsize) - now_idx == -1:
+                        scale.append(self.quantizer.scale)
+                        zero.append(self.quantizer.zero)
+                        now_idx += 1
+
+                q = self.quantizer.quantize(w.unsqueeze(1)).flatten()
+                Q1[:, i] = q
+                Losses1[:, i] = (w - q) ** 2 / d ** 2
+
+                err1 = (w - q) / d
+                W1[:, i:] -= err1.unsqueeze(1).matmul(Hinv1[i, i:].unsqueeze(0))
+                Err1[:, i] = err1
+
+            Q[:, i1:i2] = Q1
+            Losses[:, i1:i2] = Losses1 / 2
+
+            W[:, i2:] -= Err1.matmul(Hinv[i1:i2, i2:])
+
+            if os.environ.get("DEBUG"):
+                self.layer.weight.data[:, :i2] = Q[:, :i2]
+                self.layer.weight.data[:, i2:] = W[:, i2:]
+                logger.debug(torch.sum((self.layer(self.inp1) - self.out1) ** 2))
+                logger.debug(torch.sum(Losses))
+
+        torch.cuda.synchronize()
+        logger.info(f'duration: {(time.time() - tick)}')
+        logger.info(f'avg loss: {torch.sum(Losses).item() / self.nsamples}')
+
+        groupsize = groupsize if groupsize != -1 else self.columns
+        g_idx = [i // groupsize for i in range(self.columns)]
+        g_idx = torch.tensor(g_idx, dtype=torch.int32, device=Q.device)
+        if actorder:
+            invperm = torch.argsort(perm)
+            Q = Q[:, invperm]
+            g_idx = g_idx[invperm]
+
+        if isinstance(self.layer, transformers.Conv1D):
+            Q = Q.t()
+        self.layer.weight.data = Q.reshape(self.layer.weight.shape).type_as(self.layer.weight.data)
+        if os.environ.get("DEBUG"):
+            logger.debug(torch.sum((self.layer(self.inp1) - self.out1) ** 2))
+
+        if scale == []:
+            scale.append(self.quantizer.scale)
+            zero.append(self.quantizer.zero)
+        scale = torch.cat(scale, dim=1)
+        zero = torch.cat(zero, dim=1)
+        return scale, zero, g_idx
+
+    def free(self):
+        if os.environ.get("DEBUG"):
+            self.inp1 = None
+            self.out1 = None
+        self.H = None
+        self.Losses = None
+        self.Trace = None
+        torch.cuda.empty_cache()
+
+
+__all__ = ["GPTQ"]
```

### Comparing `auto_gptq-0.0.5/auto_gptq/quantization/quantizer.py` & `auto_gptq-0.1.0/auto_gptq/quantization/quantizer.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,137 +1,137 @@
-from logging import getLogger
-
-import torch
-import torch.nn as nn
-
-
-logger = getLogger(__name__)
-
-
-def quantize(x, scale, zero, maxq):
-    if maxq < 0:
-        return (x > scale / 2).float() * scale + (x < zero / 2).float() * zero
-    q = torch.clamp(torch.round(x / scale) + zero, 0, maxq)
-    return scale * (q - zero)
-
-
-class Quantizer(nn.Module):
-
-    def __init__(self, shape=1):
-        super(Quantizer, self).__init__()
-        self.register_buffer('maxq', torch.tensor(0))
-        self.register_buffer('scale', torch.zeros(shape))
-        self.register_buffer('zero', torch.zeros(shape))
-
-    def configure(
-        self,
-        bits, perchannel=False, sym=True,
-        mse=False, norm=2.4, grid=100, maxshrink=.8,
-        trits=False
-    ):
-
-        self.maxq = torch.tensor(2 ** bits - 1)
-        self.perchannel = perchannel
-        self.sym = sym
-        self.mse = mse
-        self.norm = norm
-        self.grid = grid
-        self.maxshrink = maxshrink
-        if trits:
-            self.maxq = torch.tensor(-1)
-
-    def find_params(self, x, weight=False):
-        dev = x.device
-        self.maxq = self.maxq.to(dev)
-
-        shape = x.shape
-        if self.perchannel:
-            if weight:
-                x = x.flatten(1)
-            else:
-                if len(shape) == 4:
-                    x = x.permute([1, 0, 2, 3])
-                    x = x.flatten(1)
-                if len(shape) == 3:
-                    x = x.reshape((-1, shape[-1])).t()
-                if len(shape) == 2:
-                    x = x.t()
-        else:
-            x = x.flatten().unsqueeze(0)
-
-        tmp = torch.zeros(x.shape[0], device=dev)
-        xmin = torch.minimum(x.min(1)[0], tmp)
-        xmax = torch.maximum(x.max(1)[0], tmp)
-
-        if self.sym:
-            xmax = torch.maximum(torch.abs(xmin), xmax)
-            tmp = xmin < 0
-            if torch.any(tmp):
-                xmin[tmp] = -xmax[tmp]
-        tmp = (xmin == 0) & (xmax == 0)
-        xmin[tmp] = -1
-        xmax[tmp] = +1
-
-        if self.maxq < 0:
-            self.scale = xmax
-            self.zero = xmin
-        else:
-            self.scale = (xmax - xmin) / self.maxq
-            if self.sym:
-                self.zero = torch.full_like(self.scale, (self.maxq + 1) / 2)
-            else:
-                self.zero = torch.round(-xmin / self.scale)
-
-        if self.mse:
-            best = torch.full([x.shape[0]], float('inf'), device=dev)
-            for i in range(int(self.maxshrink * self.grid)):
-                p = 1 - i / self.grid
-                xmin1 = p * xmin
-                xmax1 = p * xmax
-                scale1 = (xmax1 - xmin1) / self.maxq
-                zero1 = torch.round(-xmin1 / scale1) if not self.sym else self.zero
-                q = quantize(x, scale1.unsqueeze(1), zero1.unsqueeze(1), self.maxq)
-                q -= x
-                q.abs_()
-                q.pow_(self.norm)
-                err = torch.sum(q, 1)
-                tmp = err < best
-                if torch.any(tmp):
-                    best[tmp] = err[tmp]
-                    self.scale[tmp] = scale1[tmp]
-                    self.zero[tmp] = zero1[tmp]
-        if not self.perchannel:
-            if weight:
-                tmp = shape[0]
-            else:
-                tmp = shape[1] if len(shape) != 3 else shape[2]
-            self.scale = self.scale.repeat(tmp)
-            self.zero = self.zero.repeat(tmp)
-
-        if weight:
-            shape = [-1] + [1] * (len(shape) - 1)
-            self.scale = self.scale.reshape(shape)
-            self.zero = self.zero.reshape(shape)
-            return
-        if len(shape) == 4:
-            self.scale = self.scale.reshape((1, -1, 1, 1))
-            self.zero = self.zero.reshape((1, -1, 1, 1))
-        if len(shape) == 3:
-            self.scale = self.scale.reshape((1, 1, -1))
-            self.zero = self.zero.reshape((1, 1, -1))
-        if len(shape) == 2:
-            self.scale = self.scale.unsqueeze(0)
-            self.zero = self.zero.unsqueeze(0)
-
-    def quantize(self, x):
-        if self.ready():
-            return quantize(x, self.scale, self.zero, self.maxq)
-        return x
-
-    def enabled(self):
-        return self.maxq > 0
-
-    def ready(self):
-        return torch.all(self.scale != 0)
-
-
-__all__ = ["Quantizer"]
+from logging import getLogger
+
+import torch
+import torch.nn as nn
+
+
+logger = getLogger(__name__)
+
+
+def quantize(x, scale, zero, maxq):
+    if maxq < 0:
+        return (x > scale / 2).float() * scale + (x < zero / 2).float() * zero
+    q = torch.clamp(torch.round(x / scale) + zero, 0, maxq)
+    return scale * (q - zero)
+
+
+class Quantizer(nn.Module):
+
+    def __init__(self, shape=1):
+        super(Quantizer, self).__init__()
+        self.register_buffer('maxq', torch.tensor(0))
+        self.register_buffer('scale', torch.zeros(shape))
+        self.register_buffer('zero', torch.zeros(shape))
+
+    def configure(
+        self,
+        bits, perchannel=False, sym=True,
+        mse=False, norm=2.4, grid=100, maxshrink=.8,
+        trits=False
+    ):
+
+        self.maxq = torch.tensor(2 ** bits - 1)
+        self.perchannel = perchannel
+        self.sym = sym
+        self.mse = mse
+        self.norm = norm
+        self.grid = grid
+        self.maxshrink = maxshrink
+        if trits:
+            self.maxq = torch.tensor(-1)
+
+    def find_params(self, x, weight=False):
+        dev = x.device
+        self.maxq = self.maxq.to(dev)
+
+        shape = x.shape
+        if self.perchannel:
+            if weight:
+                x = x.flatten(1)
+            else:
+                if len(shape) == 4:
+                    x = x.permute([1, 0, 2, 3])
+                    x = x.flatten(1)
+                if len(shape) == 3:
+                    x = x.reshape((-1, shape[-1])).t()
+                if len(shape) == 2:
+                    x = x.t()
+        else:
+            x = x.flatten().unsqueeze(0)
+
+        tmp = torch.zeros(x.shape[0], device=dev)
+        xmin = torch.minimum(x.min(1)[0], tmp)
+        xmax = torch.maximum(x.max(1)[0], tmp)
+
+        if self.sym:
+            xmax = torch.maximum(torch.abs(xmin), xmax)
+            tmp = xmin < 0
+            if torch.any(tmp):
+                xmin[tmp] = -xmax[tmp]
+        tmp = (xmin == 0) & (xmax == 0)
+        xmin[tmp] = -1
+        xmax[tmp] = +1
+
+        if self.maxq < 0:
+            self.scale = xmax
+            self.zero = xmin
+        else:
+            self.scale = (xmax - xmin) / self.maxq
+            if self.sym:
+                self.zero = torch.full_like(self.scale, (self.maxq + 1) / 2)
+            else:
+                self.zero = torch.round(-xmin / self.scale)
+
+        if self.mse:
+            best = torch.full([x.shape[0]], float('inf'), device=dev)
+            for i in range(int(self.maxshrink * self.grid)):
+                p = 1 - i / self.grid
+                xmin1 = p * xmin
+                xmax1 = p * xmax
+                scale1 = (xmax1 - xmin1) / self.maxq
+                zero1 = torch.round(-xmin1 / scale1) if not self.sym else self.zero
+                q = quantize(x, scale1.unsqueeze(1), zero1.unsqueeze(1), self.maxq)
+                q -= x
+                q.abs_()
+                q.pow_(self.norm)
+                err = torch.sum(q, 1)
+                tmp = err < best
+                if torch.any(tmp):
+                    best[tmp] = err[tmp]
+                    self.scale[tmp] = scale1[tmp]
+                    self.zero[tmp] = zero1[tmp]
+        if not self.perchannel:
+            if weight:
+                tmp = shape[0]
+            else:
+                tmp = shape[1] if len(shape) != 3 else shape[2]
+            self.scale = self.scale.repeat(tmp)
+            self.zero = self.zero.repeat(tmp)
+
+        if weight:
+            shape = [-1] + [1] * (len(shape) - 1)
+            self.scale = self.scale.reshape(shape)
+            self.zero = self.zero.reshape(shape)
+            return
+        if len(shape) == 4:
+            self.scale = self.scale.reshape((1, -1, 1, 1))
+            self.zero = self.zero.reshape((1, -1, 1, 1))
+        if len(shape) == 3:
+            self.scale = self.scale.reshape((1, 1, -1))
+            self.zero = self.zero.reshape((1, 1, -1))
+        if len(shape) == 2:
+            self.scale = self.scale.unsqueeze(0)
+            self.zero = self.zero.unsqueeze(0)
+
+    def quantize(self, x):
+        if self.ready():
+            return quantize(x, self.scale, self.zero, self.maxq)
+        return x
+
+    def enabled(self):
+        return self.maxq > 0
+
+    def ready(self):
+        return torch.all(self.scale != 0)
+
+
+__all__ = ["Quantizer"]
```

### Comparing `auto_gptq-0.0.5/auto_gptq.egg-info/SOURCES.txt` & `auto_gptq-0.1.0/auto_gptq.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -10,30 +10,34 @@
 auto_gptq/eval_tasks/__init__.py
 auto_gptq/eval_tasks/_base.py
 auto_gptq/eval_tasks/language_modeling_task.py
 auto_gptq/eval_tasks/sequence_classification_task.py
 auto_gptq/eval_tasks/text_summarization_task.py
 auto_gptq/eval_tasks/_utils/__init__.py
 auto_gptq/eval_tasks/_utils/classification_utils.py
-auto_gptq/eval_tasks/_utils/data_utils.py
 auto_gptq/eval_tasks/_utils/generation_utils.py
 auto_gptq/modeling/__init__.py
 auto_gptq/modeling/_base.py
 auto_gptq/modeling/_const.py
 auto_gptq/modeling/_utils.py
 auto_gptq/modeling/auto.py
 auto_gptq/modeling/bloom.py
+auto_gptq/modeling/gpt2.py
 auto_gptq/modeling/gpt_neox.py
 auto_gptq/modeling/gptj.py
 auto_gptq/modeling/llama.py
 auto_gptq/modeling/moss.py
 auto_gptq/modeling/opt.py
 auto_gptq/nn_modules/__init__.py
+auto_gptq/nn_modules/layernorm_triton.py
 auto_gptq/nn_modules/qlinear.py
+auto_gptq/nn_modules/qlinear_old.py
 auto_gptq/nn_modules/qlinear_triton.py
 auto_gptq/nn_modules/triton_utils/__init__.py
 auto_gptq/nn_modules/triton_utils/custom_autotune.py
 auto_gptq/quantization/__init__.py
 auto_gptq/quantization/gptq.py
 auto_gptq/quantization/quantizer.py
+auto_gptq/utils/__init__.py
+auto_gptq/utils/data_utils.py
 quant_cuda/quant_cuda.cpp
 quant_cuda/quant_cuda_kernel.cu
```

