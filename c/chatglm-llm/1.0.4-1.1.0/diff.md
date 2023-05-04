# Comparing `tmp/chatglm-llm-1.0.4.tar.gz` & `tmp/chatglm-llm-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatglm-llm-1.0.4.tar", last modified: Thu May  4 02:16:17 2023, max compression
+gzip compressed data, was "chatglm-llm-1.1.0.tar", last modified: Thu May  4 07:24:49 2023, max compression
```

## Comparing `chatglm-llm-1.0.4.tar` & `chatglm-llm-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 02:16:17.377296 chatglm-llm-1.0.4/
--rw-r--r--   0 root         (0) root         (0)      164 2023-05-04 02:16:17.377296 chatglm-llm-1.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1887 2023-05-04 01:30:19.000000 chatglm-llm-1.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 02:16:17.377296 chatglm-llm-1.0.4/chatglm_llm.egg-info/
--rw-r--r--   0 root         (0) root         (0)      164 2023-05-04 02:16:17.000000 chatglm-llm-1.0.4/chatglm_llm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      351 2023-05-04 02:16:17.000000 chatglm-llm-1.0.4/chatglm_llm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 02:16:17.000000 chatglm-llm-1.0.4/chatglm_llm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-05-04 02:16:17.000000 chatglm-llm-1.0.4/chatglm_llm.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 01:30:33.000000 chatglm-llm-1.0.4/chatglm_llm.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      175 2023-05-04 02:16:17.000000 chatglm-llm-1.0.4/chatglm_llm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-05-04 02:16:17.000000 chatglm-llm-1.0.4/chatglm_llm.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 02:16:17.377296 chatglm-llm-1.0.4/chatglm_src/
--rw-r--r--   0 root         (0) root         (0)       27 2023-05-04 01:30:19.000000 chatglm-llm-1.0.4/chatglm_src/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3963 2023-05-04 01:30:19.000000 chatglm-llm-1.0.4/chatglm_src/callbacks.py
--rw-r--r--   0 root         (0) root         (0)      443 2023-05-04 01:30:19.000000 chatglm-llm-1.0.4/chatglm_src/cmd.py
--rw-r--r--   0 root         (0) root         (0)    17117 2023-05-04 02:15:45.000000 chatglm-llm-1.0.4/chatglm_src/llm.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-04 02:16:17.377296 chatglm-llm-1.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      802 2023-05-04 02:15:53.000000 chatglm-llm-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:24:49.858605 chatglm-llm-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      164 2023-05-04 07:24:49.858605 chatglm-llm-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1887 2023-05-04 01:59:08.000000 chatglm-llm-1.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:24:49.858605 chatglm-llm-1.1.0/chatglm_llm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      164 2023-05-04 07:24:49.000000 chatglm-llm-1.1.0/chatglm_llm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      351 2023-05-04 07:24:49.000000 chatglm-llm-1.1.0/chatglm_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 07:24:49.000000 chatglm-llm-1.1.0/chatglm_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-05-04 07:24:49.000000 chatglm-llm-1.1.0/chatglm_llm.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 01:59:18.000000 chatglm-llm-1.1.0/chatglm_llm.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      175 2023-05-04 07:24:49.000000 chatglm-llm-1.1.0/chatglm_llm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-04 07:24:49.000000 chatglm-llm-1.1.0/chatglm_llm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:24:49.858605 chatglm-llm-1.1.0/chatglm_src/
+-rw-r--r--   0 root         (0) root         (0)       27 2023-05-04 01:59:08.000000 chatglm-llm-1.1.0/chatglm_src/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3963 2023-05-04 01:59:08.000000 chatglm-llm-1.1.0/chatglm_src/callbacks.py
+-rw-r--r--   0 root         (0) root         (0)      443 2023-05-04 01:59:08.000000 chatglm-llm-1.1.0/chatglm_src/cmd.py
+-rw-r--r--   0 root         (0) root         (0)    20505 2023-05-04 07:22:00.000000 chatglm-llm-1.1.0/chatglm_src/llm.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-04 07:24:49.858605 chatglm-llm-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      802 2023-05-04 07:24:41.000000 chatglm-llm-1.1.0/setup.py
```

### Comparing `chatglm-llm-1.0.4/README.md` & `chatglm-llm-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.0.4/chatglm_src/callbacks.py` & `chatglm-llm-1.1.0/chatglm_src/callbacks.py`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.0.4/chatglm_src/llm.py` & `chatglm-llm-1.1.0/chatglm_src/llm.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,30 +9,98 @@
 from termcolor import colored
 import torch, gc
 from transformers import AutoTokenizer, AutoModel
 import datetime
 from hashlib import md5
 import time
 from .callbacks import AsyncWebsocketHandler, AsyncWebSocksetCallbackManager
-
+from accelerate import load_checkpoint_and_dispatch
 
 from aiowebsocket.converses import AioWebSocket
 from websocket import create_connection
 import websockets
 from websockets.server import serve
 ## LLM for chatglm
 # only load from local's path
 # default path is in ~/.cache/chatglm, if not exists, will download from huggingface'url :https://huggingface.co/THUDM/chatglm-6b
 # 
 """Common utility functions for working with LLM APIs."""
 import re
-from typing import List
+from typing import List, Dict, Any, Optional, Union
 TODAY = datetime.datetime.now()
 PASSWORD = "ADSFADSGADSHDAFHDSG@#%!@#T%DSAGADSHDFAGSY@#%@!#^%@#$Y^#$TYDGVDFSGDS!@$!@$" + f"{TODAY.year}-{TODAY.month}"
+# from transformers import AutoModel, AutoTokenizer
+
+os.environ["CUDA_VISIBLE_DEVICES"] = "0,1"
+def load_model_on_gpus(checkpoint_path, num_gpus=2):
+    # 总共占用13GB显存,28层transformer每层0.39GB左右
+    # 第一层 word_embeddings和最后一层 lm_head 层各占用1.2GB左右
+    num_trans_layers = 28
+    vram_per_layer = 0.39
+    average = 13/num_gpus
+    used = 1.2
+    device_map = {'transformer.word_embeddings': 0,
+                  'transformer.final_layernorm': num_gpus-1, 'lm_head': num_gpus-1}
+    gpu_target = 0
+    for i in range(num_trans_layers):
+        if used > average-vram_per_layer/2 and gpu_target < num_gpus:
+            gpu_target += 1
+            used = 0
+        else:
+            used += vram_per_layer
+        device_map['transformer.layers.%d' % i] = gpu_target
 
+    model = AutoModel.from_pretrained(
+        checkpoint_path, trust_remote_code=True)
+    model = model.eval()
+    model = load_checkpoint_and_dispatch(
+        model, checkpoint_path, device_map=device_map, offload_folder="offload", offload_state_dict=True).half()
+    return model
+
+def auto_configure_device_map(num_gpus: int) -> Dict[str, int]:
+    # transformer.word_embeddings 占用1层
+    # transformer.final_layernorm 和 lm_head 占用1层
+    # transformer.layers 占用 28 层
+    # 总共30层分配到num_gpus张卡上
+    num_trans_layers = 28
+    per_gpu_layers = 30 / num_gpus
+
+    # bugfix: 在linux中调用torch.embedding传入的weight,input不在同一device上,导致RuntimeError
+    # windows下 model.device 会被设置成 transformer.word_embeddings.device
+    # linux下 model.device 会被设置成 lm_head.device
+    # 在调用chat或者stream_chat时,input_ids会被放到model.device上
+    # 如果transformer.word_embeddings.device和model.device不同,则会导致RuntimeError
+    # 因此这里将transformer.word_embeddings,transformer.final_layernorm,lm_head都放到第一张卡上
+    device_map = {'transformer.word_embeddings': 0,
+                  'transformer.final_layernorm': 0, 'lm_head': 0}
+
+    used = 2
+    gpu_target = 0
+    for i in range(num_trans_layers):
+        if used >= per_gpu_layers:
+            gpu_target += 1
+            used = 0
+        assert gpu_target < num_gpus
+        device_map[f'transformer.layers.{i}'] = gpu_target
+        used += 1
+
+    return device_map
+
+
+def load_model_on_gpus_old(checkpoint_path, num_gpus: int = 2,device_map = None, **kwargs):
+    if num_gpus < 2 and device_map is None:
+        model = AutoModel.from_pretrained(checkpoint_path, trust_remote_code=True, **kwargs).half().cuda()
+    else:
+        from accelerate import dispatch_model
+        model = AutoModel.from_pretrained(checkpoint_path, trust_remote_code=True, **kwargs).half()
+        if device_map is None:
+            device_map = auto_configure_device_map(num_gpus)
+        model = dispatch_model(model, device_map=device_map)
+
+    return model
 
 def enforce_stop_tokens(text: str, stop: List[str]) -> str:
     """Cut off the text as soon as any stop words occur."""
     return re.split("|".join(stop), text)[0]
 
 def auto_gc():
     if torch.cuda.is_available():
@@ -105,28 +173,32 @@
         mo = cls(*args, **kargs)
         if "cpu" in kargs and kargs["cpu"]:
             mo.cpu = True
         if model_path is not None:
             mo.model_path = pathlib.Path(model_path)
         # load from local
         if mo.model_path.exists() and mo.remote_host is None:
-            mo.model = AutoModel.from_pretrained(mo.model_path, trust_remote_code=True)
+            if torch.cuda.device_count() > 0:
+                print(colored("[GPU]","green"),":",torch.cuda.device_count(), "GPUs" )
+                mo.model = load_model_on_gpus_old(mo.model_path, num_gpus=torch.cuda.device_count())
+            else:
+                mo.model = AutoModel.from_pretrained(mo.model_path, trust_remote_code=True, device_map="auto")
             mo.tokenizer = AutoTokenizer.from_pretrained(mo.model_path, trust_remote_code=True)
         else:
             # load from huggingface
             # use os.system to call git lfs download model
             # then load from local
             # TODO: use git lfs to download model
             pass
         if mo.remote_host is not None:
             return mo
         if mo.cpu:
             mo.model = mo.model.float()
-        else:
-            mo.model = mo.model.half().cuda()
+        # else:
+        #     mo.model = mo.model.half().cuda()
         mo.model = mo.model.eval()
         return mo
     
     def set_history(self, hist:List[str]):
         self.history = hist
     
     
@@ -298,29 +370,32 @@
 
 class WebsocketWrap:
     def __init__(self, llm, websocket):
         self.websocket = websocket
         self.llm = llm
     
     async def __call__(self, prompt=None, history=None):
-        assert prompt is not None 
-        assert isinstance(prompt, str)
-        llm = self.llm
-        current_completion = ""
-        if history is not None and isinstance(history, list):
-            llm.history = history
-        for response, history in llm.model.stream_chat(llm.tokenizer, prompt, llm.history, max_length=llm.max_token, top_p=llm.top_p,
-                                               temperature=llm.temperature):
-            delta = response[len(current_completion) :]
-            current_completion = response
-            data = { "new":delta,"response": response, "history": history,"query": prompt}
+        try:
+            assert prompt is not None 
+            assert isinstance(prompt, str)
+            llm = self.llm
+            current_completion = ""
+            if history is not None and isinstance(history, list):
+                llm.history = history
+            for response, history in llm.model.stream_chat(llm.tokenizer, prompt, llm.history, max_length=llm.max_token, top_p=llm.top_p,
+                                                temperature=llm.temperature):
+                delta = response[len(current_completion) :]
+                current_completion = response
+                data = { "new":delta,"response": response, "history": history,"query": prompt}
+                await self.websocket.send(json.dumps(data))
+            data = { "new":delta,"response": response, "history": history,"query": prompt, "stop":True}
+            
             await self.websocket.send(json.dumps(data))
-        data = { "new":delta,"response": response, "history": history,"query": prompt, "stop":True}
-        await self.websocket.send(json.dumps(data))
-
+        finally:
+            auto_gc()
 
 
 
 class AsyncServer:
     __users = {}
     _callbacks = {"hello": lambda x: colored("[hello]","green") + time.asctime()}
     llm = None
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `chatglm-llm-1.0.4/setup.py` & `chatglm-llm-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 
 setup(name='chatglm-llm',
-    version='1.0.4',
+    version='1.1.0',
     description='chatglm llm',
     url='https://github.com/xxx',
     author='auth',
     author_email='xxx@gmail.com',
     license='MIT',
     include_package_data=True,
     zip_safe=False,
```

