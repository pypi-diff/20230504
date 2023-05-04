# Comparing `tmp/xfact-lm-0.2.44.tar.gz` & `tmp/xfact-lm-0.2.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xfact-lm-0.2.44.tar", last modified: Wed Mar 15 01:56:13 2023, max compression
+gzip compressed data, was "xfact-lm-0.2.50.tar", last modified: Thu May  4 02:45:57 2023, max compression
```

## Comparing `xfact-lm-0.2.44.tar` & `xfact-lm-0.2.50.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 01:56:13.392433 xfact-lm-0.2.44/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-15 01:55:15.000000 xfact-lm-0.2.44/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-15 01:56:13.392433 xfact-lm-0.2.44/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-03-15 01:55:15.000000 xfact-lm-0.2.44/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-15 01:55:15.000000 xfact-lm-0.2.44/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-15 01:56:13.392433 xfact-lm-0.2.44/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-03-15 01:55:15.000000 xfact-lm-0.2.44/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 01:56:13.388433 xfact-lm-0.2.44/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 01:56:13.388433 xfact-lm-0.2.44/src/xfact_lm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-15 01:56:13.000000 xfact-lm-0.2.44/src/xfact_lm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-03-15 01:56:13.000000 xfact-lm-0.2.44/src/xfact_lm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 01:56:13.000000 xfact-lm-0.2.44/src/xfact_lm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-15 01:56:13.000000 xfact-lm-0.2.44/src/xfact_lm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-15 01:56:13.000000 xfact-lm-0.2.44/src/xfact_lm.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 01:56:13.388433 xfact-lm-0.2.44/src/xfact_lslms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 01:55:15.000000 xfact-lm-0.2.44/src/xfact_lslms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 01:56:13.388433 xfact-lm-0.2.44/src/xfact_lslms/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 01:55:15.000000 xfact-lm-0.2.44/src/xfact_lslms/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-03-15 01:55:15.000000 xfact-lm-0.2.44/src/xfact_lslms/client/lslms_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-03-15 01:55:15.000000 xfact-lm-0.2.44/src/xfact_lslms/log_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 01:56:13.388433 xfact-lm-0.2.44/src/xfact_lslms/service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 01:55:15.000000 xfact-lm-0.2.44/src/xfact_lslms/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-03-15 01:55:15.000000 xfact-lm-0.2.44/src/xfact_lslms/service/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-03-15 01:55:15.000000 xfact-lm-0.2.44/src/xfact_lslms/service/amq_communications.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-03-15 01:55:15.000000 xfact-lm-0.2.44/src/xfact_lslms/service/llama_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-03-15 01:55:15.000000 xfact-lm-0.2.44/src/xfact_lslms/service/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:45:57.166168 xfact-lm-0.2.50/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-04 02:44:21.000000 xfact-lm-0.2.50/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-04 02:45:57.166168 xfact-lm-0.2.50/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-04 02:44:21.000000 xfact-lm-0.2.50/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-04 02:44:21.000000 xfact-lm-0.2.50/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 02:45:57.166168 xfact-lm-0.2.50/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-04 02:44:21.000000 xfact-lm-0.2.50/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:45:57.162167 xfact-lm-0.2.50/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:45:57.162167 xfact-lm-0.2.50/src/xfact_lm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-04 02:45:57.000000 xfact-lm-0.2.50/src/xfact_lm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-04 02:45:57.000000 xfact-lm-0.2.50/src/xfact_lm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 02:45:57.000000 xfact-lm-0.2.50/src/xfact_lm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-04 02:45:57.000000 xfact-lm-0.2.50/src/xfact_lm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 02:45:57.000000 xfact-lm-0.2.50/src/xfact_lm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:45:57.162167 xfact-lm-0.2.50/src/xfact_lslms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 02:44:21.000000 xfact-lm-0.2.50/src/xfact_lslms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:45:57.162167 xfact-lm-0.2.50/src/xfact_lslms/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 02:44:21.000000 xfact-lm-0.2.50/src/xfact_lslms/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-05-04 02:44:21.000000 xfact-lm-0.2.50/src/xfact_lslms/client/lslms_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-04 02:44:21.000000 xfact-lm-0.2.50/src/xfact_lslms/log_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:45:57.166168 xfact-lm-0.2.50/src/xfact_lslms/service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 02:44:21.000000 xfact-lm-0.2.50/src/xfact_lslms/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-04 02:44:21.000000 xfact-lm-0.2.50/src/xfact_lslms/service/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-04 02:44:21.000000 xfact-lm-0.2.50/src/xfact_lslms/service/amq_communications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-05-04 02:44:21.000000 xfact-lm-0.2.50/src/xfact_lslms/service/models.py
```

### Comparing `xfact-lm-0.2.44/setup.py` & `xfact-lm-0.2.50/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 install = [req for req in reqs if not req.startswith("git+git://")]
 depends = [req.replace("git+git://", "git+http://") for req in reqs if req.startswith("git+git://")]
 
 
 setup(
     name='xfact-lm',
-    version='0.2.44',
+    version='0.2.50',
     author='James Thorne',
     author_email='james@jamesthorne.com',
     description='xfact language model',
     long_description="readme",
     python_requires='>=3.8',
     packages=["xfact_lslms",
               "xfact_lslms.client",
```

### Comparing `xfact-lm-0.2.44/src/xfact_lslms/client/lslms_client.py` & `xfact-lm-0.2.50/src/xfact_lslms/client/lslms_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -49,75 +49,43 @@
         self.queue = model_name
 
     def on_response(self, ch, method, props, body):
         if self.corr_id == props.correlation_id:
             self.response = body
 
     def call(self, n, tokenizer_kwargs=None, generate_kwargs=None, timeout=50):
+        return self.generate(n, tokenizer_kwargs, generate_kwargs, timeout)
+        
+    def generate(self, n, tokenizer_kwargs=None, generate_kwargs=None, timeout=50):
         self.response = None
         self.corr_id = str(uuid.uuid4())
         self.channel.basic_publish(
             exchange='',
             routing_key=self.queue,
             properties=pika.BasicProperties(
                 reply_to=self.callback_queue,
                 correlation_id=self.corr_id,
                 expiration=str(timeout)+'000',
             ),
             body=json.dumps({
                 "batch": n,
                 "tokenizer_kwargs": tokenizer_kwargs or {},
-                "generate_kwargs": generate_kwargs or {}
+                "generate_kwargs": generate_kwargs or {'max_length': 500}
             }).encode())
 
         self.connection.process_data_events(time_limit=timeout)
 
         if self.response:
             resp =  json.loads(self.response.decode('utf-8'))
             if 'error' in resp:
-                print(resp['stack_trace'])
-            else:
-                return resp
-        else:
-            print('Error: Make sure the model is running (http://status.xfact.net/models). If the model is running, adjust the timeout or reduce the max_length parameter')
-            return None
-        
-    def generate(self, n, tokenizer_kwargs=None, generate_kwargs=None, timeout=50):
-        self.response = None
-        self.corr_id = str(uuid.uuid4())
-
-        message = json.dumps({'func': 'generate', 
-                              'body' : {
-                                    "batch": n,
-                                    "tokenizer_kwargs": tokenizer_kwargs or {},
-                                    "generate_kwargs": generate_kwargs or {}
-                                    }
-        }).encode()
-
-        self.channel.basic_publish(
-            exchange='',
-            routing_key=self.queue,
-            properties=pika.BasicProperties(
-                reply_to=self.callback_queue,
-                correlation_id=self.corr_id,
-                expiration=str(timeout)+'000',
-            ),
-            body=message)
-
-        self.connection.process_data_events(time_limit=timeout)
-
-        if self.response:
-            resp =  json.loads(self.response.decode('utf-8'))
-            if 'error' in resp:
-                print(resp['stack_trace'])
+                raise Exception('Exception occur on the server \n' + resp['stack_trace'])
             else:
                 return resp
         else:
-            print('Error: Make sure the model is running (http://status.xfact.net/models). If the model is running, adjust the timeout or reduce the max_length parameter')
-            return None
+            raise Exception('Error: Make sure the model is running (http://status.xfact.net/models). If the model is running, adjust the timeout or reduce the max_length parameter')
         
     def forward(self, inputs, timeout=50):
         self.response = None
         self.corr_id = str(uuid.uuid4())
 
         message = {'func': 'forward', 'body' : {
             "inputs": inputs
```

### Comparing `xfact-lm-0.2.44/src/xfact_lslms/log_helper.py` & `xfact-lm-0.2.50/src/xfact_lslms/log_helper.py`

 * *Files identical despite different names*

### Comparing `xfact-lm-0.2.44/src/xfact_lslms/service/amq_communications.py` & `xfact-lm-0.2.50/src/xfact_lslms/service/amq_communications.py`

 * *Files identical despite different names*

### Comparing `xfact-lm-0.2.44/src/xfact_lslms/service/models.py` & `xfact-lm-0.2.50/src/xfact_lslms/service/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,33 +6,19 @@
 # Huggingface Imports
 from transformers import AutoConfig, AutoTokenizer, AutoModelForSeq2SeqLM, AutoModelForCausalLM, AutoModelForMaskedLM
 import math
 from accelerate import init_empty_weights, infer_auto_device_map
 
 logger = logging.getLogger(__name__)
 
-class ThreadWithReturnValue(Thread):
-    
-    def __init__(self, group=None, target=None, name=None,
-                 args=(), kwargs={}, Verbose=None):
-        Thread.__init__(self, group, target, name, args, kwargs)
-        self._return = None
-
-    def run(self):
-        if self._target is not None:
-            self._return = self._target(*self._args,
-                                                **self._kwargs)
-    def join(self, *args):
-        Thread.join(self, *args)
-        return self._return
-
-def get_device_map(model_name, dtype, mem_gpu0=10):
+def get_device_map(args, dtype):
+    mem_gpu0 = args.gpu0
     # Making a empty shell for Model
     with init_empty_weights():
-        config = AutoConfig.from_pretrained(model_name)
+        config = AutoConfig.from_pretrained(args.model)
         try:
             model = AutoModelForSeq2SeqLM.from_config(config).to(dtype)
         except:
             try:
                 model = AutoModelForCausalLM.from_config(config).to(dtype)
             except:
                 model = AutoModelForMaskedLM.from_config(config).to(dtype)
@@ -43,48 +29,48 @@
     mem = mem_params
     for i in ['B', 'KB', 'MB', 'GB', 'TB', 'PB']:
             if mem < 1024.0:
                 break
             mem /= 1024.0
     logger.info(f'Memory Used by model: {mem:.{3}f} {i}')
 
-    if num_device <= 1 or mem_params < 5*1024*1024*1024:
+    if num_device <= 1 or mem_params < 5*1024*1024*1024 or args.auto_map:
         return 'auto'
 
     # Genetrating Custom Device Map
     mem_gpuN = math.ceil((mem_params/(1024*1024*1024) - mem_gpu0) / (num_device-1))+1
     mem_map=[str(mem_gpu0)+'GiB', str(mem_gpuN)+'GiB']
 
     d = {0: mem_map[0]}
     for i in range(1, num_device):
         d[i] = mem_map[1]
     logger.info(f'Memory Map for the model: {d}')
 
     device_map = infer_auto_device_map(
-        model, max_memory=d, dtype=dtype, no_split_module_classes=["BloomBlock", "OPTDecoderLayer", "LLaMADecoderLayer", "T5LayerFF"]
+        model, max_memory=d, dtype=dtype, no_split_module_classes=["BloomBlock", "OPTDecoderLayer", "LLaMADecoderLayer", "T5LayerFF", "T5LayerCrossAttention"]
     )
     logger.info(f'Device Map for the model: \n{device_map}')
     # Checking Device Map validity
     for i in d:
         if torch.cuda.get_device_properties(i).total_memory <= d[i]:
             raise Exception('Model cannot fit in given GPU Configuration; CUDA: Out of Memory')
     del model
     return device_map
 
 class LanguageModelAgent():
     def __init__(self, args):
-        self.past_key_values = None
+
         if args.bf16:
             self.dtype = torch.bfloat16
         elif args.fp16:
             self.dtype = torch.float16
         else:
             self.dtype = torch.float32
         if args.multi_gpu:
-            device_map = get_device_map(args.model, self.dtype)
+            device_map = get_device_map(args, self.dtype)
         else:
             device_map = None
 
         model_args = {
             'pretrained_model_name_or_path': args.model,
             'cache_dir': args.cache_dir if args.cache_dir and os.path.exists(args.cache_dir) else None,
             'torch_dtype': self.dtype,
@@ -95,99 +81,83 @@
             'pretrained_model_name_or_path': args.model,
             'cache_dir': args.cache_dir if args.cache_dir and os.path.exists(args.cache_dir) else None,
         }
 
         logger.info(f'Loading model: {args.model}')
         self.tokenizer = AutoTokenizer.from_pretrained(**tokenizer_args, use_fast="/opt" not in args.model)
 
+        self.autoregressive = False
         try:
             self.model = AutoModelForSeq2SeqLM.from_pretrained(**model_args)
         except:
             try:
                 self.model = AutoModelForCausalLM.from_pretrained(**model_args)
+                self.autoregressive = True
             except:
                 self.model = AutoModelForMaskedLM.from_pretrained(**model_args)
 
         logger.info(f'Model Loaded: {args.model}')
         
         self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
         if not args.multi_gpu:
             self.model.to(self.device)
 
         self.model.eval()
         self.bechmark()
 
-    ## Need some optimization
-    def multi_threading(self, batch, tokenizer_kwargs={}, generate_kwargs={}, num_threads=2):
-        outs = {"input_text": [], "decoded_text": []}
-        threads = []
-        if len(batch) / num_threads < 2:
-            raise Exception('Send an appropriate number for Batch and num_threads')
-        
-        n = math.ceil(len(batch) / num_threads)
-
-        for i in range(0, len(batch), n):
-            t = ThreadWithReturnValue(target=self.infer, args=(batch[i: i+n], tokenizer_kwargs, generate_kwargs))
-            # add the thread to the list
-            threads.append(t)
-            # start the thread
-            t.start()
-
-        for t in threads:
-            outs['input_text'].extend(t.join()['input_text'])
-            outs['decoded_text'].extend(t.join()['decoded_text'])
-
-        return outs
-
     def bechmark(self, max_length=100, num_iter=10, batch_size=16):
         text = "Explain how babies are born? How to calm them down and why do they cry so much?"
+        batch = [text]*batch_size
         generate_kwargs={"max_length": max_length}
 
         logger.info(f'Starting Benchmark')
         start = time.time()
         for _ in range(num_iter):
             responce = self.infer(batch=text, generate_kwargs=generate_kwargs, tokenizer_kwargs={})
-        length = len(responce['decoded_text'][0].split(' '))
         end = time.time()
+        length = len(responce['decoded_text'][0].split(' '))
         logger.info(f'Benchmark results: Using single prompt, the model achieves generation speed of {num_iter/(end-start):.{3}f} it/s with generation length of {length}')
         
-        text = ["Explain how babies are born? How to calm them down and why do they cry so much?"]*batch_size
         start = time.time()
         for _ in range(num_iter):
-            responce = self.infer(batch=text, generate_kwargs=generate_kwargs, tokenizer_kwargs={})
-        length = len(responce['decoded_text'][0].split(' '))
+            responce = self.infer(batch=batch, generate_kwargs=generate_kwargs, tokenizer_kwargs={})
         end = time.time()
+        length = len(responce['decoded_text'][0].split(' '))
         logger.info(f'Benchmark reults: Using batch size of {batch_size}, the model achieves generation speed of {num_iter/(end-start):.{3}f} it/s with generation length of {length}')
 
     @torch.inference_mode()
     def infer(self, batch, tokenizer_kwargs, generate_kwargs):
         input_ids = self.tokenizer(batch, return_tensors="pt", **tokenizer_kwargs).to(self.device)
-        outs = self.model.generate(**input_ids, **generate_kwargs).cpu()
+        outs = self.model.generate(input_ids=input_ids['input_ids'], attention_mask=input_ids['attention_mask'], **generate_kwargs).cpu()
         predictions = self.tokenizer.batch_decode(outs, skip_special_tokens=True)
 
+        if self.autoregressive and type(batch) == str:
+            predictions[0] = predictions[0][len(batch):]
+        elif self.autoregressive:
+            predictions = [prediction[len(batch[i]):] for i, prediction in enumerate(predictions)]
+
         logger.debug(f"Predicting on {batch}")
         logger.debug(f"Predicted {predictions}")
 
         return {
             "input_text": batch,
             "decoded_text": predictions
         }
     
     @torch.inference_mode()
     def forward(self, inputs):
-        
         for key in inputs:
             inputs[key] = torch.tensor(inputs[key], dtype=torch.int, device=self.device)
 
-        outs = self.model(**inputs, past_key_values=self.past_key_values)
+        outs = self.model(**inputs)
 
         logger.debug(f"Input {inputs}")
         logger.debug(f"Output {outs}")
 
         responce = {}
         for key in outs:
             if key != 'past_key_values':
                 responce[key] = outs[key].tolist()
             else:
-                self.past_key_values = outs[key]
+                past_key_values = outs[key]
             
         return responce
```

