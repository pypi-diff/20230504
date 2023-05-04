# Comparing `tmp/responsibleai_text-0.1.1.tar.gz` & `tmp/responsibleai_text-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/responsibleai_text-0.1.1.tar", last modified: Thu Apr 27 20:24:24 2023, max compression
+gzip compressed data, was "dist/responsibleai_text-0.1.2.tar", last modified: Thu May  4 21:48:52 2023, max compression
```

## Comparing `responsibleai_text-0.1.1.tar` & `responsibleai_text-0.1.2.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:24:24.000000 responsibleai_text-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-27 20:24:24.000000 responsibleai_text-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-27 20:21:44.000000 responsibleai_text-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:24:24.000000 responsibleai_text-0.1.1/responsibleai_text/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-27 20:21:44.000000 responsibleai_text-0.1.1/responsibleai_text/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:24:24.000000 responsibleai_text-0.1.1/responsibleai_text/common/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-27 20:21:44.000000 responsibleai_text-0.1.1/responsibleai_text/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-27 20:21:44.000000 responsibleai_text-0.1.1/responsibleai_text/common/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:24:24.000000 responsibleai_text-0.1.1/responsibleai_text/managers/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-27 20:21:44.000000 responsibleai_text-0.1.1/responsibleai_text/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12392 2023-04-27 20:21:44.000000 responsibleai_text-0.1.1/responsibleai_text/managers/error_analysis_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    13920 2023-04-27 20:21:44.000000 responsibleai_text-0.1.1/responsibleai_text/managers/explainer_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:24:24.000000 responsibleai_text-0.1.1/responsibleai_text/rai_text_insights/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-27 20:21:44.000000 responsibleai_text-0.1.1/responsibleai_text/rai_text_insights/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25644 2023-04-27 20:21:44.000000 responsibleai_text-0.1.1/responsibleai_text/rai_text_insights/rai_text_insights.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:24:24.000000 responsibleai_text-0.1.1/responsibleai_text/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-27 20:21:44.000000 responsibleai_text-0.1.1/responsibleai_text/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-04-27 20:21:44.000000 responsibleai_text-0.1.1/responsibleai_text/utils/feature_extractors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-27 20:21:44.000000 responsibleai_text-0.1.1/responsibleai_text/utils/question_answering.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-27 20:21:44.000000 responsibleai_text-0.1.1/responsibleai_text/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:24:24.000000 responsibleai_text-0.1.1/responsibleai_text.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-27 20:24:24.000000 responsibleai_text-0.1.1/responsibleai_text.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-27 20:24:24.000000 responsibleai_text-0.1.1/responsibleai_text.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 20:24:24.000000 responsibleai_text-0.1.1/responsibleai_text.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-27 20:24:24.000000 responsibleai_text-0.1.1/responsibleai_text.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-27 20:24:24.000000 responsibleai_text-0.1.1/responsibleai_text.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 20:24:24.000000 responsibleai_text-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-27 20:21:44.000000 responsibleai_text-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:24:24.000000 responsibleai_text-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-04-27 20:21:44.000000 responsibleai_text-0.1.1/tests/test_rai_text_insights.py
--rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-04-27 20:21:44.000000 responsibleai_text-0.1.1/tests/test_rai_text_insights_save_and_load_scenarios.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:48:52.000000 responsibleai_text-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-04 21:48:52.000000 responsibleai_text-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-04 21:46:08.000000 responsibleai_text-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:48:52.000000 responsibleai_text-0.1.2/responsibleai_text/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-04 21:46:08.000000 responsibleai_text-0.1.2/responsibleai_text/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:48:52.000000 responsibleai_text-0.1.2/responsibleai_text/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-04 21:46:08.000000 responsibleai_text-0.1.2/responsibleai_text/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-04 21:46:08.000000 responsibleai_text-0.1.2/responsibleai_text/common/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:48:52.000000 responsibleai_text-0.1.2/responsibleai_text/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-04 21:46:08.000000 responsibleai_text-0.1.2/responsibleai_text/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12392 2023-05-04 21:46:08.000000 responsibleai_text-0.1.2/responsibleai_text/managers/error_analysis_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13920 2023-05-04 21:46:08.000000 responsibleai_text-0.1.2/responsibleai_text/managers/explainer_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:48:52.000000 responsibleai_text-0.1.2/responsibleai_text/rai_text_insights/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-04 21:46:08.000000 responsibleai_text-0.1.2/responsibleai_text/rai_text_insights/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25504 2023-05-04 21:46:08.000000 responsibleai_text-0.1.2/responsibleai_text/rai_text_insights/rai_text_insights.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:48:52.000000 responsibleai_text-0.1.2/responsibleai_text/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-04 21:46:08.000000 responsibleai_text-0.1.2/responsibleai_text/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-05-04 21:46:08.000000 responsibleai_text-0.1.2/responsibleai_text/utils/feature_extractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-04 21:46:08.000000 responsibleai_text-0.1.2/responsibleai_text/utils/question_answering.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-04 21:46:08.000000 responsibleai_text-0.1.2/responsibleai_text/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:48:52.000000 responsibleai_text-0.1.2/responsibleai_text.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-04 21:48:52.000000 responsibleai_text-0.1.2/responsibleai_text.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-04 21:48:52.000000 responsibleai_text-0.1.2/responsibleai_text.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 21:48:52.000000 responsibleai_text-0.1.2/responsibleai_text.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-04 21:48:52.000000 responsibleai_text-0.1.2/responsibleai_text.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-04 21:48:52.000000 responsibleai_text-0.1.2/responsibleai_text.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 21:48:52.000000 responsibleai_text-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-04 21:46:08.000000 responsibleai_text-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:48:52.000000 responsibleai_text-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-04 21:46:08.000000 responsibleai_text-0.1.2/tests/test_feature_extractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-04 21:46:08.000000 responsibleai_text-0.1.2/tests/test_rai_text_insights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-05-04 21:46:08.000000 responsibleai_text-0.1.2/tests/test_rai_text_insights_save_and_load_scenarios.py
```

### Comparing `responsibleai_text-0.1.1/PKG-INFO` & `responsibleai_text-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: responsibleai_text
-Version: 0.1.1
+Version: 0.1.2
 Summary: SDK API to assess text Machine Learning models.
 Home-page: https://github.com/microsoft/responsible-ai-toolbox
 Author: Roman Lutz, Ilya Matiach, Ke Xu
 Author-email: raiwidgets-maintain@microsoft.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `responsibleai_text-0.1.1/README.md` & `responsibleai_text-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `responsibleai_text-0.1.1/responsibleai_text/common/constants.py` & `responsibleai_text-0.1.2/responsibleai_text/common/constants.py`

 * *Files identical despite different names*

### Comparing `responsibleai_text-0.1.1/responsibleai_text/managers/error_analysis_manager.py` & `responsibleai_text-0.1.2/responsibleai_text/managers/error_analysis_manager.py`

 * *Files identical despite different names*

### Comparing `responsibleai_text-0.1.1/responsibleai_text/managers/explainer_manager.py` & `responsibleai_text-0.1.2/responsibleai_text/managers/explainer_manager.py`

 * *Files identical despite different names*

### Comparing `responsibleai_text-0.1.1/responsibleai_text/rai_text_insights/rai_text_insights.py` & `responsibleai_text-0.1.2/responsibleai_text/rai_text_insights/rai_text_insights.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from typing import Any, List, Optional, Union
 
 import numpy as np
 import pandas as pd
 from erroranalysis._internal.cohort_filter import FilterDataWithCohortFilters
 from ml_wrappers import wrap_model
 from raiutils.data_processing import convert_to_list, serialize_json_safe
-from raiutils.models import ModelTask as RAIModelTask
 from raiutils.models import SKLearn, is_classifier
 from responsibleai._interfaces import Dataset, RAIInsightsData
 from responsibleai._internal.constants import (ManagerNames, Metadata,
                                                SerializationAttributes)
 from responsibleai.exceptions import UserConfigValidationException
 from responsibleai.rai_insights.rai_base_insights import RAIBaseInsights
 
@@ -428,23 +427,21 @@
         classification_tasks = [ModelTask.TEXT_CLASSIFICATION,
                                 ModelTask.MULTILABEL_TEXT_CLASSIFICATION]
         return self.task_type in classification_tasks
 
     def _get_dataset(self):
         dashboard_dataset = Dataset()
         tasktype = self.task_type
-        is_classification_task = self._is_classification_task
-        if is_classification_task:
-            tasktype = RAIModelTask.CLASSIFICATION
         if isinstance(tasktype, Enum):
             tasktype = tasktype.value
         dashboard_dataset.task_type = tasktype
         dashboard_dataset.categorical_features = []
         dashboard_dataset.class_names = convert_to_list(
             self._classes)
+        is_classification_task = self._is_classification_task
         dataset = self._get_test_without_target(is_classification_task)
 
         predicted_y = None
         if dataset is not None and self._wrapped_model is not None:
             try:
                 predicted_y = self._wrapped_model.predict(dataset)
             except Exception as ex:
```

### Comparing `responsibleai_text-0.1.1/responsibleai_text/utils/feature_extractors.py` & `responsibleai_text-0.1.2/responsibleai_text/utils/feature_extractors.py`

 * *Files 24% similar despite different names*

```diff
@@ -45,14 +45,15 @@
         prefixes = [QuestionAnsweringFields.CONTEXT + "_",
                     QuestionAnsweringFields.QUESTION + "_"]
         for prefix in prefixes:
             for feature_name in base_feature_names:
                 feature_names.append(prefix + feature_name)
 
         feature_names.append("question_type")
+        feature_names.append("context_overlap")
     else:
         raise ValueError("Unknown task type: {}".format(task_type))
     if not isinstance(target_column, list):
         target_column = [target_column]
     text_features = text_dataset.drop(target_column, axis=1)
 
     if task_type in single_text_col_tasks:
@@ -64,14 +65,18 @@
     elif task_type == ModelTask.QUESTION_ANSWERING:
         for _, row in tqdm(text_features.iterrows()):
             extracted_features = []
             add_extracted_features_for_sentence(
                 row[QuestionAnsweringFields.CONTEXT], extracted_features)
             add_extracted_features_for_sentence(
                 row[QuestionAnsweringFields.QUESTIONS], extracted_features, sentence_type="QUESTION")
+
+            context_overlap = get_context_overlap(context=row[QuestionAnsweringFields.CONTEXT],
+                                                  question=row[QuestionAnsweringFields.QUESTIONS])
+            extracted_features.append(context_overlap)
             results.append(extracted_features)
     else:
         raise ValueError("Unknown task type: {}".format(task_type))
     return results, feature_names
 
 
 def add_extracted_features_for_sentence(sentence, extracted_features, sentence_type=None):
@@ -99,37 +104,57 @@
     # TODO: This extractor seems to be very slow:
     # mf_count = exts.get_male_female_words_count(doc)
 
     extracted_features.extend(features)
 
 
 def get_question_type(qtext):
-
-    if re.search(r'\b\A(can|could|will|would|have|has|do|does|' +
-                 'did|is|are|was|may|might)', qtext, re.I):
+    if re.search(r'\b\A(can|could|will|would|have|has|do|does|did|is|are|was|may|might)\s',
+                 qtext, re.I):
         return "YES/NO"
-    elif re.search(r'\b\A(what|which)\s+(\w+)', qtext, re.I):
-        nextword = re.search(r'\b\A(what|which)\s+(\w+)', qtext, re.I).group(2)
-        if nextword == "year" or nextword == "month" or nextword == "date" or nextword == "day":
+    elif re.search(r'\b\A(what|which)(\'s|\'re)?\s+(\w+)', qtext, re.I):
+        nextword = re.search(r'\b\A(what|which)(\'s|\'re)?\s+(\w+)', qtext, re.I).group(3)
+        if nextword in ["year", "month", "date", "day"]:
             return "WHEN"
         else:
             return "WHAT"
-    elif re.search(r'\bwho\s', qtext, re.I):
+    elif re.search(r'\bwho(\'s|\'re)?\s', qtext, re.I):
         return "WHO"
-    elif re.search(r'\bwhy\s', qtext, re.I):
+    elif re.search(r'\bwhy(\'s|\'re)?\s', qtext, re.I):
         return "WHY"
-    elif re.search(r'\bwhere\s', qtext, re.I):
+    elif re.search(r'\bwhere(\'s|\'re)?\s', qtext, re.I):
         return "WHERE"
-    elif re.search(r'\bhow\s', qtext, re.I):
-        nextword = re.search(r'\b(how)\s(\w+)', qtext, re.I).group(2)
-        if nextword == "many" or nextword == "much" or nextword == "long":
+    elif re.search(r'\bhow(\'s|\'re)?\s', qtext, re.I):
+        nextword = re.search(r'\b(how)(\'s|\'re)?\s(\w+)', qtext, re.I).group(3)
+        if nextword in ["many", "much", "long", "old", "often"]:
             return "NUMBER"
         else:
             return "HOW"
-    elif re.search(r'\bwhen\s', qtext, re.I):
+    elif re.search(r'\bwhen(\'s|\'re)?\s', qtext, re.I):
         return "WHEN"
-    elif "in what year" in qtext or "in which year" in qtext:
+    elif re.search(r'\b(in|on|at|by|for|to|from|during|within)\s+(what|which)\s+(year|month|day|date|time)\s',
+                   qtext, re.I):
         return "WHEN"
     elif re.search(r'\bto\swhom\s', qtext, re.I):
         return "WHO"
     else:
         return "OTHER"
+
+
+def get_context_overlap(context, question):
+    global nlp
+    if nlp is None:
+        nlp = spacy.load("en_core_web_sm")
+
+    doc_q = nlp(question)
+    doc_c = nlp(context)
+
+    # get tokens in base form
+    tokens_q = set([token.lemma_ for token in doc_q if not token.is_stop and not token.is_punct])
+    tokens_c = set([token.lemma_ for token in doc_c if not token.is_stop and not token.is_punct])
+
+    intersection = tokens_q.intersection(tokens_c)
+
+    # the size of the intersection token set /  the size of the question token set
+    overlap_ratio = len(intersection) / len(tokens_q)
+
+    return round(overlap_ratio, 3)
```

### Comparing `responsibleai_text-0.1.1/responsibleai_text/utils/question_answering.py` & `responsibleai_text-0.1.2/responsibleai_text/utils/question_answering.py`

 * *Files identical despite different names*

### Comparing `responsibleai_text-0.1.1/responsibleai_text.egg-info/PKG-INFO` & `responsibleai_text-0.1.2/responsibleai_text.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: responsibleai-text
-Version: 0.1.1
+Version: 0.1.2
 Summary: SDK API to assess text Machine Learning models.
 Home-page: https://github.com/microsoft/responsible-ai-toolbox
 Author: Roman Lutz, Ilya Matiach, Ke Xu
 Author-email: raiwidgets-maintain@microsoft.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `responsibleai_text-0.1.1/responsibleai_text.egg-info/SOURCES.txt` & `responsibleai_text-0.1.2/responsibleai_text.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -13,9 +13,10 @@
 responsibleai_text/managers/error_analysis_manager.py
 responsibleai_text/managers/explainer_manager.py
 responsibleai_text/rai_text_insights/__init__.py
 responsibleai_text/rai_text_insights/rai_text_insights.py
 responsibleai_text/utils/__init__.py
 responsibleai_text/utils/feature_extractors.py
 responsibleai_text/utils/question_answering.py
+tests/test_feature_extractors.py
 tests/test_rai_text_insights.py
 tests/test_rai_text_insights_save_and_load_scenarios.py
```

### Comparing `responsibleai_text-0.1.1/setup.py` & `responsibleai_text-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `responsibleai_text-0.1.1/tests/test_rai_text_insights.py` & `responsibleai_text-0.1.2/tests/test_rai_text_insights.py`

 * *Files identical despite different names*

### Comparing `responsibleai_text-0.1.1/tests/test_rai_text_insights_save_and_load_scenarios.py` & `responsibleai_text-0.1.2/tests/test_rai_text_insights_save_and_load_scenarios.py`

 * *Files identical despite different names*

