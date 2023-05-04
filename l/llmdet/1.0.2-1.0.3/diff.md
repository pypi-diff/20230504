# Comparing `tmp/llmdet-1.0.2.tar.gz` & `tmp/llmdet-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmdet-1.0.2.tar", last modified: Wed May  3 12:52:29 2023, max compression
+gzip compressed data, was "llmdet-1.0.3.tar", last modified: Thu May  4 08:44:36 2023, max compression
```

## Comparing `llmdet-1.0.2.tar` & `llmdet-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:52:29.185199 llmdet-1.0.2/
--rw-r--r--   0 root         (0) root         (0)     1093 2023-05-03 11:43:47.000000 llmdet-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3598 2023-05-03 12:52:29.185199 llmdet-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3151 2023-05-03 11:43:47.000000 llmdet-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:52:29.185199 llmdet-1.0.2/llmdet/
--rw-r--r--   0 root         (0) root         (0)     1181 2023-05-03 12:17:07.000000 llmdet-1.0.2/llmdet/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6002 2023-05-03 11:43:48.000000 llmdet-1.0.2/llmdet/arguments.py
--rw-r--r--   0 root         (0) root         (0)     2835 2023-05-03 11:43:48.000000 llmdet-1.0.2/llmdet/classifier.py
--rw-r--r--   0 root         (0) root         (0)     8064 2023-05-03 11:43:48.000000 llmdet-1.0.2/llmdet/detector.py
--rw-r--r--   0 root         (0) root         (0)    25372 2023-05-03 11:43:48.000000 llmdet-1.0.2/llmdet/new_proxy_perplexity.py
--rw-r--r--   0 root         (0) root         (0)    16061 2023-05-03 11:43:48.000000 llmdet-1.0.2/llmdet/run_main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:52:29.185199 llmdet-1.0.2/llmdet.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3598 2023-05-03 12:52:29.000000 llmdet-1.0.2/llmdet.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      304 2023-05-03 12:52:29.000000 llmdet-1.0.2/llmdet.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 12:52:29.000000 llmdet-1.0.2/llmdet.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-05-03 12:52:29.000000 llmdet-1.0.2/llmdet.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-03 12:52:29.000000 llmdet-1.0.2/llmdet.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 12:52:29.185199 llmdet-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      888 2023-05-03 12:52:01.000000 llmdet-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 08:44:36.493380 llmdet-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)     1093 2023-05-03 11:43:47.000000 llmdet-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3598 2023-05-04 08:44:36.493380 llmdet-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3151 2023-05-03 11:43:47.000000 llmdet-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 08:44:36.489380 llmdet-1.0.3/llmdet/
+-rw-r--r--   0 root         (0) root         (0)     1224 2023-05-04 07:59:29.000000 llmdet-1.0.3/llmdet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6002 2023-05-03 11:43:48.000000 llmdet-1.0.3/llmdet/arguments.py
+-rw-r--r--   0 root         (0) root         (0)     2835 2023-05-03 11:43:48.000000 llmdet-1.0.3/llmdet/classifier.py
+-rw-r--r--   0 root         (0) root         (0)     7702 2023-05-04 08:43:28.000000 llmdet-1.0.3/llmdet/detector.py
+-rw-r--r--   0 root         (0) root         (0)    25372 2023-05-03 11:43:48.000000 llmdet-1.0.3/llmdet/new_proxy_perplexity.py
+-rw-r--r--   0 root         (0) root         (0)    16061 2023-05-03 11:43:48.000000 llmdet-1.0.3/llmdet/run_main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 08:44:36.489380 llmdet-1.0.3/llmdet.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3598 2023-05-04 08:44:36.000000 llmdet-1.0.3/llmdet.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      304 2023-05-04 08:44:36.000000 llmdet-1.0.3/llmdet.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 08:44:36.000000 llmdet-1.0.3/llmdet.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-05-04 08:44:36.000000 llmdet-1.0.3/llmdet.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-04 08:44:36.000000 llmdet-1.0.3/llmdet.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-04 08:44:36.493380 llmdet-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      888 2023-05-04 08:43:56.000000 llmdet-1.0.3/setup.py
```

### Comparing `llmdet-1.0.2/LICENSE` & `llmdet-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `llmdet-1.0.2/PKG-INFO` & `llmdet-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmdet
-Version: 1.0.2
+Version: 1.0.3
 Summary: LLMDet：A Large Language Models Detection Tool
 Home-page: https://github.com/cansee5/LLMDet
 Author: Kangxi Wu, Liang Pang
 Author-email: wukx0901@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `llmdet-1.0.2/README.md` & `llmdet-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `llmdet-1.0.2/llmdet/__init__.py` & `llmdet-1.0.3/llmdet/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,8 +15,10 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 __version__ = "1.0.2"
-from detector import detect
+
+from .detector import load_probability
+from .detector import detect
```

### Comparing `llmdet-1.0.2/llmdet/arguments.py` & `llmdet-1.0.3/llmdet/arguments.py`

 * *Files identical despite different names*

### Comparing `llmdet-1.0.2/llmdet/classifier.py` & `llmdet-1.0.3/llmdet/classifier.py`

 * *Files identical despite different names*

### Comparing `llmdet-1.0.2/llmdet/detector.py` & `llmdet-1.0.3/llmdet/detector.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,73 +4,76 @@
 import math
 import json
 from transformers import AutoTokenizer
 from unilm import UniLMTokenizer
 from lightgbm import Booster
 
 
+def load_probability():
+    dm = datasets.DownloadManager()
+    files = dm.download_and_extract('https://huggingface.co/datasets/wukx/n-grams_sample_probability/resolve/main/new_n_grams.zip')
+    n_grams = np.load(f'{files}/new_n_grams.npz' , allow_pickle=True)
+    global gpt_n_grams_probability, opt_n_grams_probability, unilm_n_grams_probability
+    gpt_n_grams_probability = n_grams["gpt"]
+    opt_n_grams_probability = n_grams["opt"]
+    unilm_n_grams_probability = n_grams["unilm"]
+
 # Calculate the perplexity of text.
 def perplexity(text_set_token_ids, n_grams_probability, vocab_size):
-    # Load n-grams probability
-    probability_2_grams_keys = n_grams_probability['sample_probs'][0]["keys"]
-    probability_2_grams_values = n_grams_probability['sample_probs'][0]["values"]
-    probability_3_grams_keys = n_grams_probability['sample_probs'][1]["keys"]
-    probability_3_grams_values = n_grams_probability['sample_probs'][1]["values"]
-    probability_4_grams_keys = n_grams_probability['sample_probs'][2]["keys"]
-    probability_4_grams_values = n_grams_probability['sample_probs'][2]["values"]
 
     # Calculate proxy perplexity value for test text set
     test_perplexity = []
 
     for k in tqdm(range(len(text_set_token_ids))):
         text_token_ids = text_set_token_ids[k]
         ppl = 0
         number_3_grams = 0
         number_4_grams = 0
         number_2_grams = 0
         for i in range(2, len(text_token_ids) - 1):
 
             # Calculate the perplexity with 4-grams samples probability
-            if tuple([text_token_ids[i - j] for j in range(2, -1, -1)]) in probability_4_grams_keys.keys():
-                if text_token_ids[i + 1] in probability_4_grams_keys[tuple([text_token_ids[i - j] for j in range(2, -1, -1)])]:
-                    if probability_4_grams_values[tuple([text_token_ids[i - j] for j in range(2, -1, -1)])][probability_4_grams_keys[tuple([text_token_ids[i - j] for j in range(2, -1, -1)])].tolist().index(text_token_ids[i + 1])] > 0:
-                        ppl = ppl + math.log2(probability_4_grams_values[tuple([text_token_ids[i - j] for j in range(2, -1, -1)])][probability_4_grams_keys[tuple([text_token_ids[i - j] for j in range(2, -1, -1)])].tolist().index(text_token_ids[i + 1])])
+            if tuple([text_token_ids[i - j] for j in range(2, -1, -1)]) in n_grams_probability[4].keys():
+                if text_token_ids[i + 1] in n_grams_probability[4][tuple([text_token_ids[i - j] for j in range(2, -1, -1)])]:
+                    if n_grams_probability[5][tuple([text_token_ids[i - j] for j in range(2, -1, -1)])][n_grams_probability[4][tuple([text_token_ids[i - j] for j in range(2, -1, -1)])].tolist().index(text_token_ids[i + 1])] > 0:
+                        ppl = ppl + math.log2(n_grams_probability[5][tuple([text_token_ids[i - j] for j in range(2, -1, -1)])][n_grams_probability[4][tuple([text_token_ids[i - j] for j in range(2, -1, -1)])].tolist().index(text_token_ids[i + 1])])
                 else:
-                    top_k = len(probability_4_grams_keys[tuple([text_token_ids[i - j] for j in range(2, -1, -1)])])
-                    sum_probs = sum(probability_4_grams_values[tuple([text_token_ids[i - j] for j in range(2, -1, -1)])])
+                    top_k = len(n_grams_probability[4][tuple([text_token_ids[i - j] for j in range(2, -1, -1)])])
+                    sum_probs = sum(n_grams_probability[5][tuple([text_token_ids[i - j] for j in range(2, -1, -1)])])
                     if (1 - sum_probs) > 0:
                         ppl = ppl + math.log2((1 - sum_probs) / (vocab_size - top_k))
                 number_4_grams = number_4_grams + 1
 
             # Calculate the perplexity with 3-grams samples probability
-            elif tuple([text_token_ids[i - 1], text_token_ids[i]]) in probability_3_grams_keys.keys():
-                if text_token_ids[i + 1] in probability_3_grams_keys[tuple([text_token_ids[i - 1], text_token_ids[i]])]:
-                    if probability_3_grams_values[tuple([text_token_ids[i - 1], text_token_ids[i]])][probability_3_grams_keys[tuple([text_token_ids[i - 1], text_token_ids[i]])].tolist().index(text_token_ids[i + 1])] > 0:
-                        ppl = ppl + math.log2(probability_3_grams_values[tuple([text_token_ids[i - 1], text_token_ids[i]])][probability_3_grams_keys[tuple([text_token_ids[i - 1], text_token_ids[i]])].tolist().index(text_token_ids[i + 1])])
+            elif tuple([text_token_ids[i - 1], text_token_ids[i]]) in n_grams_probability[2].keys():
+                if text_token_ids[i + 1] in n_grams_probability[2][tuple([text_token_ids[i - 1], text_token_ids[i]])]:
+                    if n_grams_probability[3][tuple([text_token_ids[i - 1], text_token_ids[i]])][n_grams_probability[2][tuple([text_token_ids[i - 1], text_token_ids[i]])].tolist().index(text_token_ids[i + 1])] > 0:
+                        ppl = ppl + math.log2(
+                            n_grams_probability[3][tuple([text_token_ids[i - 1], text_token_ids[i]])][n_grams_probability[2][tuple([text_token_ids[i - 1], text_token_ids[i]])].tolist().index(text_token_ids[i + 1])])
                 else:
-                    top_k = len(probability_3_grams_keys[tuple([text_token_ids[i - 1], text_token_ids[i]])])
-                    sum_probs = sum(probability_3_grams_values[tuple([text_token_ids[i - 1], text_token_ids[i]])])
+                    top_k = len(n_grams_probability[2][tuple([text_token_ids[i - 1], text_token_ids[i]])])
+                    sum_probs = sum(n_grams_probability[3][tuple([text_token_ids[i - 1], text_token_ids[i]])])
                     if (1 - sum_probs) > 0:
                         ppl = ppl + math.log2((1 - sum_probs) / (vocab_size - top_k))
                 number_3_grams = number_3_grams + 1
 
             # Calculate the perplexity with 2-grams samples probability
-            elif tuple([text_token_ids[i]]) in probability_2_grams_keys.keys():
-                if text_token_ids[i + 1] in probability_2_grams_keys[tuple([text_token_ids[i]])]:
-                    if probability_2_grams_values[tuple([text_token_ids[i]])][probability_2_grams_keys[tuple([text_token_ids[i]])].tolist().index(text_token_ids[i + 1])] > 0:
-                        ppl = ppl + math.log2(probability_2_grams_values[tuple([text_token_ids[i]])][probability_2_grams_keys[tuple([text_token_ids[i]])].tolist().index(text_token_ids[i + 1])])
+            elif tuple([text_token_ids[i]]) in n_grams_probability[0].keys():
+                if text_token_ids[i + 1] in n_grams_probability[0][tuple([text_token_ids[i]])]:
+                    if n_grams_probability[1][tuple([text_token_ids[i]])][n_grams_probability[0][tuple([text_token_ids[i]])].tolist().index(text_token_ids[i + 1])] > 0:
+                        ppl = ppl + math.log2(n_grams_probability[1][tuple([text_token_ids[i]])][n_grams_probability[0][tuple([text_token_ids[i]])].tolist().index(text_token_ids[i + 1])])
                 else:
-                    top_k = len(probability_2_grams_keys[tuple([text_token_ids[i]])])
-                    sum_probs = sum(probability_2_grams_values[tuple([text_token_ids[i]])])
+                    top_k = len(n_grams_probability[0][tuple([text_token_ids[i]])])
+                    sum_probs = sum(n_grams_probability[1][tuple([text_token_ids[i]])])
                     if (1 - sum_probs) > 0:
                         ppl = ppl + math.log2((1 - sum_probs) / (vocab_size - top_k))
                 number_2_grams = number_2_grams + 1
 
         perplexity = round(ppl / (number_2_grams + number_3_grams + number_4_grams + 1), 2)
-        test_perplexity.append(perplexity)
+        test_perplexity.append(-perplexity)
 
     return test_perplexity
 
 # Detect function
 def detect(text):
     # Determine whether the input is a single text or a collection of text.
     if isinstance(text, str):
@@ -85,51 +88,50 @@
             )
     else:
         raise ValueError(
             "The type of `text` which you input is not a string or list. "
             "Please enter the correct data type for `text`."
         )
     dm = datasets.DownloadManager()
-    files = dm.download_and_extract('https://huggingface.co/datasets/wukx/n-grams_sample_probability/resolve/main/n_grams.zip')
-        
-    gpt_tokenizer = AutoTokenizer.from_pretrained("gpt2")
-    gpt_vocab_size = 50265
-    text_gpt_token_ids = []
-    for text in test_text:
-        gpt_text_tokenize = gpt_tokenizer.tokenize(text, truncation=True)
-        text_gpt_token_ids.append(gpt_tokenizer.convert_tokens_to_ids(gpt_text_tokenize))
-    gpt_sample_probability_file = f'{files}/n_grams/gpt.npz'
-    # Load GPT model's n-grams probability data
-    gpt_n_grams_probability = np.load(gpt_sample_probability_file, allow_pickle=True)
-    gpt_perplexity = perplexity(text_gpt_token_ids, gpt_n_grams_probability, gpt_vocab_size)
-
-    opt_tokenizer = AutoTokenizer.from_pretrained("facebook/opt-1.3b")
-    opt_vocab_size = 50257
-    text_opt_token_ids = []
-    for text in test_text:
-        opt_text_tokenize = opt_tokenizer.tokenize(text)
-        text_opt_token_ids.append(opt_tokenizer.convert_tokens_to_ids(opt_text_tokenize))
-    opt_sample_probability_file = f'{files}/n_grams/opt.npz'
-    # Load OPT model's n-grams probability data
-    opt_n_grams_probability = np.load(opt_sample_probability_file, allow_pickle=True)
-    opt_perplexity = perplexity(text_opt_token_ids, opt_n_grams_probability, opt_vocab_size)
-
-    unilm_tokenizer = UniLMTokenizer.from_pretrained("microsoft/unilm-base-cased")
-    unilm_vocab_size = 28996
-    text_unilm_token_ids = []
-    for text in test_text:
-        unilm_text_tokenize = unilm_tokenizer.tokenize(text)
-        text_unilm_token_ids.append(unilm_tokenizer.convert_tokens_to_ids(unilm_text_tokenize))
-    unilm_sample_probability_file = f'{files}/n_grams/unilm.npz'
-    # Load UniLM model's n-grams probability data
-    unilm_n_grams_probability = np.load(unilm_sample_probability_file, allow_pickle=True)
-    unilm_perplexity = perplexity(text_unilm_token_ids, unilm_n_grams_probability, unilm_vocab_size)
+    # files = dm.download_and_extract('https://huggingface.co/datasets/wukx/n-grams_sample_probability/resolve/main/n_grams.zip')
+
+    model_information = [{"model_name": "gpt2", "vocab_size": 50265, "model_probability": "gpt_n_grams_probability"},
+                         {"model_name": "facebook/opt-1.3b", "vocab_size": 50257, "model_probability": "opt_n_grams_probability"},
+                         {"model_name": "microsoft/unilm-base-cased", "vocab_size": 28996, "model_probability": "unilm_n_grams_probability"}]
+
+    # Calculate the proxy perplexity
+    perplexity_result = []
+    for model in model_information:
+        if any([(model_type in model["model_name"]) for model_type in ["unilm"]]):
+            tokenizer = UniLMTokenizer.from_pretrained(model["model_name"])
+        else:
+            tokenizer = AutoTokenizer.from_pretrained(model["model_name"])
+
+        text_token_ids = []
+        for text in test_text:
+            if any([(model_type in model["model_name"]) for model_type in ["gpt"]]):
+                text_tokenize = tokenizer.tokenize(text, truncation=True)
+            else:
+                text_tokenize = tokenizer.tokenize(text)
+            text_token_ids.append(tokenizer.convert_tokens_to_ids(text_tokenize))
+
+
+        if model["model_probability"] in globals():
+            perplexity_result.append(perplexity(text_token_ids, globals()[model["model_probability"]], model["vocab_size"]))
+        else:
+            raise ValueError(
+                "The {} does not exist, please load n-grams probability!".format(model["model_probability"])
+            )
+
+    # The input features of classiffier
+    features = np.stack([perplexity_result[i] for i in range(len(perplexity_result))], axis=1)
+    print(features)
 
     # Load classiffier model
-    model_files = dm.download_and_extract('https://huggingface.co/datasets/wukx/n-grams_sample_probability/resolve/main/LightGBM_model.zip')
+    model_files = dm.download_and_extract(
+        'https://huggingface.co/datasets/wukx/n-grams_sample_probability/resolve/main/LightGBM_model.zip')
     model = Booster(model_file=f'{model_files}/LightGBM_model.txt')
-    test_result = []
-    for gpt, opt, unilm in zip(gpt_perplexity, opt_perplexity, unilm_perplexity):
-        y_pred = model.predict([[gpt, opt, unilm]])
-        result = {"Human_write": y_pred[0][0], "GPT-2": y_pred[0][1], "OPT": y_pred[0][2], "UniLM": y_pred[0][3]}
-        test_result.append(result)
+    y_pred = model.predict(features)
+    label = ["Human_write", "GPT-2", "OPT", "UniLM"]
+    test_result = [{label[i]: y_pred[j][i] for i in range(len(label))} for j in range(len(y_pred))]
+
     return test_result
```

### Comparing `llmdet-1.0.2/llmdet/new_proxy_perplexity.py` & `llmdet-1.0.3/llmdet/new_proxy_perplexity.py`

 * *Files identical despite different names*

### Comparing `llmdet-1.0.2/llmdet/run_main.py` & `llmdet-1.0.3/llmdet/run_main.py`

 * *Files identical despite different names*

### Comparing `llmdet-1.0.2/llmdet.egg-info/PKG-INFO` & `llmdet-1.0.3/llmdet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmdet
-Version: 1.0.2
+Version: 1.0.3
 Summary: LLMDet：A Large Language Models Detection Tool
 Home-page: https://github.com/cansee5/LLMDet
 Author: Kangxi Wu, Liang Pang
 Author-email: wukx0901@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `llmdet-1.0.2/setup.py` & `llmdet-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="llmdet",
-    version="1.0.2",
+    version="1.0.3",
     author="Kangxi Wu, Liang Pang",
     author_email="wukx0901@gmail.com",
     description="LLMDet：A Large Language Models Detection Tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cansee5/LLMDet",
     packages=setuptools.find_packages(),
```

