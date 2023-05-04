# Comparing `tmp/spacy_huggingface_pipelines-0.0.2.tar.gz` & `tmp/spacy_huggingface_pipelines-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacy_huggingface_pipelines-0.0.2.tar", last modified: Wed Apr 26 13:18:52 2023, max compression
+gzip compressed data, was "spacy_huggingface_pipelines-0.0.3.tar", last modified: Thu May  4 15:26:45 2023, max compression
```

## Comparing `spacy_huggingface_pipelines-0.0.2.tar` & `spacy_huggingface_pipelines-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-26 13:18:52.302397 spacy_huggingface_pipelines-0.0.2/
--rw-r--r--   0 vsts      (1001) docker     (122)     1073 2023-04-26 13:18:35.000000 spacy_huggingface_pipelines-0.0.2/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      102 2023-04-26 13:18:35.000000 spacy_huggingface_pipelines-0.0.2/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     9718 2023-04-26 13:18:52.302397 spacy_huggingface_pipelines-0.0.2/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     8455 2023-04-26 13:18:35.000000 spacy_huggingface_pipelines-0.0.2/README.md
--rw-r--r--   0 vsts      (1001) docker     (122)       88 2023-04-26 13:18:35.000000 spacy_huggingface_pipelines-0.0.2/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (122)     1766 2023-04-26 13:18:52.306397 spacy_huggingface_pipelines-0.0.2/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)      171 2023-04-26 13:18:35.000000 spacy_huggingface_pipelines-0.0.2/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-26 13:18:52.302397 spacy_huggingface_pipelines-0.0.2/spacy_huggingface_pipelines/
--rw-r--r--   0 vsts      (1001) docker     (122)      143 2023-04-26 13:18:35.000000 spacy_huggingface_pipelines-0.0.2/spacy_huggingface_pipelines/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-26 13:18:52.302397 spacy_huggingface_pipelines-0.0.2/spacy_huggingface_pipelines/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-26 13:18:35.000000 spacy_huggingface_pipelines-0.0.2/spacy_huggingface_pipelines/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)       45 2023-04-26 13:18:35.000000 spacy_huggingface_pipelines-0.0.2/spacy_huggingface_pipelines/tests/enable_gpu.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3028 2023-04-26 13:18:35.000000 spacy_huggingface_pipelines-0.0.2/spacy_huggingface_pipelines/tests/test_pipeline_components.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3701 2023-04-26 13:18:35.000000 spacy_huggingface_pipelines-0.0.2/spacy_huggingface_pipelines/text_classification.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6764 2023-04-26 13:18:35.000000 spacy_huggingface_pipelines-0.0.2/spacy_huggingface_pipelines/token_classification.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-26 13:18:52.302397 spacy_huggingface_pipelines-0.0.2/spacy_huggingface_pipelines.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     9718 2023-04-26 13:18:52.000000 spacy_huggingface_pipelines-0.0.2/spacy_huggingface_pipelines.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      720 2023-04-26 13:18:52.000000 spacy_huggingface_pipelines-0.0.2/spacy_huggingface_pipelines.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-26 13:18:52.000000 spacy_huggingface_pipelines-0.0.2/spacy_huggingface_pipelines.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      183 2023-04-26 13:18:52.000000 spacy_huggingface_pipelines-0.0.2/spacy_huggingface_pipelines.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-26 13:18:52.000000 spacy_huggingface_pipelines-0.0.2/spacy_huggingface_pipelines.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)       61 2023-04-26 13:18:52.000000 spacy_huggingface_pipelines-0.0.2/spacy_huggingface_pipelines.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       28 2023-04-26 13:18:52.000000 spacy_huggingface_pipelines-0.0.2/spacy_huggingface_pipelines.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-04 15:26:45.280632 spacy_huggingface_pipelines-0.0.3/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1073 2023-05-04 15:26:29.000000 spacy_huggingface_pipelines-0.0.3/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      102 2023-05-04 15:26:29.000000 spacy_huggingface_pipelines-0.0.3/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     9718 2023-05-04 15:26:45.280632 spacy_huggingface_pipelines-0.0.3/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     8455 2023-05-04 15:26:29.000000 spacy_huggingface_pipelines-0.0.3/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)       88 2023-05-04 15:26:29.000000 spacy_huggingface_pipelines-0.0.3/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)     1766 2023-05-04 15:26:45.280632 spacy_huggingface_pipelines-0.0.3/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)      171 2023-05-04 15:26:29.000000 spacy_huggingface_pipelines-0.0.3/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-04 15:26:45.276632 spacy_huggingface_pipelines-0.0.3/spacy_huggingface_pipelines/
+-rw-r--r--   0 vsts      (1001) docker     (122)      143 2023-05-04 15:26:29.000000 spacy_huggingface_pipelines-0.0.3/spacy_huggingface_pipelines/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-04 15:26:45.280632 spacy_huggingface_pipelines-0.0.3/spacy_huggingface_pipelines/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-04 15:26:29.000000 spacy_huggingface_pipelines-0.0.3/spacy_huggingface_pipelines/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       45 2023-05-04 15:26:29.000000 spacy_huggingface_pipelines-0.0.3/spacy_huggingface_pipelines/tests/enable_gpu.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3028 2023-05-04 15:26:29.000000 spacy_huggingface_pipelines-0.0.3/spacy_huggingface_pipelines/tests/test_pipeline_components.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3701 2023-05-04 15:26:29.000000 spacy_huggingface_pipelines-0.0.3/spacy_huggingface_pipelines/text_classification.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6764 2023-05-04 15:26:29.000000 spacy_huggingface_pipelines-0.0.3/spacy_huggingface_pipelines/token_classification.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-04 15:26:45.276632 spacy_huggingface_pipelines-0.0.3/spacy_huggingface_pipelines.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     9718 2023-05-04 15:26:45.000000 spacy_huggingface_pipelines-0.0.3/spacy_huggingface_pipelines.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      720 2023-05-04 15:26:45.000000 spacy_huggingface_pipelines-0.0.3/spacy_huggingface_pipelines.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-04 15:26:45.000000 spacy_huggingface_pipelines-0.0.3/spacy_huggingface_pipelines.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      183 2023-05-04 15:26:45.000000 spacy_huggingface_pipelines-0.0.3/spacy_huggingface_pipelines.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-04 15:26:45.000000 spacy_huggingface_pipelines-0.0.3/spacy_huggingface_pipelines.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)       61 2023-05-04 15:26:45.000000 spacy_huggingface_pipelines-0.0.3/spacy_huggingface_pipelines.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       28 2023-05-04 15:26:45.000000 spacy_huggingface_pipelines-0.0.3/spacy_huggingface_pipelines.egg-info/top_level.txt
```

### Comparing `spacy_huggingface_pipelines-0.0.2/LICENSE` & `spacy_huggingface_pipelines-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spacy_huggingface_pipelines-0.0.2/PKG-INFO` & `spacy_huggingface_pipelines-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacy_huggingface_pipelines
-Version: 0.0.2
+Version: 0.0.3
 Summary: spaCy wrapper for Hugging Face Transformers pipelines
 Home-page: https://github.com/explosion/spacy-huggingface-pipelines
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Project-URL: Release notes, https://github.com/explosion/spacy-huggingface-pipelines/releases
 Project-URL: Source, https://github.com/explosion/spacy-huggingface-pipelines
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spacy_huggingface_pipelines Version: 0.0.2 Summary:
+Metadata-Version: 2.1 Name: spacy_huggingface_pipelines Version: 0.0.3 Summary:
 spaCy wrapper for Hugging Face Transformers pipelines Home-page: https://
 github.com/explosion/spacy-huggingface-pipelines Author: Explosion Author-
 email: contact@explosion.ai License: MIT Project-URL: Release notes, https://
 github.com/explosion/spacy-huggingface-pipelines/releases Project-URL: Source,
 https://github.com/explosion/spacy-huggingface-pipelines Classifier:
 Development Status :: 4 - Beta Classifier: Environment :: Console Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Science/
```

### Comparing `spacy_huggingface_pipelines-0.0.2/README.md` & `spacy_huggingface_pipelines-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `spacy_huggingface_pipelines-0.0.2/setup.cfg` & `spacy_huggingface_pipelines-0.0.3/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 0.0.2
+version = 0.0.3
 description = spaCy wrapper for Hugging Face Transformers pipelines
 url = https://github.com/explosion/spacy-huggingface-pipelines
 author = Explosion
 author_email = contact@explosion.ai
 license = MIT
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `spacy_huggingface_pipelines-0.0.2/spacy_huggingface_pipelines/tests/test_pipeline_components.py` & `spacy_huggingface_pipelines-0.0.3/spacy_huggingface_pipelines/tests/test_pipeline_components.py`

 * *Files identical despite different names*

### Comparing `spacy_huggingface_pipelines-0.0.2/spacy_huggingface_pipelines/text_classification.py` & `spacy_huggingface_pipelines-0.0.3/spacy_huggingface_pipelines/text_classification.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,22 +44,22 @@
         task="text-classification",
         model=model,
         revision=revision,
         device=device,
         truncation=True,
         **kwargs,
     )
-    return HfTextPipe(
+    return HFTextPipe(
         name=name,
         hf_pipeline=hf_pipeline,
         scorer=scorer,
     )
 
 
-class HfTextPipe(Pipe):
+class HFTextPipe(Pipe):
     def __init__(
         self, name: str, hf_pipeline: pipeline, *, scorer: Optional[Callable] = None
     ):
         self.name = name
         self.hf_pipeline = hf_pipeline
         self.scorer = scorer
```

### Comparing `spacy_huggingface_pipelines-0.0.2/spacy_huggingface_pipelines/token_classification.py` & `spacy_huggingface_pipelines-0.0.3/spacy_huggingface_pipelines/token_classification.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,25 +58,25 @@
         model=model,
         revision=revision,
         aggregation_strategy=aggregation_strategy,
         device=device,
         stride=stride,
         **kwargs,
     )
-    return HfTokenPipe(
+    return HFTokenPipe(
         name=name,
         hf_pipeline=hf_pipeline,
         annotate=annotate,
         annotate_spans_key=annotate_spans_key,
         alignment_mode=alignment_mode,
         scorer=scorer,
     )
 
 
-class HfTokenPipe(Pipe):
+class HFTokenPipe(Pipe):
     def __init__(
         self,
         name: str,
         hf_pipeline: pipeline,
         *,
         annotate: Literal["ents", "pos", "spans", "tag"] = "ents",
         annotate_spans_key: Optional[str] = None,
```

### Comparing `spacy_huggingface_pipelines-0.0.2/spacy_huggingface_pipelines.egg-info/PKG-INFO` & `spacy_huggingface_pipelines-0.0.3/spacy_huggingface_pipelines.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacy-huggingface-pipelines
-Version: 0.0.2
+Version: 0.0.3
 Summary: spaCy wrapper for Hugging Face Transformers pipelines
 Home-page: https://github.com/explosion/spacy-huggingface-pipelines
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Project-URL: Release notes, https://github.com/explosion/spacy-huggingface-pipelines/releases
 Project-URL: Source, https://github.com/explosion/spacy-huggingface-pipelines
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spacy-huggingface-pipelines Version: 0.0.2 Summary:
+Metadata-Version: 2.1 Name: spacy-huggingface-pipelines Version: 0.0.3 Summary:
 spaCy wrapper for Hugging Face Transformers pipelines Home-page: https://
 github.com/explosion/spacy-huggingface-pipelines Author: Explosion Author-
 email: contact@explosion.ai License: MIT Project-URL: Release notes, https://
 github.com/explosion/spacy-huggingface-pipelines/releases Project-URL: Source,
 https://github.com/explosion/spacy-huggingface-pipelines Classifier:
 Development Status :: 4 - Beta Classifier: Environment :: Console Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Science/
```

### Comparing `spacy_huggingface_pipelines-0.0.2/spacy_huggingface_pipelines.egg-info/SOURCES.txt` & `spacy_huggingface_pipelines-0.0.3/spacy_huggingface_pipelines.egg-info/SOURCES.txt`

 * *Files identical despite different names*

