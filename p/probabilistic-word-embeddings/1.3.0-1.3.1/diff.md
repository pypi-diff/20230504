# Comparing `tmp/probabilistic_word_embeddings-1.3.0.tar.gz` & `tmp/probabilistic_word_embeddings-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "probabilistic_word_embeddings-1.3.0.tar", max compression
+gzip compressed data, was "probabilistic_word_embeddings-1.3.1.tar", max compression
```

## Comparing `probabilistic_word_embeddings-1.3.0.tar` & `probabilistic_word_embeddings-1.3.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     3406 2023-01-18 15:20:33.692173 probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/__init__.py
--rw-r--r--   0        0        0    17101 2022-02-11 12:52:21.792289 probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/Card-660.tsv
--rw-r--r--   0        0        0      544 2022-02-11 12:52:21.794652 probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/MC-30.tsv
--rw-r--r--   0        0        0    53593 2022-02-11 12:52:21.797827 probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/MEN-TR-3k.tsv
--rw-r--r--   0        0        0     7219 2022-02-11 12:52:21.805255 probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/MTurk-287.tsv
--rw-r--r--   0        0        0    19626 2022-11-07 15:05:53.936879 probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/MTurk-771.tsv
--rw-r--r--   0        0        0     1209 2022-02-11 12:52:21.810618 probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/RG-65.tsv
--rw-r--r--   0        0        0    49851 2022-02-11 12:52:21.813786 probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/RW-STANFORD.tsv
--rw-r--r--   0        0        0    18024 2022-02-11 12:52:21.820517 probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/SimLex999.tsv
--rw-r--r--   0        0        0    62470 2022-02-11 12:52:21.823693 probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/SimVerb-3500.tsv
--rw-r--r--   0        0        0     7405 2022-02-11 12:52:21.830909 probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/WS-353-ALL.tsv
--rw-r--r--   0        0        0     5134 2022-02-11 12:52:21.833629 probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/WS-353-REL.tsv
--rw-r--r--   0        0        0     4002 2022-02-11 12:52:21.835687 probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/WS-353-SIM.tsv
--rw-r--r--   0        0        0     2614 2022-02-11 12:52:21.837905 probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/YP-130.tsv
--rw-r--r--   0        0        0     7424 2023-04-25 13:31:30.609859 probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/embeddings.py
--rw-r--r--   0        0        0    11330 2023-05-04 09:46:06.402140 probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/estimation.py
--rwxr-xr-x   0        0        0    10097 2023-04-28 07:46:05.201078 probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/evaluation.py
--rw-r--r--   0        0        0     3551 2023-04-25 13:31:30.615164 probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/models.py
--rw-r--r--   0        0        0     5699 2023-04-28 08:50:42.813909 probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/preprocessing.py
--rw-r--r--   0        0        0     2411 2023-04-28 07:51:27.253198 probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/utils.py
--rw-r--r--   0        0        0      473 2023-05-04 10:13:10.463505 probabilistic_word_embeddings-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      815 1970-01-01 00:00:00.000000 probabilistic_word_embeddings-1.3.0/setup.py
--rw-r--r--   0        0        0      757 1970-01-01 00:00:00.000000 probabilistic_word_embeddings-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     3406 2023-01-18 15:20:33.692173 probabilistic_word_embeddings-1.3.1/probabilistic_word_embeddings/__init__.py
+-rw-r--r--   0        0        0    17101 2022-02-11 12:52:21.792289 probabilistic_word_embeddings-1.3.1/probabilistic_word_embeddings/data/eval/Card-660.tsv
+-rw-r--r--   0        0        0      544 2022-02-11 12:52:21.794652 probabilistic_word_embeddings-1.3.1/probabilistic_word_embeddings/data/eval/MC-30.tsv
+-rw-r--r--   0        0        0    53593 2022-02-11 12:52:21.797827 probabilistic_word_embeddings-1.3.1/probabilistic_word_embeddings/data/eval/MEN-TR-3k.tsv
+-rw-r--r--   0        0        0     7219 2022-02-11 12:52:21.805255 probabilistic_word_embeddings-1.3.1/probabilistic_word_embeddings/data/eval/MTurk-287.tsv
+-rw-r--r--   0        0        0    19626 2022-11-07 15:05:53.936879 probabilistic_word_embeddings-1.3.1/probabilistic_word_embeddings/data/eval/MTurk-771.tsv
+-rw-r--r--   0        0        0     1209 2022-02-11 12:52:21.810618 probabilistic_word_embeddings-1.3.1/probabilistic_word_embeddings/data/eval/RG-65.tsv
+-rw-r--r--   0        0        0    49851 2022-02-11 12:52:21.813786 probabilistic_word_embeddings-1.3.1/probabilistic_word_embeddings/data/eval/RW-STANFORD.tsv
+-rw-r--r--   0        0        0    18024 2022-02-11 12:52:21.820517 probabilistic_word_embeddings-1.3.1/probabilistic_word_embeddings/data/eval/SimLex999.tsv
+-rw-r--r--   0        0        0    62470 2022-02-11 12:52:21.823693 probabilistic_word_embeddings-1.3.1/probabilistic_word_embeddings/data/eval/SimVerb-3500.tsv
+-rw-r--r--   0        0        0     7405 2022-02-11 12:52:21.830909 probabilistic_word_embeddings-1.3.1/probabilistic_word_embeddings/data/eval/WS-353-ALL.tsv
+-rw-r--r--   0        0        0     5134 2022-02-11 12:52:21.833629 probabilistic_word_embeddings-1.3.1/probabilistic_word_embeddings/data/eval/WS-353-REL.tsv
+-rw-r--r--   0        0        0     4002 2022-02-11 12:52:21.835687 probabilistic_word_embeddings-1.3.1/probabilistic_word_embeddings/data/eval/WS-353-SIM.tsv
+-rw-r--r--   0        0        0     2614 2022-02-11 12:52:21.837905 probabilistic_word_embeddings-1.3.1/probabilistic_word_embeddings/data/eval/YP-130.tsv
+-rw-r--r--   0        0        0     7424 2023-04-25 13:31:30.609859 probabilistic_word_embeddings-1.3.1/probabilistic_word_embeddings/embeddings.py
+-rw-r--r--   0        0        0    11330 2023-05-04 09:46:06.402140 probabilistic_word_embeddings-1.3.1/probabilistic_word_embeddings/estimation.py
+-rwxr-xr-x   0        0        0    10286 2023-05-04 12:56:38.958397 probabilistic_word_embeddings-1.3.1/probabilistic_word_embeddings/evaluation.py
+-rw-r--r--   0        0        0     3551 2023-04-25 13:31:30.615164 probabilistic_word_embeddings-1.3.1/probabilistic_word_embeddings/models.py
+-rw-r--r--   0        0        0     5699 2023-04-28 08:50:42.813909 probabilistic_word_embeddings-1.3.1/probabilistic_word_embeddings/preprocessing.py
+-rw-r--r--   0        0        0     2411 2023-04-28 07:51:27.253198 probabilistic_word_embeddings-1.3.1/probabilistic_word_embeddings/utils.py
+-rw-r--r--   0        0        0      473 2023-05-04 12:59:19.196812 probabilistic_word_embeddings-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0      815 1970-01-01 00:00:00.000000 probabilistic_word_embeddings-1.3.1/setup.py
+-rw-r--r--   0        0        0      757 1970-01-01 00:00:00.000000 probabilistic_word_embeddings-1.3.1/PKG-INFO
```

### Comparing `probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/__init__.py` & `probabilistic_word_embeddings-1.3.1/probabilistic_word_embeddings/__init__.py`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/Card-660.tsv` & `probabilistic_word_embeddings-1.3.1/probabilistic_word_embeddings/data/eval/Card-660.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/MC-30.tsv` & `probabilistic_word_embeddings-1.3.1/probabilistic_word_embeddings/data/eval/MC-30.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/MEN-TR-3k.tsv` & `probabilistic_word_embeddings-1.3.1/probabilistic_word_embeddings/data/eval/MEN-TR-3k.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/MTurk-287.tsv` & `probabilistic_word_embeddings-1.3.1/probabilistic_word_embeddings/data/eval/MTurk-287.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/MTurk-771.tsv` & `probabilistic_word_embeddings-1.3.1/probabilistic_word_embeddings/data/eval/MTurk-771.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/RG-65.tsv` & `probabilistic_word_embeddings-1.3.1/probabilistic_word_embeddings/data/eval/RG-65.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/RW-STANFORD.tsv` & `probabilistic_word_embeddings-1.3.1/probabilistic_word_embeddings/data/eval/RW-STANFORD.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/SimLex999.tsv` & `probabilistic_word_embeddings-1.3.1/probabilistic_word_embeddings/data/eval/SimLex999.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/SimVerb-3500.tsv` & `probabilistic_word_embeddings-1.3.1/probabilistic_word_embeddings/data/eval/SimVerb-3500.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/WS-353-ALL.tsv` & `probabilistic_word_embeddings-1.3.1/probabilistic_word_embeddings/data/eval/WS-353-ALL.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/WS-353-REL.tsv` & `probabilistic_word_embeddings-1.3.1/probabilistic_word_embeddings/data/eval/WS-353-REL.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/WS-353-SIM.tsv` & `probabilistic_word_embeddings-1.3.1/probabilistic_word_embeddings/data/eval/WS-353-SIM.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/data/eval/YP-130.tsv` & `probabilistic_word_embeddings-1.3.1/probabilistic_word_embeddings/data/eval/YP-130.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/embeddings.py` & `probabilistic_word_embeddings-1.3.1/probabilistic_word_embeddings/embeddings.py`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/estimation.py` & `probabilistic_word_embeddings-1.3.1/probabilistic_word_embeddings/estimation.py`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/evaluation.py` & `probabilistic_word_embeddings-1.3.1/probabilistic_word_embeddings/evaluation.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,18 +48,24 @@
     valid_batches = len(data) // batch_size
 
     valid_ll = tf.constant([], dtype=tf.float64)
     for batch in progressbar.progressbar(range(valid_batches)):
         start_ix = batch_size * batch
         if model == "sgns":
             i,j,x  = generate_sgns_batch(data, ws=ws, ns=ns, batch=batch_size, start_ix=start_ix)
-            valid_ll = tf.concat([valid_ll, sgns_likelihood(embedding, i, j, x=x)], axis=0)
+            valid_ll_batch = sgns_likelihood(embedding, i, j, x=x)
         elif model == "cbow":
             i,j,x  = generate_cbow_batch(data, ws=ws, ns=ns, batch=batch_size, start_ix=start_ix)
-            valid_ll = tf.concat([valid_ll, cbow_likelihood(embedding, i, j, x=x)], axis=0)
+            valid_ll_batch = cbow_likelihood(embedding, i, j, x=x)
+
+        # Reduce memory footprint by calculating the mean on the fly
+        if reduce_mean:
+            valid_ll_batch = tf.expand_dims(tf.reduce_mean(valid_ll_batch), 0)
+
+        valid_ll = tf.concat([valid_ll, valid_ll_batch], axis=0)
 
     if reduce_mean:
         return tf.reduce_mean(valid_ll)
     else:
         return valid_ll
 
 ###################
```

### Comparing `probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/models.py` & `probabilistic_word_embeddings-1.3.1/probabilistic_word_embeddings/models.py`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/preprocessing.py` & `probabilistic_word_embeddings-1.3.1/probabilistic_word_embeddings/preprocessing.py`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.3.0/probabilistic_word_embeddings/utils.py` & `probabilistic_word_embeddings-1.3.1/probabilistic_word_embeddings/utils.py`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.3.0/setup.py` & `probabilistic_word_embeddings-1.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'progressbar2',
  'scikit-learn',
  'tensorflow-probability>=0.11,<0.12',
  'tensorflow>=2.2,<3.0']
 
 setup_kwargs = {
     'name': 'probabilistic-word-embeddings',
-    'version': '1.3.0',
+    'version': '1.3.1',
     'description': 'Probabilistic Word Embeddings for Python',
     'long_description': 'None',
     'author': 'Your Name',
     'author_email': 'you@example.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `probabilistic_word_embeddings-1.3.0/PKG-INFO` & `probabilistic_word_embeddings-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: probabilistic-word-embeddings
-Version: 1.3.0
+Version: 1.3.1
 Summary: Probabilistic Word Embeddings for Python
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

