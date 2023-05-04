# Comparing `tmp/probabilistic_word_embeddings-1.2.2.tar.gz` & `tmp/probabilistic_word_embeddings-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "probabilistic_word_embeddings-1.2.2.tar", max compression
+gzip compressed data, was "probabilistic_word_embeddings-1.3.0.tar", max compression
```

## Comparing `probabilistic_word_embeddings-1.2.2.tar` & `probabilistic_word_embeddings-1.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     3406 2023-01-18 15:20:33.692173 probabilistic_word_embeddings-1.2.2/probabilistic_word_embeddings/__init__.py
--rw-r--r--   0        0        0    17101 2022-02-11 12:52:21.792289 probabilistic_word_embeddings-1.2.2/probabilistic_word_embeddings/data/eval/Card-660.tsv
--rw-r--r--   0        0        0      544 2022-02-11 12:52:21.794652 probabilistic_word_embeddings-1.2.2/probabilistic_word_embeddings/data/eval/MC-30.tsv
--rw-r--r--   0        0        0    53593 2022-02-11 12:52:21.797827 probabilistic_word_embeddings-1.2.2/probabilistic_word_embeddings/data/eval/MEN-TR-3k.tsv
--rw-r--r--   0        0        0     7219 2022-02-11 12:52:21.805255 probabilistic_word_embeddings-1.2.2/probabilistic_word_embeddings/data/eval/MTurk-287.tsv
--rw-r--r--   0        0        0    19626 2022-11-07 15:05:53.936879 probabilistic_word_embeddings-1.2.2/probabilistic_word_embeddings/data/eval/MTurk-771.tsv
--rw-r--r--   0        0        0     1209 2022-02-11 12:52:21.810618 probabilistic_word_embeddings-1.2.2/probabilistic_word_embeddings/data/eval/RG-65.tsv
--rw-r--r--   0        0        0    49851 2022-02-11 12:52:21.813786 probabilistic_word_embeddings-1.2.2/probabilistic_word_embeddings/data/eval/RW-STANFORD.tsv
--rw-r--r--   0        0        0    18024 2022-02-11 12:52:21.820517 probabilistic_word_embeddings-1.2.2/probabilistic_word_embeddings/data/eval/SimLex999.tsv
--rw-r--r--   0        0        0    62470 2022-02-11 12:52:21.823693 probabilistic_word_embeddings-1.2.2/probabilistic_word_embeddings/data/eval/SimVerb-3500.tsv
--rw-r--r--   0        0        0     7405 2022-02-11 12:52:21.830909 probabilistic_word_embeddings-1.2.2/probabilistic_word_embeddings/data/eval/WS-353-ALL.tsv
--rw-r--r--   0        0        0     5134 2022-02-11 12:52:21.833629 probabilistic_word_embeddings-1.2.2/probabilistic_word_embeddings/data/eval/WS-353-REL.tsv
--rw-r--r--   0        0        0     4002 2022-02-11 12:52:21.835687 probabilistic_word_embeddings-1.2.2/probabilistic_word_embeddings/data/eval/WS-353-SIM.tsv
--rw-r--r--   0        0        0     2614 2022-02-11 12:52:21.837905 probabilistic_word_embeddings-1.2.2/probabilistic_word_embeddings/data/eval/YP-130.tsv
--rw-r--r--   0        0        0     7424 2023-04-25 13:31:30.609859 probabilistic_word_embeddings-1.2.2/probabilistic_word_embeddings/embeddings.py
--rw-r--r--   0        0        0     9750 2023-04-26 08:35:50.582614 probabilistic_word_embeddings-1.2.2/probabilistic_word_embeddings/estimation.py
--rwxr-xr-x   0        0        0     9947 2023-04-27 11:49:12.185931 probabilistic_word_embeddings-1.2.2/probabilistic_word_embeddings/evaluation.py
--rw-r--r--   0        0        0     3551 2023-04-25 13:31:30.615164 probabilistic_word_embeddings-1.2.2/probabilistic_word_embeddings/models.py
--rw-r--r--   0        0        0     5471 2023-04-25 14:40:29.826311 probabilistic_word_embeddings-1.2.2/probabilistic_word_embeddings/preprocessing.py
--rw-r--r--   0        0        0     3492 2023-04-25 13:31:30.616555 probabilistic_word_embeddings-1.2.2/probabilistic_word_embeddings/utils.py
--rw-r--r--   0        0        0      473 2023-04-27 11:49:37.076821 probabilistic_word_embeddings-1.2.2/pyproject.toml
--rw-r--r--   0        0        0      815 1970-01-01 00:00:00.000000 probabilistic_word_embeddings-1.2.2/setup.py
--rw-r--r--   0        0        0      757 1970-01-01 00:00:00.000000 probabilistic_word_embeddings-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     3406 2023-01-18 15:20:33.692173 probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/__init__.py
+-rw-r--r--   0        0        0    17101 2022-02-11 12:52:21.792289 probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/Card-660.tsv
+-rw-r--r--   0        0        0      544 2022-02-11 12:52:21.794652 probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/MC-30.tsv
+-rw-r--r--   0        0        0    53593 2022-02-11 12:52:21.797827 probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/MEN-TR-3k.tsv
+-rw-r--r--   0        0        0     7219 2022-02-11 12:52:21.805255 probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/MTurk-287.tsv
+-rw-r--r--   0        0        0    19626 2022-11-07 15:05:53.936879 probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/MTurk-771.tsv
+-rw-r--r--   0        0        0     1209 2022-02-11 12:52:21.810618 probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/RG-65.tsv
+-rw-r--r--   0        0        0    49851 2022-02-11 12:52:21.813786 probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/RW-STANFORD.tsv
+-rw-r--r--   0        0        0    18024 2022-02-11 12:52:21.820517 probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/SimLex999.tsv
+-rw-r--r--   0        0        0    62470 2022-02-11 12:52:21.823693 probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/SimVerb-3500.tsv
+-rw-r--r--   0        0        0     7405 2022-02-11 12:52:21.830909 probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/WS-353-ALL.tsv
+-rw-r--r--   0        0        0     5134 2022-02-11 12:52:21.833629 probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/WS-353-REL.tsv
+-rw-r--r--   0        0        0     4002 2022-02-11 12:52:21.835687 probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/WS-353-SIM.tsv
+-rw-r--r--   0        0        0     2614 2022-02-11 12:52:21.837905 probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/YP-130.tsv
+-rw-r--r--   0        0        0     7424 2023-04-25 13:31:30.609859 probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/embeddings.py
+-rw-r--r--   0        0        0    11330 2023-05-04 09:46:06.402140 probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/estimation.py
+-rwxr-xr-x   0        0        0    10097 2023-04-28 07:46:05.201078 probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/evaluation.py
+-rw-r--r--   0        0        0     3551 2023-04-25 13:31:30.615164 probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/models.py
+-rw-r--r--   0        0        0     5699 2023-04-28 08:50:42.813909 probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/preprocessing.py
+-rw-r--r--   0        0        0     2411 2023-04-28 07:51:27.253198 probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/utils.py
+-rw-r--r--   0        0        0      473 2023-05-04 10:13:10.463505 probabilistic_word_embeddings-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      815 1970-01-01 00:00:00.000000 probabilistic_word_embeddings-1.3.0/setup.py
+-rw-r--r--   0        0        0      757 1970-01-01 00:00:00.000000 probabilistic_word_embeddings-1.3.0/PKG-INFO
```

### Comparing `probabilistic_word_embeddings-1.2.2/probabilistic_word_embeddings/__init__.py` & `probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/__init__.py`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.2.2/probabilistic_word_embeddings/data/eval/Card-660.tsv` & `probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/Card-660.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.2.2/probabilistic_word_embeddings/data/eval/MC-30.tsv` & `probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/MC-30.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.2.2/probabilistic_word_embeddings/data/eval/MEN-TR-3k.tsv` & `probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/MEN-TR-3k.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.2.2/probabilistic_word_embeddings/data/eval/MTurk-287.tsv` & `probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/MTurk-287.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.2.2/probabilistic_word_embeddings/data/eval/MTurk-771.tsv` & `probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/MTurk-771.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.2.2/probabilistic_word_embeddings/data/eval/RG-65.tsv` & `probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/RG-65.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.2.2/probabilistic_word_embeddings/data/eval/RW-STANFORD.tsv` & `probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/RW-STANFORD.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.2.2/probabilistic_word_embeddings/data/eval/SimLex999.tsv` & `probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/SimLex999.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.2.2/probabilistic_word_embeddings/data/eval/SimVerb-3500.tsv` & `probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/SimVerb-3500.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.2.2/probabilistic_word_embeddings/data/eval/WS-353-ALL.tsv` & `probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/WS-353-ALL.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.2.2/probabilistic_word_embeddings/data/eval/WS-353-REL.tsv` & `probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/WS-353-REL.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.2.2/probabilistic_word_embeddings/data/eval/WS-353-SIM.tsv` & `probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/WS-353-SIM.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.2.2/probabilistic_word_embeddings/data/eval/YP-130.tsv` & `probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/YP-130.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.2.2/probabilistic_word_embeddings/embeddings.py` & `probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/embeddings.py`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.2.2/probabilistic_word_embeddings/estimation.py` & `probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/estimation.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,14 +23,15 @@
         data: Data as a list of python strings.
         model (str): Word embedding model, either 'sgns' or 'cbow'.
         ws (int): SGNS or CBOW window size
         ns (int): SGNS or CBOW number of negative samples
         batch_size (int): Batch size in the training process 
         epochs (int): The number of passes over the data.
         evaluate (bool): Whether to run word similarity evaluation during training on the standard English evaluation data sets
+        vocab_freqs (dict): The frequencies of the word used for negative sampling. If not provided, the word frequencies are calculated from 'data'.
         valid_data: Data as a list of python strings.
         early_stopping (bool): Wheter to only save the best model according to the validation loss. Requires valid_data.
         profile (bool): whether to run the tensorflow profiler during training
         training_loss (bool): whether to print out the training loss during training.
     
     Returns:
         Trained embedding
@@ -132,30 +133,56 @@
                         print(f"Epoch {epoch} mean training loss after {batch_no} batches: {np.mean(epoch_training_loss)}")
 
     if early_stopping and valid_data is not None and best_valid_weights is not None:
         print("Assign the weights corresponding to the best validation loss")
         embedding.theta.assign(best_valid_weights)
     return embedding
 
-def mean_field_vi(embedding, data, model="cbow", ws=5, ns=5, batch_size=25000, epochs=5, evaluate=True, valid_data=None, elbo_history=False):
+def mean_field_vi(embedding, data, model="cbow", ws=5, ns=5, batch_size=25000, epochs=5, init_mean=True, init_std=0.05, evaluate=True, valid_data=None, elbo_history=False):
+    """
+    Perform mean-field variational inference.
+    
+    Args:
+        embedding: Embedding with a suitable vocabulary and log_prob function. Subclass of pwe.Embedding
+        data: Data as a list of python strings.
+        model (str): Word embedding model, either 'sgns' or 'cbow'.
+        ws (int): SGNS or CBOW window size
+        ns (int): SGNS or CBOW number of negative samples
+        batch_size (int): Batch size in the training process 
+        epochs (int): The number of passes over the data.
+        init_mean (bool): Randomize the initial values of the embedding. If False, uses the values provided in the 'embedding' argument.
+        init_std (float / np.array / tf.Tensor): Default value for the standard deviations. Can be a scalar (float) or an array (np.array / tf.Tensor)
+        evaluate (bool): Whether to run word similarity evaluation during training on the standard English evaluation data sets
+        valid_data: Data as a list of python strings.
+        elbo_history (bool): Whether to return the ELBO history as a list
+    
+    Returns:
+        A tuple consisting of the means as a pwe.Embedding and the standard deviations as an np.array
+    """
     if not isinstance(embedding, Embedding):
         warnings.warn("embedding is not a subclass of probabilistic_word_embeddings.Embedding")
     if model not in ["sgns", "cbow"]:
         raise ValueError("model must be 'sgns' or 'cbow'")
 
     if not isinstance(data, tf.Tensor):
         data = tf.constant(data)
 
     optimizer = tf.keras.optimizers.experimental.Adam(learning_rate=0.001)
     e = embedding
     N = len(data)
     batches = N // batch_size
     
-    q_mean = tf.Variable(tf.random.normal(e.theta.shape, dtype=tf.float64)* 0.00001)
-    q_std_log =  tf.Variable(tf.random.normal(e.theta.shape, dtype=tf.float64)* 0.00001 - 3.0)
+    q_mean_init = embedding.theta
+    if init_mean:
+        q_mean_init = tf.random.normal(e.theta.shape, dtype=tf.float64) * 0.00001
+    q_mean = tf.Variable(q_mean_init)
+    if type(init_std) == float:
+        init_std = tf.random.normal(e.theta.shape, dtype=tf.float64)* 0.00001 + tf.cast(tf.math.log(init_std), dtype=tf.float64)
+        print(init_std)
+    q_std_log =  tf.Variable(init_std)
     
     opt_mean_var = optimizer.add_variable_from_reference(q_mean, "q_mean", initial_value=q_mean)
     opt_std_var = optimizer.add_variable_from_reference(q_std_log, "q_std_log", initial_value=q_std_log)
     optimizer.build([opt_mean_var, opt_std_var])
 
     elbo_history = []
     for epoch in range(epochs):
```

### Comparing `probabilistic_word_embeddings-1.2.2/probabilistic_word_embeddings/evaluation.py` & `probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/evaluation.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,19 +120,21 @@
         rows.append([dataset, corr, len(merged_df), p_value])
         #print(f"Rank Correlation {corr}")
 
     return pd.DataFrame(rows, columns=["Dataset", "Rank Correlation", "No. of Observations", "p-value"])
 
 def nearest_neighbors(embedding, words, K=25, epsilon=1e-10):
     """
-    Evaluate embedding performance on word analogy tasks.
+    Get the K nearest neighbors using cosine distance
     
     Args:
         embedding: embedding as pwe.embeddings.Embedding
-        dataset (pd.DataFrame): Dataframe where each row has four words, word1 - word2 + word3 ≈ word4
+        words (list): List of words for which the nearest neighbors are fetched
+        K (int): the number of nearest neighbors per word
+        epsilon (float): the noise injected to the embedding to numerical issues. For most uses, the default value is ok.
     """
     e = copy.deepcopy(embedding)
     noise = tf.random.normal(shape=e.theta.shape, dtype=tf.float64) * epsilon
     e.theta.assign_add(noise)
     words = [wd for wd in words if wd in embedding]
     r = len(words)
     X = embedding[words]
@@ -218,15 +220,15 @@
 
 ###############################
 # BILINGUAL LEXICON INDUCTION #
 ###############################
 
 def bli(pairs, e, precision=[1,5,15], reverse=False):
     """
-    Calculates the Bilingual Lexicon Induction performance of a crosslingual word embedding.
+    Calculate the Bilingual Lexicon Induction performance of a crosslingual word embedding.
     
     Args:
         pairs: list of word pairs
         e: embedding as a pwe.Embedding
         precision: Precision level of the BLI score.
         reverse: Reverse the prediction; target language becomes the source language and vice versa.
     """
```

### Comparing `probabilistic_word_embeddings-1.2.2/probabilistic_word_embeddings/models.py` & `probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/models.py`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.2.2/probabilistic_word_embeddings/preprocessing.py` & `probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/preprocessing.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import numpy as np
 import tensorflow as tf
-from .utils import dict_to_tf, transitive_dict
+from .utils import dict_to_tf
 import progressbar
 
 def filter_rare_words(data, limit=5, keep_words=set()):
     """
     Filter out words that only occur a handful of times
     
     Args:
         data (list): list of strs
+        limit: (int): words with fewer occurences are discarded
+        keep_words (set): set of words that are always included regardless of frequency
     
     Returns:
         data, counts: list of strs and word counts as a dict
     """
     counts = {}
     if isinstance(data[0], list):
         for dataset in progressbar.progressbar(data):
@@ -36,15 +38,16 @@
     Discard words with the probability of 1 - sqrt(10^-5 / freq)
     Initially proposed by Mikolov et al. (2013)
     
     Args:
         data (Union[list, tf.Tensor]): list of strs or tf.Tensor of strings
         counts (dict): word counts in the dataset
         cutoff (float): lowest word frequency for when downsampling is applied
-    
+        chunk_len (int): the number of words that are processed at a time to restrict memory use
+
     Returns:
         list of strs
     """
     if not isinstance(data, tf.Tensor):
         data = tf.constant(data)
 
     print("Discard some instances of the most common words...")
```

### Comparing `probabilistic_word_embeddings-1.2.2/setup.py` & `probabilistic_word_embeddings-1.3.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'progressbar2',
  'scikit-learn',
  'tensorflow-probability>=0.11,<0.12',
  'tensorflow>=2.2,<3.0']
 
 setup_kwargs = {
     'name': 'probabilistic-word-embeddings',
-    'version': '1.2.2',
+    'version': '1.3.0',
     'description': 'Probabilistic Word Embeddings for Python',
     'long_description': 'None',
     'author': 'Your Name',
     'author_email': 'you@example.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `probabilistic_word_embeddings-1.2.2/PKG-INFO` & `probabilistic_word_embeddings-1.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: probabilistic-word-embeddings
-Version: 1.2.2
+Version: 1.3.0
 Summary: Probabilistic Word Embeddings for Python
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

