# Comparing `tmp/embetter-0.3.7.tar.gz` & `tmp/embetter-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embetter-0.3.7.tar", last modified: Sat Apr 15 18:28:51 2023, max compression
+gzip compressed data, was "embetter-0.3.8.tar", last modified: Thu May  4 19:47:28 2023, max compression
```

## Comparing `embetter-0.3.7.tar` & `embetter-0.3.8.tar`

### file list

```diff
@@ -1,42 +1,46 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-15 18:28:51.112967 embetter-0.3.7/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7584 2023-04-15 18:28:51.108967 embetter-0.3.7/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6455 2023-04-15 18:17:06.000000 embetter-0.3.7/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-15 18:28:51.100967 embetter-0.3.7/embetter/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      185 2023-04-15 18:17:06.000000 embetter-0.3.7/embetter/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      326 2023-04-15 18:17:06.000000 embetter-0.3.7/embetter/base.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      742 2023-04-15 18:17:06.000000 embetter-0.3.7/embetter/error.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-15 18:28:51.104967 embetter-0.3.7/embetter/external/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      256 2023-04-15 18:17:06.000000 embetter-0.3.7/embetter/external/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2001 2023-04-15 18:17:06.000000 embetter-0.3.7/embetter/external/_cohere.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2356 2023-04-15 18:17:06.000000 embetter-0.3.7/embetter/external/_openai.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-15 18:28:51.104967 embetter-0.3.7/embetter/finetune/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      401 2023-04-15 18:17:06.000000 embetter-0.3.7/embetter/finetune/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5414 2023-04-15 18:17:06.000000 embetter-0.3.7/embetter/finetune/_contrastive.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2640 2023-04-15 18:17:06.000000 embetter-0.3.7/embetter/finetune/_forward.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2408 2023-04-15 18:17:06.000000 embetter-0.3.7/embetter/grab.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-15 18:28:51.104967 embetter-0.3.7/embetter/text/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      730 2023-04-15 18:17:06.000000 embetter-0.3.7/embetter/text/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3794 2023-04-15 18:17:06.000000 embetter-0.3.7/embetter/text/_bpemb.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1579 2023-04-15 18:17:06.000000 embetter-0.3.7/embetter/text/_s2v.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3179 2023-04-15 18:20:18.000000 embetter-0.3.7/embetter/text/_sbert.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2767 2023-04-15 18:17:06.000000 embetter-0.3.7/embetter/text/_spacy.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-15 18:28:51.108967 embetter-0.3.7/embetter/vision/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      361 2023-04-15 18:17:06.000000 embetter-0.3.7/embetter/vision/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1980 2023-04-15 18:17:06.000000 embetter-0.3.7/embetter/vision/_colorhist.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2205 2023-04-15 18:17:06.000000 embetter-0.3.7/embetter/vision/_loader.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2056 2023-04-15 18:17:06.000000 embetter-0.3.7/embetter/vision/_torchvis.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-15 18:28:51.100967 embetter-0.3.7/embetter.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7584 2023-04-15 18:28:50.000000 embetter-0.3.7/embetter.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      784 2023-04-15 18:28:50.000000 embetter-0.3.7/embetter.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-04-15 18:28:50.000000 embetter-0.3.7/embetter.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1004 2023-04-15 18:28:50.000000 embetter-0.3.7/embetter.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       15 2023-04-15 18:28:50.000000 embetter-0.3.7/embetter.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-04-15 18:28:51.112967 embetter-0.3.7/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2595 2023-04-15 18:21:08.000000 embetter-0.3.7/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-15 18:28:51.108967 embetter-0.3.7/tests/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-15 18:17:06.000000 embetter-0.3.7/tests/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      324 2023-04-15 18:17:06.000000 embetter-0.3.7/tests/test_base.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       64 2023-04-15 18:17:06.000000 embetter-0.3.7/tests/test_default.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      910 2023-04-15 18:17:06.000000 embetter-0.3.7/tests/test_docs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2521 2023-04-15 18:17:06.000000 embetter-0.3.7/tests/test_text.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      871 2023-04-15 18:17:06.000000 embetter-0.3.7/tests/test_vision.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-04 19:47:28.895062 embetter-0.3.8/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5190 2023-05-04 19:47:28.895062 embetter-0.3.8/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4061 2023-05-04 19:18:34.000000 embetter-0.3.8/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-04 19:47:28.875062 embetter-0.3.8/embetter/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      185 2023-05-04 19:11:56.000000 embetter-0.3.8/embetter/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      326 2023-05-04 19:11:56.000000 embetter-0.3.8/embetter/base.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      742 2023-05-04 19:11:56.000000 embetter-0.3.8/embetter/error.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-04 19:47:28.879062 embetter-0.3.8/embetter/external/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      256 2023-05-04 19:11:56.000000 embetter-0.3.8/embetter/external/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2001 2023-05-04 19:11:56.000000 embetter-0.3.8/embetter/external/_cohere.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2356 2023-05-04 19:11:56.000000 embetter-0.3.8/embetter/external/_openai.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-04 19:47:28.883062 embetter-0.3.8/embetter/finetune/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      401 2023-05-04 19:11:56.000000 embetter-0.3.8/embetter/finetune/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5414 2023-05-04 19:11:56.000000 embetter-0.3.8/embetter/finetune/_contrastive.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2851 2023-05-04 19:30:13.000000 embetter-0.3.8/embetter/finetune/_forward.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2408 2023-05-04 19:11:56.000000 embetter-0.3.8/embetter/grab.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-04 19:47:28.883062 embetter-0.3.8/embetter/multi/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      185 2023-05-04 19:17:23.000000 embetter-0.3.8/embetter/multi/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1758 2023-05-04 19:30:13.000000 embetter-0.3.8/embetter/multi/_clip.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-04 19:47:28.887062 embetter-0.3.8/embetter/text/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      730 2023-05-04 19:11:56.000000 embetter-0.3.8/embetter/text/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3794 2023-05-04 19:11:56.000000 embetter-0.3.8/embetter/text/_bpemb.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1579 2023-05-04 19:11:56.000000 embetter-0.3.8/embetter/text/_s2v.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3179 2023-05-04 19:11:56.000000 embetter-0.3.8/embetter/text/_sbert.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2767 2023-05-04 19:11:56.000000 embetter-0.3.8/embetter/text/_spacy.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-04 19:47:28.891062 embetter-0.3.8/embetter/vision/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      361 2023-05-04 19:11:56.000000 embetter-0.3.8/embetter/vision/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1980 2023-05-04 19:11:56.000000 embetter-0.3.8/embetter/vision/_colorhist.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2205 2023-05-04 19:11:56.000000 embetter-0.3.8/embetter/vision/_loader.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2056 2023-05-04 19:11:56.000000 embetter-0.3.8/embetter/vision/_torchvis.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-04 19:47:28.879062 embetter-0.3.8/embetter.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5190 2023-05-04 19:47:28.000000 embetter-0.3.8/embetter.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      860 2023-05-04 19:47:28.000000 embetter-0.3.8/embetter.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-05-04 19:47:28.000000 embetter-0.3.8/embetter.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1004 2023-05-04 19:47:28.000000 embetter-0.3.8/embetter.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       15 2023-05-04 19:47:28.000000 embetter-0.3.8/embetter.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-05-04 19:47:28.895062 embetter-0.3.8/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2595 2023-05-04 19:32:08.000000 embetter-0.3.8/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-04 19:47:28.895062 embetter-0.3.8/tests/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-04 19:12:23.000000 embetter-0.3.8/tests/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      324 2023-05-04 19:11:56.000000 embetter-0.3.8/tests/test_base.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       64 2023-05-04 19:11:56.000000 embetter-0.3.8/tests/test_default.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      910 2023-05-04 19:11:56.000000 embetter-0.3.8/tests/test_docs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      452 2023-05-04 19:30:56.000000 embetter-0.3.8/tests/test_finetuners.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2521 2023-05-04 19:11:56.000000 embetter-0.3.8/tests/test_text.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      871 2023-05-04 19:11:56.000000 embetter-0.3.8/tests/test_vision.py
```

### Comparing `embetter-0.3.7/embetter/error.py` & `embetter-0.3.8/embetter/error.py`

 * *Files identical despite different names*

### Comparing `embetter-0.3.7/embetter/external/_cohere.py` & `embetter-0.3.8/embetter/external/_cohere.py`

 * *Files identical despite different names*

### Comparing `embetter-0.3.7/embetter/external/_openai.py` & `embetter-0.3.8/embetter/external/_openai.py`

 * *Files identical despite different names*

### Comparing `embetter-0.3.7/embetter/finetune/_contrastive.py` & `embetter-0.3.8/embetter/finetune/_contrastive.py`

 * *Files identical despite different names*

### Comparing `embetter-0.3.7/embetter/finetune/_forward.py` & `embetter-0.3.8/embetter/finetune/_forward.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 import torch
 import torch.nn as nn
 from sklearn.base import BaseEstimator, TransformerMixin
+from sklearn.preprocessing import LabelEncoder
 
 
 class FeedForwardModel(nn.Module):
     """
     The internal model for the ForwardFinetuner
     """
 
@@ -34,37 +35,40 @@
         learning_rate: The learning rate of the feed forward model
     """
 
     def __init__(self, hidden_dim=50, n_epochs=500, learning_rate=0.01) -> None:
         self.hidden_dim = hidden_dim
         self.n_epochs = n_epochs
         self.learning_rate = learning_rate
+        self.label_enc = LabelEncoder()
 
     def fit(self, X, y):
         """Fits the finetuner."""
         return self.partial_fit(X, y, classes=np.unique(y))
 
     def partial_fit(self, X, y, classes=None):
         """Fits the finetuner using the partial_fit API."""
         if not hasattr(self, "_classes"):
             if classes is None:
                 raise ValueError("`classes` must be provided for partial_fit")
             self._classes = classes
+            self.label_enc.fit(classes)
+            assert (self._classes == self.label_enc.classes_).all()
         # Create a model if it does not exist yet.
         if not hasattr(self, "_model"):
             self._model = FeedForwardModel(
                 X.shape[1], self.hidden_dim, len(self._classes)
             )
             self._optimizer = torch.optim.Adam(
                 self._model.parameters(), lr=self.learning_rate
             )
             self._criterion = nn.CrossEntropyLoss()
 
         torch_X = torch.from_numpy(X).detach().float()
-        torch_y = torch.from_numpy(np.array(y)).detach()
+        torch_y = torch.from_numpy(self.label_enc.transform(y)).detach()
 
         for _ in range(self.n_epochs):
             self._optimizer.zero_grad()
             out = self._model(torch_X)
             loss = self._criterion(out, torch_y)
             loss.backward()
             self._optimizer.step()
```

### Comparing `embetter-0.3.7/embetter/grab.py` & `embetter-0.3.8/embetter/grab.py`

 * *Files identical despite different names*

### Comparing `embetter-0.3.7/embetter/text/__init__.py` & `embetter-0.3.8/embetter/text/__init__.py`

 * *Files identical despite different names*

### Comparing `embetter-0.3.7/embetter/text/_bpemb.py` & `embetter-0.3.8/embetter/text/_bpemb.py`

 * *Files identical despite different names*

### Comparing `embetter-0.3.7/embetter/text/_s2v.py` & `embetter-0.3.8/embetter/text/_s2v.py`

 * *Files identical despite different names*

### Comparing `embetter-0.3.7/embetter/text/_sbert.py` & `embetter-0.3.8/embetter/text/_sbert.py`

 * *Files identical despite different names*

### Comparing `embetter-0.3.7/embetter/text/_spacy.py` & `embetter-0.3.8/embetter/text/_spacy.py`

 * *Files identical despite different names*

### Comparing `embetter-0.3.7/embetter/vision/_colorhist.py` & `embetter-0.3.8/embetter/vision/_colorhist.py`

 * *Files identical despite different names*

### Comparing `embetter-0.3.7/embetter/vision/_loader.py` & `embetter-0.3.8/embetter/vision/_loader.py`

 * *Files identical despite different names*

### Comparing `embetter-0.3.7/embetter/vision/_torchvis.py` & `embetter-0.3.8/embetter/vision/_torchvis.py`

 * *Files identical despite different names*

### Comparing `embetter-0.3.7/embetter.egg-info/SOURCES.txt` & `embetter-0.3.8/embetter.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,22 +11,25 @@
 embetter.egg-info/top_level.txt
 embetter/external/__init__.py
 embetter/external/_cohere.py
 embetter/external/_openai.py
 embetter/finetune/__init__.py
 embetter/finetune/_contrastive.py
 embetter/finetune/_forward.py
+embetter/multi/__init__.py
+embetter/multi/_clip.py
 embetter/text/__init__.py
 embetter/text/_bpemb.py
 embetter/text/_s2v.py
 embetter/text/_sbert.py
 embetter/text/_spacy.py
 embetter/vision/__init__.py
 embetter/vision/_colorhist.py
 embetter/vision/_loader.py
 embetter/vision/_torchvis.py
 tests/__init__.py
 tests/test_base.py
 tests/test_default.py
 tests/test_docs.py
+tests/test_finetuners.py
 tests/test_text.py
 tests/test_vision.py
```

### Comparing `embetter-0.3.7/embetter.egg-info/requires.txt` & `embetter-0.3.8/embetter.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `embetter-0.3.7/setup.py` & `embetter-0.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 all_packages = base_packages + text_packages + vision_packages + openai_packages
 dev_packages = all_packages + docs_packages + test_packages
 
 
 setup(
     name="embetter",
-    version="0.3.7",
+    version="0.3.8",
     author="Vincent D. Warmerdam",
     packages=find_packages(exclude=["notebooks", "docs"]),
     description="Just a bunch of useful embeddings to get started quickly.",
     long_description=pathlib.Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     license_files=("LICENSE"),
     url="https://koaning.github.io/embetter/",
```

### Comparing `embetter-0.3.7/tests/test_docs.py` & `embetter-0.3.8/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `embetter-0.3.7/tests/test_text.py` & `embetter-0.3.8/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `embetter-0.3.7/tests/test_vision.py` & `embetter-0.3.8/tests/test_vision.py`

 * *Files identical despite different names*

