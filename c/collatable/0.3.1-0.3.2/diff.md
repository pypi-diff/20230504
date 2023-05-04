# Comparing `tmp/collatable-0.3.1.tar.gz` & `tmp/collatable-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collatable-0.3.1.tar", max compression
+gzip compressed data, was "collatable-0.3.2.tar", max compression
```

## Comparing `collatable-0.3.1.tar` & `collatable-0.3.2.tar`

### file list

```diff
@@ -1,28 +1,27 @@
--rw-r--r--   0        0        0     1064 2023-02-06 01:00:34.001098 collatable-0.3.1/LICENSE
--rw-r--r--   0        0        0     6401 2023-02-06 01:00:34.001098 collatable-0.3.1/README.md
--rw-r--r--   0        0        0      690 2023-02-06 01:00:34.001098 collatable-0.3.1/collatable/__init__.py
--rw-r--r--   0        0        0      552 2023-02-06 01:00:34.001098 collatable-0.3.1/collatable/collator.py
--rw-r--r--   0        0        0      214 2023-02-06 01:00:34.001098 collatable-0.3.1/collatable/extras/__init__.py
--rw-r--r--   0        0        0     2062 2023-02-06 01:00:34.001098 collatable-0.3.1/collatable/extras/dataloader.py
--rw-r--r--   0        0        0     6694 2023-02-06 01:00:34.001098 collatable-0.3.1/collatable/extras/dataset.py
--rw-r--r--   0        0        0     6065 2023-02-06 01:00:34.001098 collatable-0.3.1/collatable/extras/indexer.py
--rw-r--r--   0        0        0      828 2023-02-06 01:00:34.001098 collatable-0.3.1/collatable/fields/__init__.py
--rw-r--r--   0        0        0     3108 2023-02-06 01:00:34.001098 collatable-0.3.1/collatable/fields/adjacency_field.py
--rw-r--r--   0        0        0     2150 2023-02-06 01:00:34.001098 collatable-0.3.1/collatable/fields/field.py
--rw-r--r--   0        0        0      795 2023-02-06 01:00:34.001098 collatable-0.3.1/collatable/fields/index_field.py
--rw-r--r--   0        0        0     1668 2023-02-06 01:00:34.001098 collatable-0.3.1/collatable/fields/label_field.py
--rw-r--r--   0        0        0     1308 2023-02-06 01:00:34.001098 collatable-0.3.1/collatable/fields/list_field.py
--rw-r--r--   0        0        0      735 2023-02-06 01:00:34.001098 collatable-0.3.1/collatable/fields/metadata_field.py
--rw-r--r--   0        0        0      839 2023-02-06 01:00:34.001098 collatable-0.3.1/collatable/fields/scalar_field.py
--rw-r--r--   0        0        0      266 2023-02-06 01:00:34.001098 collatable-0.3.1/collatable/fields/sequence_field.py
--rw-r--r--   0        0        0     2385 2023-02-06 01:00:34.001098 collatable-0.3.1/collatable/fields/sequence_label_field.py
--rw-r--r--   0        0        0     1497 2023-02-06 01:00:34.001098 collatable-0.3.1/collatable/fields/span_field.py
--rw-r--r--   0        0        0     1006 2023-02-06 01:00:34.001098 collatable-0.3.1/collatable/fields/tensor_field.py
--rw-r--r--   0        0        0     2203 2023-02-06 01:00:34.001098 collatable-0.3.1/collatable/fields/text_field.py
--rw-r--r--   0        0        0      384 2023-02-06 01:00:34.001098 collatable-0.3.1/collatable/instance.py
--rw-r--r--   0        0        0        0 2023-02-06 01:00:34.001098 collatable-0.3.1/collatable/py.typed
--rw-r--r--   0        0        0      423 2023-02-06 01:00:34.001098 collatable-0.3.1/collatable/typing.py
--rw-r--r--   0        0        0     1180 2023-02-06 01:00:34.001098 collatable-0.3.1/collatable/util.py
--rw-r--r--   0        0        0     1500 2023-02-06 01:00:34.005099 collatable-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     7344 1970-01-01 00:00:00.000000 collatable-0.3.1/setup.py
--rw-r--r--   0        0        0     7032 1970-01-01 00:00:00.000000 collatable-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-04 09:04:19.601967 collatable-0.3.2/LICENSE
+-rw-r--r--   0        0        0     6401 2023-05-04 09:04:19.601967 collatable-0.3.2/README.md
+-rw-r--r--   0        0        0      690 2023-05-04 09:04:19.601967 collatable-0.3.2/collatable/__init__.py
+-rw-r--r--   0        0        0      552 2023-05-04 09:04:19.601967 collatable-0.3.2/collatable/collator.py
+-rw-r--r--   0        0        0      214 2023-05-04 09:04:19.601967 collatable-0.3.2/collatable/extras/__init__.py
+-rw-r--r--   0        0        0     2062 2023-05-04 09:04:19.601967 collatable-0.3.2/collatable/extras/dataloader.py
+-rw-r--r--   0        0        0     6694 2023-05-04 09:04:19.601967 collatable-0.3.2/collatable/extras/dataset.py
+-rw-r--r--   0        0        0     6065 2023-05-04 09:04:19.601967 collatable-0.3.2/collatable/extras/indexer.py
+-rw-r--r--   0        0        0      828 2023-05-04 09:04:19.601967 collatable-0.3.2/collatable/fields/__init__.py
+-rw-r--r--   0        0        0     3108 2023-05-04 09:04:19.601967 collatable-0.3.2/collatable/fields/adjacency_field.py
+-rw-r--r--   0        0        0     2150 2023-05-04 09:04:19.601967 collatable-0.3.2/collatable/fields/field.py
+-rw-r--r--   0        0        0      795 2023-05-04 09:04:19.601967 collatable-0.3.2/collatable/fields/index_field.py
+-rw-r--r--   0        0        0     1668 2023-05-04 09:04:19.601967 collatable-0.3.2/collatable/fields/label_field.py
+-rw-r--r--   0        0        0     1308 2023-05-04 09:04:19.601967 collatable-0.3.2/collatable/fields/list_field.py
+-rw-r--r--   0        0        0      735 2023-05-04 09:04:19.601967 collatable-0.3.2/collatable/fields/metadata_field.py
+-rw-r--r--   0        0        0      839 2023-05-04 09:04:19.601967 collatable-0.3.2/collatable/fields/scalar_field.py
+-rw-r--r--   0        0        0      266 2023-05-04 09:04:19.601967 collatable-0.3.2/collatable/fields/sequence_field.py
+-rw-r--r--   0        0        0     2385 2023-05-04 09:04:19.605967 collatable-0.3.2/collatable/fields/sequence_label_field.py
+-rw-r--r--   0        0        0     1497 2023-05-04 09:04:19.605967 collatable-0.3.2/collatable/fields/span_field.py
+-rw-r--r--   0        0        0     1006 2023-05-04 09:04:19.605967 collatable-0.3.2/collatable/fields/tensor_field.py
+-rw-r--r--   0        0        0     2203 2023-05-04 09:04:19.605967 collatable-0.3.2/collatable/fields/text_field.py
+-rw-r--r--   0        0        0      384 2023-05-04 09:04:19.605967 collatable-0.3.2/collatable/instance.py
+-rw-r--r--   0        0        0        0 2023-05-04 09:04:19.605967 collatable-0.3.2/collatable/py.typed
+-rw-r--r--   0        0        0      423 2023-05-04 09:04:19.605967 collatable-0.3.2/collatable/typing.py
+-rw-r--r--   0        0        0     1180 2023-05-04 09:04:19.605967 collatable-0.3.2/collatable/util.py
+-rw-r--r--   0        0        0     1485 2023-05-04 09:04:19.605967 collatable-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     7080 1970-01-01 00:00:00.000000 collatable-0.3.2/PKG-INFO
```

### Comparing `collatable-0.3.1/LICENSE` & `collatable-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `collatable-0.3.1/README.md` & `collatable-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `collatable-0.3.1/collatable/__init__.py` & `collatable-0.3.2/collatable/__init__.py`

 * *Files identical despite different names*

### Comparing `collatable-0.3.1/collatable/collator.py` & `collatable-0.3.2/collatable/collator.py`

 * *Files identical despite different names*

### Comparing `collatable-0.3.1/collatable/extras/dataloader.py` & `collatable-0.3.2/collatable/extras/dataloader.py`

 * *Files identical despite different names*

### Comparing `collatable-0.3.1/collatable/extras/dataset.py` & `collatable-0.3.2/collatable/extras/dataset.py`

 * *Files identical despite different names*

### Comparing `collatable-0.3.1/collatable/extras/indexer.py` & `collatable-0.3.2/collatable/extras/indexer.py`

 * *Files identical despite different names*

### Comparing `collatable-0.3.1/collatable/fields/__init__.py` & `collatable-0.3.2/collatable/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `collatable-0.3.1/collatable/fields/adjacency_field.py` & `collatable-0.3.2/collatable/fields/adjacency_field.py`

 * *Files identical despite different names*

### Comparing `collatable-0.3.1/collatable/fields/field.py` & `collatable-0.3.2/collatable/fields/field.py`

 * *Files identical despite different names*

### Comparing `collatable-0.3.1/collatable/fields/index_field.py` & `collatable-0.3.2/collatable/fields/index_field.py`

 * *Files identical despite different names*

### Comparing `collatable-0.3.1/collatable/fields/label_field.py` & `collatable-0.3.2/collatable/fields/label_field.py`

 * *Files identical despite different names*

### Comparing `collatable-0.3.1/collatable/fields/list_field.py` & `collatable-0.3.2/collatable/fields/list_field.py`

 * *Files identical despite different names*

### Comparing `collatable-0.3.1/collatable/fields/metadata_field.py` & `collatable-0.3.2/collatable/fields/metadata_field.py`

 * *Files identical despite different names*

### Comparing `collatable-0.3.1/collatable/fields/scalar_field.py` & `collatable-0.3.2/collatable/fields/scalar_field.py`

 * *Files identical despite different names*

### Comparing `collatable-0.3.1/collatable/fields/sequence_label_field.py` & `collatable-0.3.2/collatable/fields/sequence_label_field.py`

 * *Files identical despite different names*

### Comparing `collatable-0.3.1/collatable/fields/span_field.py` & `collatable-0.3.2/collatable/fields/span_field.py`

 * *Files identical despite different names*

### Comparing `collatable-0.3.1/collatable/fields/tensor_field.py` & `collatable-0.3.2/collatable/fields/tensor_field.py`

 * *Files identical despite different names*

### Comparing `collatable-0.3.1/collatable/fields/text_field.py` & `collatable-0.3.2/collatable/fields/text_field.py`

 * *Files identical despite different names*

### Comparing `collatable-0.3.1/collatable/util.py` & `collatable-0.3.2/collatable/util.py`

 * *Files identical despite different names*

### Comparing `collatable-0.3.1/pyproject.toml` & `collatable-0.3.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [tool.poetry]
 name = "collatable"
-version = "0.3.1"
+version = "0.3.2"
 description = "Constructing batched tensors for any machine learning tasks"
 authors = ["altescy <altescy@fastmail.com>"]
 license = "MIT License"
 readme = "README.md"
 homepage = "https://github.com/altescy/collatable"
 keywords = ["python", "machine learning"]
 packages = [
     { include = "collatable" },
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8.1,<4.0"
+python = ">=3.8,<4.0"
 numpy = "^1.0.0"
 
 [tool.poetry.dev-dependencies]
 python-language-server = "^0.36.2"
-pytest = "^7.1.3"
-pysen = {version = "^0.10.2"}
-black = "^22.12.0"
-isort = "^5.11.3"
-flake8 = "^6.0.0"
-mypy = "^0.991"
+pytest = "^7.3.1"
+pysen = "^0.10.4"
+black = "^23.3.0"
+isort = "^5.12.0"
+flake8 = "^5.0.4"
+mypy = "^1.2.0"
 
 [tool.pysen]
 version = "0.10"
 
 [tool.pysen-cli]
 settings_dir = "."
```

### Comparing `collatable-0.3.1/setup.py` & `collatable-0.3.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,203 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: collatable
+Version: 0.3.2
+Summary: Constructing batched tensors for any machine learning tasks
+Home-page: https://github.com/altescy/collatable
+License: MIT
+Keywords: python,machine learning
+Author: altescy
+Author-email: altescy@fastmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: numpy (>=1.0.0,<2.0.0)
+Description-Content-Type: text/markdown
+
+# Collatable
+
+[![Actions Status](https://github.com/altescy/collatable/workflows/CI/badge.svg)](https://github.com/altescy/collatable/actions/workflows/ci.yml)
+[![License](https://img.shields.io/github/license/altescy/collatable)](https://github.com/altescy/collatable/blob/main/LICENSE)
+[![Python version](https://img.shields.io/pypi/pyversions/collatable)](https://github.com/altescy/collatable)
+[![pypi version](https://img.shields.io/pypi/v/collatable)](https://pypi.org/project/collatable/)
+
+Constructing batched tensors for any machine learning tasks
+
+## Installation
+
+```bash
+pip install collatable
+```
+
+## Examples
+
+The following scripts show how to tokenize/index/collate your dataset with `collatable`:
+
+### Text Classification
+
+```python
+import collatable
+from collatable import Instance, LabelField, MetadataField, TextField
+from collatable.extras.indexer import LabelIndexer, TokenIndexer
+
+dataset = [
+    ("this is awesome", "positive"),
+    ("this is a bad movie", "negative"),
+    ("this movie is an awesome movie", "positive"),
+    ("this movie is too bad to watch", "negative"),
+]
+
+# Set up indexers for tokens and labels
+PAD_TOKEN = "<PAD>"
+UNK_TOKEN = "<UNK>"
+token_indexer = TokenIndexer[str](specials=[PAD_TOKEN, UNK_TOKEN], default=UNK_TOKEN)
+label_indexer = LabelIndexer[str]()
+
+# Load training dataset
+instances = []
+with token_indexer.context(train=True), label_indexer.context(train=True):
+    for id_, (text, label) in enumerate(dataset):
+        # Prepare each field with the corresponding field class
+        text_field = TextField(
+            text.split(),
+            indexer=token_indexer,
+            padding_value=token_indexer[PAD_TOKEN],
+        )
+        label_field = LabelField(
+            label,
+            indexer=label_indexer,
+        )
+        metadata_field = MetadataField({"id": id_})
+        # Combine these fields into instance
+        instance = Instance(
+            text=text_field,
+            label=label_field,
+            metadata=metadata_field,
+        )
+        instances.append(instance)
+
+# Collate instances and build batch
+output = collatable.collate(instances)
+print(output)
+```
+
+Execution result:
+
+```text
+{'metadata': [{'id': 0}, {'id': 1}, {'id': 2}, {'id': 3}],
+ 'text': {
+    'token_ids': array([[ 2,  3,  4,  0,  0,  0,  0],
+                        [ 2,  3,  5,  6,  7,  0,  0],
+                        [ 2,  7,  3,  8,  4,  7,  0],
+                        [ 2,  7,  3,  9,  6, 10, 11]]),
+    'mask': array([[ True,  True,  True, False, False, False, False],
+                   [ True,  True,  True,  True,  True, False, False],
+                   [ True,  True,  True,  True,  True,  True, False],
+                   [ True,  True,  True,  True,  True,  True,  True]])},
+ 'label': array([0, 1, 0, 1], dtype=int32)}
+```
+
+### Sequence Labeling
+
+```python
+import collatable
+from collatable import Instance, SequenceLabelField, TextField
+from collatable.extras.indexer import LabelIndexer, TokenIndexer
+
+dataset = [
+    (["my", "name", "is", "john", "smith"], ["O", "O", "O", "B", "I"]),
+    (["i", "lived", "in", "japan", "three", "years", "ago"], ["O", "O", "O", "U", "O", "O", "O"]),
+]
+
+# Set up indexers for tokens and labels
+PAD_TOKEN = "<PAD>"
+token_indexer = TokenIndexer[str](specials=(PAD_TOKEN,))
+label_indexer = LabelIndexer[str]()
+
+# Load training dataset
+instances = []
+with token_indexer.context(train=True), label_indexer.context(train=True):
+    for tokens, labels in dataset:
+        text_field = TextField(tokens, indexer=token_indexer, padding_value=token_indexer[PAD_TOKEN])
+        label_field = SequenceLabelField(labels, text_field, indexer=label_indexer)
+        instance = Instance(text=text_field, label=label_field)
+        instances.append(instance)
+
+output = collatable.collate(instances)
+print(output)
+```
+
+Execution result:
+
+```text
+{'label': array([[0, 0, 0, 1, 2, 0, 0],
+                 [0, 0, 0, 3, 0, 0, 0]]),
+ 'text': {
+    'token_ids': array([[ 1,  2,  3,  4,  5,  0,  0],
+                        [ 6,  7,  8,  9, 10, 11, 12]]),
+    'mask': array([[ True,  True,  True,  True,  True, False, False],
+                   [ True,  True,  True,  True,  True,  True,  True]])}}
+```
+
+### Relation Extraction
+
+```python
+import collatable
+from collatable.extras.indexer import LabelIndexer, TokenIndexer
+from collatable import AdjacencyField, Instance, ListField, SpanField, TextField
+
+PAD_TOKEN = "<PAD>"
+token_indexer = TokenIndexer[str](specials=(PAD_TOKEN,))
+label_indexer = LabelIndexer[str]()
+
+instances = []
+with token_indexer.context(train=True), label_indexer.context(train=True):
+    text = TextField(
+        ["john", "smith", "was", "born", "in", "new", "york", "and", "now", "lives", "in", "tokyo"],
+        indexer=token_indexer,
+        padding_value=token_indexer[PAD_TOKEN],
+    )
+    spans = ListField([SpanField(0, 2, text), SpanField(5, 7, text), SpanField(11, 12, text)])
+    relations = AdjacencyField([(0, 1), (0, 2)], spans, labels=["born-in", "lives-in"], indexer=label_indexer)
+    instance = Instance(text=text, spans=spans, relations=relations)
+    instances.append(instance)
+
+    text = TextField(
+        ["tokyo", "is", "the", "capital", "of", "japan"],
+        indexer=token_indexer,
+        padding_value=token_indexer[PAD_TOKEN],
+    )
+    spans = ListField([SpanField(0, 1, text), SpanField(5, 6, text)])
+    relations = AdjacencyField([(0, 1)], spans, labels=["capital-of"], indexer=label_indexer)
+    instance = Instance(text=text, spans=spans, relations=relations)
+    instances.append(instance)
+
+output = collatable.collate(instances)
+print(output)
+```
+
+Execution result:
+
+```text
+{'text': {
+    'token_ids': array([[ 1,  2,  3,  4,  5,  6,  7,  8,  9, 10,  5, 11],
+                        [11, 12, 13, 14, 15, 16,  0,  0,  0,  0,  0,  0]]),
+    'mask': array([[ True,  True,  True,  True,  True,  True,  True,  True,  True, True,  True,  True],
+                   [ True,  True,  True,  True,  True,  True, False, False, False, False, False, False]])},
+ 'spans': array([[[ 0,  2],
+                  [ 5,  7],
+                  [11, 12]],
+                 [[ 0,  1],
+                  [ 5,  6],
+                  [-1, -1]]]),
+ 'relations': array([[[-1,  0,  1],
+                      [-1, -1, -1],
+                      [-1, -1, -1]],
+                     [[-1,  2, -1],
+                      [-1, -1, -1],
+                      [-1, -1, -1]]], dtype=int32)}
+```
 
-packages = \
-['collatable', 'collatable.extras', 'collatable.fields']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['numpy>=1.0.0,<2.0.0']
-
-setup_kwargs = {
-    'name': 'collatable',
-    'version': '0.3.1',
-    'description': 'Constructing batched tensors for any machine learning tasks',
-    'long_description': '# Collatable\n\n[![Actions Status](https://github.com/altescy/collatable/workflows/CI/badge.svg)](https://github.com/altescy/collatable/actions/workflows/ci.yml)\n[![License](https://img.shields.io/github/license/altescy/collatable)](https://github.com/altescy/collatable/blob/main/LICENSE)\n[![Python version](https://img.shields.io/pypi/pyversions/collatable)](https://github.com/altescy/collatable)\n[![pypi version](https://img.shields.io/pypi/v/collatable)](https://pypi.org/project/collatable/)\n\nConstructing batched tensors for any machine learning tasks\n\n## Installation\n\n```bash\npip install collatable\n```\n\n## Examples\n\nThe following scripts show how to tokenize/index/collate your dataset with `collatable`:\n\n### Text Classification\n\n```python\nimport collatable\nfrom collatable import Instance, LabelField, MetadataField, TextField\nfrom collatable.extras.indexer import LabelIndexer, TokenIndexer\n\ndataset = [\n    ("this is awesome", "positive"),\n    ("this is a bad movie", "negative"),\n    ("this movie is an awesome movie", "positive"),\n    ("this movie is too bad to watch", "negative"),\n]\n\n# Set up indexers for tokens and labels\nPAD_TOKEN = "<PAD>"\nUNK_TOKEN = "<UNK>"\ntoken_indexer = TokenIndexer[str](specials=[PAD_TOKEN, UNK_TOKEN], default=UNK_TOKEN)\nlabel_indexer = LabelIndexer[str]()\n\n# Load training dataset\ninstances = []\nwith token_indexer.context(train=True), label_indexer.context(train=True):\n    for id_, (text, label) in enumerate(dataset):\n        # Prepare each field with the corresponding field class\n        text_field = TextField(\n            text.split(),\n            indexer=token_indexer,\n            padding_value=token_indexer[PAD_TOKEN],\n        )\n        label_field = LabelField(\n            label,\n            indexer=label_indexer,\n        )\n        metadata_field = MetadataField({"id": id_})\n        # Combine these fields into instance\n        instance = Instance(\n            text=text_field,\n            label=label_field,\n            metadata=metadata_field,\n        )\n        instances.append(instance)\n\n# Collate instances and build batch\noutput = collatable.collate(instances)\nprint(output)\n```\n\nExecution result:\n\n```text\n{\'metadata\': [{\'id\': 0}, {\'id\': 1}, {\'id\': 2}, {\'id\': 3}],\n \'text\': {\n    \'token_ids\': array([[ 2,  3,  4,  0,  0,  0,  0],\n                        [ 2,  3,  5,  6,  7,  0,  0],\n                        [ 2,  7,  3,  8,  4,  7,  0],\n                        [ 2,  7,  3,  9,  6, 10, 11]]),\n    \'mask\': array([[ True,  True,  True, False, False, False, False],\n                   [ True,  True,  True,  True,  True, False, False],\n                   [ True,  True,  True,  True,  True,  True, False],\n                   [ True,  True,  True,  True,  True,  True,  True]])},\n \'label\': array([0, 1, 0, 1], dtype=int32)}\n```\n\n### Sequence Labeling\n\n```python\nimport collatable\nfrom collatable import Instance, SequenceLabelField, TextField\nfrom collatable.extras.indexer import LabelIndexer, TokenIndexer\n\ndataset = [\n    (["my", "name", "is", "john", "smith"], ["O", "O", "O", "B", "I"]),\n    (["i", "lived", "in", "japan", "three", "years", "ago"], ["O", "O", "O", "U", "O", "O", "O"]),\n]\n\n# Set up indexers for tokens and labels\nPAD_TOKEN = "<PAD>"\ntoken_indexer = TokenIndexer[str](specials=(PAD_TOKEN,))\nlabel_indexer = LabelIndexer[str]()\n\n# Load training dataset\ninstances = []\nwith token_indexer.context(train=True), label_indexer.context(train=True):\n    for tokens, labels in dataset:\n        text_field = TextField(tokens, indexer=token_indexer, padding_value=token_indexer[PAD_TOKEN])\n        label_field = SequenceLabelField(labels, text_field, indexer=label_indexer)\n        instance = Instance(text=text_field, label=label_field)\n        instances.append(instance)\n\noutput = collatable.collate(instances)\nprint(output)\n```\n\nExecution result:\n\n```text\n{\'label\': array([[0, 0, 0, 1, 2, 0, 0],\n                 [0, 0, 0, 3, 0, 0, 0]]),\n \'text\': {\n    \'token_ids\': array([[ 1,  2,  3,  4,  5,  0,  0],\n                        [ 6,  7,  8,  9, 10, 11, 12]]),\n    \'mask\': array([[ True,  True,  True,  True,  True, False, False],\n                   [ True,  True,  True,  True,  True,  True,  True]])}}\n```\n\n### Relation Extraction\n\n```python\nimport collatable\nfrom collatable.extras.indexer import LabelIndexer, TokenIndexer\nfrom collatable import AdjacencyField, Instance, ListField, SpanField, TextField\n\nPAD_TOKEN = "<PAD>"\ntoken_indexer = TokenIndexer[str](specials=(PAD_TOKEN,))\nlabel_indexer = LabelIndexer[str]()\n\ninstances = []\nwith token_indexer.context(train=True), label_indexer.context(train=True):\n    text = TextField(\n        ["john", "smith", "was", "born", "in", "new", "york", "and", "now", "lives", "in", "tokyo"],\n        indexer=token_indexer,\n        padding_value=token_indexer[PAD_TOKEN],\n    )\n    spans = ListField([SpanField(0, 2, text), SpanField(5, 7, text), SpanField(11, 12, text)])\n    relations = AdjacencyField([(0, 1), (0, 2)], spans, labels=["born-in", "lives-in"], indexer=label_indexer)\n    instance = Instance(text=text, spans=spans, relations=relations)\n    instances.append(instance)\n\n    text = TextField(\n        ["tokyo", "is", "the", "capital", "of", "japan"],\n        indexer=token_indexer,\n        padding_value=token_indexer[PAD_TOKEN],\n    )\n    spans = ListField([SpanField(0, 1, text), SpanField(5, 6, text)])\n    relations = AdjacencyField([(0, 1)], spans, labels=["capital-of"], indexer=label_indexer)\n    instance = Instance(text=text, spans=spans, relations=relations)\n    instances.append(instance)\n\noutput = collatable.collate(instances)\nprint(output)\n```\n\nExecution result:\n\n```text\n{\'text\': {\n    \'token_ids\': array([[ 1,  2,  3,  4,  5,  6,  7,  8,  9, 10,  5, 11],\n                        [11, 12, 13, 14, 15, 16,  0,  0,  0,  0,  0,  0]]),\n    \'mask\': array([[ True,  True,  True,  True,  True,  True,  True,  True,  True, True,  True,  True],\n                   [ True,  True,  True,  True,  True,  True, False, False, False, False, False, False]])},\n \'spans\': array([[[ 0,  2],\n                  [ 5,  7],\n                  [11, 12]],\n                 [[ 0,  1],\n                  [ 5,  6],\n                  [-1, -1]]]),\n \'relations\': array([[[-1,  0,  1],\n                      [-1, -1, -1],\n                      [-1, -1, -1]],\n                     [[-1,  2, -1],\n                      [-1, -1, -1],\n                      [-1, -1, -1]]], dtype=int32)}\n```\n',
-    'author': 'altescy',
-    'author_email': 'altescy@fastmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/altescy/collatable',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8.1,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

