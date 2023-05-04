# Comparing `tmp/headline_detector-1.0.1.tar.gz` & `tmp/headline_detector-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "headline_detector-1.0.1.tar", last modified: Tue May  2 12:40:57 2023, max compression
+gzip compressed data, was "headline_detector-1.0.2.tar", last modified: Thu May  4 08:25:52 2023, max compression
```

## Comparing `headline_detector-1.0.1.tar` & `headline_detector-1.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 12:40:57.685066 headline_detector-1.0.1/
--rw-rw-rw-   0        0        0     3367 2023-05-02 12:40:57.685066 headline_detector-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2418 2023-05-02 12:37:59.000000 headline_detector-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-02 12:40:57.685066 headline_detector-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      884 2023-05-02 12:40:52.000000 headline_detector-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:40:57.656065 headline_detector-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-02 12:40:57.667065 headline_detector-1.0.1/src/headline_detector/
--rw-rw-rw-   0        0        0       93 2023-05-02 12:00:22.000000 headline_detector-1.0.1/src/headline_detector/__init__.py
--rw-rw-rw-   0        0        0     7773 2023-05-02 12:00:50.000000 headline_detector-1.0.1/src/headline_detector/detector.py
--rw-rw-rw-   0        0        0      498 2023-05-02 09:35:48.000000 headline_detector-1.0.1/src/headline_detector/hyper_params.py
--rw-rw-rw-   0        0        0     5241 2023-05-02 11:58:36.000000 headline_detector-1.0.1/src/headline_detector/model.py
--rw-rw-rw-   0        0        0     1407 2023-05-02 09:47:20.000000 headline_detector-1.0.1/src/headline_detector/model_checkpoint.py
--rw-rw-rw-   0        0        0     1812 2023-05-02 11:26:46.000000 headline_detector-1.0.1/src/headline_detector/preprocessing_scenario.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:40:57.684066 headline_detector-1.0.1/src/headline_detector/processing_pipeline/
--rw-rw-rw-   0        0        0      142 2023-05-02 11:08:45.000000 headline_detector-1.0.1/src/headline_detector/processing_pipeline/__init__.py
--rw-rw-rw-   0        0        0     1758 2023-05-02 11:32:18.000000 headline_detector-1.0.1/src/headline_detector/processing_pipeline/pipeline.py
--rw-rw-rw-   0        0        0     2256 2023-05-02 11:07:28.000000 headline_detector-1.0.1/src/headline_detector/processing_pipeline/processing_func.py
--rw-rw-rw-   0        0        0     2821 2023-05-02 11:07:12.000000 headline_detector-1.0.1/src/headline_detector/processing_pipeline/stemmer.py
--rw-rw-rw-   0        0        0      202 2023-05-02 10:42:33.000000 headline_detector-1.0.1/src/headline_detector/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:40:57.679064 headline_detector-1.0.1/src/headline_detector.egg-info/
--rw-rw-rw-   0        0        0     3367 2023-05-02 12:40:57.000000 headline_detector-1.0.1/src/headline_detector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      722 2023-05-02 12:40:57.000000 headline_detector-1.0.1/src/headline_detector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 12:40:57.000000 headline_detector-1.0.1/src/headline_detector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2023-05-02 12:40:57.000000 headline_detector-1.0.1/src/headline_detector.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-02 12:40:57.000000 headline_detector-1.0.1/src/headline_detector.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 08:25:52.850201 headline_detector-1.0.2/
+-rw-rw-rw-   0        0        0     2729 2023-05-04 08:25:52.849202 headline_detector-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2418 2023-05-02 12:37:59.000000 headline_detector-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-04 08:25:52.850201 headline_detector-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      781 2023-05-04 08:25:35.000000 headline_detector-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 08:25:52.821200 headline_detector-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-04 08:25:52.830201 headline_detector-1.0.2/src/headline_detector/
+-rw-rw-rw-   0        0        0       93 2023-05-02 12:00:22.000000 headline_detector-1.0.2/src/headline_detector/__init__.py
+-rw-rw-rw-   0        0        0     7773 2023-05-02 12:00:50.000000 headline_detector-1.0.2/src/headline_detector/detector.py
+-rw-rw-rw-   0        0        0      498 2023-05-02 09:35:48.000000 headline_detector-1.0.2/src/headline_detector/hyper_params.py
+-rw-rw-rw-   0        0        0     5241 2023-05-02 11:58:36.000000 headline_detector-1.0.2/src/headline_detector/model.py
+-rw-rw-rw-   0        0        0     1407 2023-05-02 09:47:20.000000 headline_detector-1.0.2/src/headline_detector/model_checkpoint.py
+-rw-rw-rw-   0        0        0     1395 2023-05-04 08:22:17.000000 headline_detector-1.0.2/src/headline_detector/preprocessing_scenario.py
+drwxrwxrwx   0        0        0        0 2023-05-04 08:25:52.848200 headline_detector-1.0.2/src/headline_detector/processing_pipeline/
+-rw-rw-rw-   0        0        0      142 2023-05-02 11:08:45.000000 headline_detector-1.0.2/src/headline_detector/processing_pipeline/__init__.py
+-rw-rw-rw-   0        0        0     1758 2023-05-02 11:32:18.000000 headline_detector-1.0.2/src/headline_detector/processing_pipeline/pipeline.py
+-rw-rw-rw-   0        0        0     2256 2023-05-02 11:07:28.000000 headline_detector-1.0.2/src/headline_detector/processing_pipeline/processing_func.py
+-rw-rw-rw-   0        0        0     2821 2023-05-02 11:07:12.000000 headline_detector-1.0.2/src/headline_detector/processing_pipeline/stemmer.py
+-rw-rw-rw-   0        0        0      202 2023-05-02 10:42:33.000000 headline_detector-1.0.2/src/headline_detector/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-04 08:25:52.843200 headline_detector-1.0.2/src/headline_detector.egg-info/
+-rw-rw-rw-   0        0        0     2729 2023-05-04 08:25:52.000000 headline_detector-1.0.2/src/headline_detector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      722 2023-05-04 08:25:52.000000 headline_detector-1.0.2/src/headline_detector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 08:25:52.000000 headline_detector-1.0.2/src/headline_detector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2023-05-04 08:25:52.000000 headline_detector-1.0.2/src/headline_detector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-04 08:25:52.000000 headline_detector-1.0.2/src/headline_detector.egg-info/top_level.txt
```

### Comparing `headline_detector-1.0.1/PKG-INFO` & `headline_detector-1.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,84 +1,81 @@
 Metadata-Version: 2.1
 Name: headline_detector
-Version: 1.0.1
+Version: 1.0.2
 Summary: An Indonesian Headline Detection Python API.
-Home-page: UNKNOWN
 Author: Kaenova Mahendra Auditama
 Author-email: kaenova@gmail.com
-License: UNKNOWN
-Description: # [headline_detector](https://github.com/kaenova/headline_detector)
-        
-        _Indonesian Headline Detection Python API_
-        
-        This is a Python library that provides APIs for detecting headlines in textual data, especially on social media platforms such as Twitter. The library utilizes a model that has been developed and trained on a dataset of Twitter posts containing both headline and non-headline texts, with the assistance of journalism professionals to ensure the data quality.
-        
-        ```sh
-        $ pip install headline-detector
-        ```
-        
-        ## Available scenario and the performance
-        
-        | Model        | Scenario 1 | Scenario 2 | Scenario 3 | Scenario 4 | Scenario 5 | Scenario 6 |
-        | ------------ | ---------- | ---------- | ---------- | ---------- | ---------- | ---------- |
-        | Fasttext     | 0.8766     | 0.8714     | 0.8793     | 0.8714     | 0.8714     | 0.8661     |
-        | CNN          | 0.9081     | 0.9081     | 0.8950     | 0.8898     | 0.8950     | 0.8898     |
-        | IndoBERTweet | 0.9895     | 0.9921     | 0.9738     | 0.9580     | 0.9843     | 0.9685     |
-        
-        All meassured in accuracy
-        
-        ### Model Throughput
-        
-        | Model        | Throughput (Â± Text/seconds) |
-        | ------------ | --------------------------- |
-        | IndoBERTweet | Â±1.3                        |
-        | CNN          | Â±281.60                     |
-        | Fasttext     | Â±2048.41                    |
-        
-        Tested on Intel i7-6700k and 32GB of RAM.
-        
-        ## Usage
-        
-        Output either 0 (non-headline) and 1 (headline)
-        
-        ```python
-        from headline_detector import FasttextDetector, IndoBERTweetDetector, CNNDetector
-        
-        detector = FasttextDetector.load_from_scenario(1)
-        data = detector.predict_text(
-            [
-                "nama kamu siapa?",
-                "Kapolda Jatim Teddy Minahasa Dikabarkan Ditangkap Terkait Narkoba  https://t.co/LD9X6VFaUR",
-            ]
-        )
-        print(data)  # output: [0, 1]
-        
-        detector = CNNDetector.load_from_scenario(3)
-        data = detector.predict_text(
-            [
-                "nama kamu siapa?",
-                "Kapolda Jatim Teddy Minahasa Dikabarkan Ditangkap Terkait Narkoba  https://t.co/LD9X6VFaUR",
-            ]
-        )
-        print(data)  # output: [0, 1]
-        
-        detector = IndoBERTweetDetector.load_from_scenario(5)
-        data = detector.predict_text(
-            [
-                "nama kamu siapa?",
-                "Kapolda Jatim Teddy Minahasa Dikabarkan Ditangkap Terkait Narkoba  https://t.co/LD9X6VFaUR",
-            ]
-        )
-        print(data)  # output: [0, 1]
-        
-        # 0 is non-headline
-        # 1 is headline
-        ```
-        
-        ## Paper
-        
-        Coming soon.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+
+# [headline_detector](https://github.com/kaenova/headline_detector)
+
+_Indonesian Headline Detection Python API_
+
+This is a Python library that provides APIs for detecting headlines in textual data, especially on social media platforms such as Twitter. The library utilizes a model that has been developed and trained on a dataset of Twitter posts containing both headline and non-headline texts, with the assistance of journalism professionals to ensure the data quality.
+
+```sh
+$ pip install headline-detector
+```
+
+## Available scenario and the performance
+
+| Model        | Scenario 1 | Scenario 2 | Scenario 3 | Scenario 4 | Scenario 5 | Scenario 6 |
+| ------------ | ---------- | ---------- | ---------- | ---------- | ---------- | ---------- |
+| Fasttext     | 0.8766     | 0.8714     | 0.8793     | 0.8714     | 0.8714     | 0.8661     |
+| CNN          | 0.9081     | 0.9081     | 0.8950     | 0.8898     | 0.8950     | 0.8898     |
+| IndoBERTweet | 0.9895     | 0.9921     | 0.9738     | 0.9580     | 0.9843     | 0.9685     |
+
+All meassured in accuracy
+
+### Model Throughput
+
+| Model        | Throughput (Â± Text/seconds) |
+| ------------ | --------------------------- |
+| IndoBERTweet | Â±1.3                        |
+| CNN          | Â±281.60                     |
+| Fasttext     | Â±2048.41                    |
+
+Tested on Intel i7-6700k and 32GB of RAM.
+
+## Usage
+
+Output either 0 (non-headline) and 1 (headline)
+
+```python
+from headline_detector import FasttextDetector, IndoBERTweetDetector, CNNDetector
+
+detector = FasttextDetector.load_from_scenario(1)
+data = detector.predict_text(
+    [
+        "nama kamu siapa?",
+        "Kapolda Jatim Teddy Minahasa Dikabarkan Ditangkap Terkait Narkoba  https://t.co/LD9X6VFaUR",
+    ]
+)
+print(data)  # output: [0, 1]
+
+detector = CNNDetector.load_from_scenario(3)
+data = detector.predict_text(
+    [
+        "nama kamu siapa?",
+        "Kapolda Jatim Teddy Minahasa Dikabarkan Ditangkap Terkait Narkoba  https://t.co/LD9X6VFaUR",
+    ]
+)
+print(data)  # output: [0, 1]
+
+detector = IndoBERTweetDetector.load_from_scenario(5)
+data = detector.predict_text(
+    [
+        "nama kamu siapa?",
+        "Kapolda Jatim Teddy Minahasa Dikabarkan Ditangkap Terkait Narkoba  https://t.co/LD9X6VFaUR",
+    ]
+)
+print(data)  # output: [0, 1]
+
+# 0 is non-headline
+# 1 is headline
+```
+
+## Paper
+
+Coming soon.
```

### Comparing `headline_detector-1.0.1/README.md` & `headline_detector-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `headline_detector-1.0.1/setup.py` & `headline_detector-1.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,23 @@
 import setuptools
-
 from pathlib import Path
+
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
+requirements = (this_directory / "requirements.txt").read_text().split("\n")
 
 setuptools.setup(
     name = "headline_detector",
-    version = "1.0.1",
+    version = "1.0.2",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = "Kaenova Mahendra Auditama",
     author_email = "kaenova@gmail.com",
     description = "An Indonesian Headline Detection Python API.",
     classifiers = [
         "Programming Language :: Python :: 3",
     ],
     package_dir = {"": "src"},
     packages = setuptools.find_packages(where="src"),
     python_requires = ">=3.8",
-    install_requires=[
-        "transformers",
-        "torch",
-        "lightning",
-        "pytorch-nlp",
-        "huggingface_hub",
-        "numpy",
-        "emoji",
-        "NDETCStemmer-kaenova"
-    ]
+    install_requires=requirements
 )
```

### Comparing `headline_detector-1.0.1/src/headline_detector/detector.py` & `headline_detector-1.0.2/src/headline_detector/detector.py`

 * *Files identical despite different names*

### Comparing `headline_detector-1.0.1/src/headline_detector/model.py` & `headline_detector-1.0.2/src/headline_detector/model.py`

 * *Files identical despite different names*

### Comparing `headline_detector-1.0.1/src/headline_detector/model_checkpoint.py` & `headline_detector-1.0.2/src/headline_detector/model_checkpoint.py`

 * *Files identical despite different names*

### Comparing `headline_detector-1.0.1/src/headline_detector/processing_pipeline/pipeline.py` & `headline_detector-1.0.2/src/headline_detector/processing_pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `headline_detector-1.0.1/src/headline_detector/processing_pipeline/processing_func.py` & `headline_detector-1.0.2/src/headline_detector/processing_pipeline/processing_func.py`

 * *Files identical despite different names*

### Comparing `headline_detector-1.0.1/src/headline_detector/processing_pipeline/stemmer.py` & `headline_detector-1.0.2/src/headline_detector/processing_pipeline/stemmer.py`

 * *Files identical despite different names*

### Comparing `headline_detector-1.0.1/src/headline_detector.egg-info/PKG-INFO` & `headline_detector-1.0.2/src/headline_detector.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,84 +1,81 @@
 Metadata-Version: 2.1
 Name: headline-detector
-Version: 1.0.1
+Version: 1.0.2
 Summary: An Indonesian Headline Detection Python API.
-Home-page: UNKNOWN
 Author: Kaenova Mahendra Auditama
 Author-email: kaenova@gmail.com
-License: UNKNOWN
-Description: # [headline_detector](https://github.com/kaenova/headline_detector)
-        
-        _Indonesian Headline Detection Python API_
-        
-        This is a Python library that provides APIs for detecting headlines in textual data, especially on social media platforms such as Twitter. The library utilizes a model that has been developed and trained on a dataset of Twitter posts containing both headline and non-headline texts, with the assistance of journalism professionals to ensure the data quality.
-        
-        ```sh
-        $ pip install headline-detector
-        ```
-        
-        ## Available scenario and the performance
-        
-        | Model        | Scenario 1 | Scenario 2 | Scenario 3 | Scenario 4 | Scenario 5 | Scenario 6 |
-        | ------------ | ---------- | ---------- | ---------- | ---------- | ---------- | ---------- |
-        | Fasttext     | 0.8766     | 0.8714     | 0.8793     | 0.8714     | 0.8714     | 0.8661     |
-        | CNN          | 0.9081     | 0.9081     | 0.8950     | 0.8898     | 0.8950     | 0.8898     |
-        | IndoBERTweet | 0.9895     | 0.9921     | 0.9738     | 0.9580     | 0.9843     | 0.9685     |
-        
-        All meassured in accuracy
-        
-        ### Model Throughput
-        
-        | Model        | Throughput (Â± Text/seconds) |
-        | ------------ | --------------------------- |
-        | IndoBERTweet | Â±1.3                        |
-        | CNN          | Â±281.60                     |
-        | Fasttext     | Â±2048.41                    |
-        
-        Tested on Intel i7-6700k and 32GB of RAM.
-        
-        ## Usage
-        
-        Output either 0 (non-headline) and 1 (headline)
-        
-        ```python
-        from headline_detector import FasttextDetector, IndoBERTweetDetector, CNNDetector
-        
-        detector = FasttextDetector.load_from_scenario(1)
-        data = detector.predict_text(
-            [
-                "nama kamu siapa?",
-                "Kapolda Jatim Teddy Minahasa Dikabarkan Ditangkap Terkait Narkoba  https://t.co/LD9X6VFaUR",
-            ]
-        )
-        print(data)  # output: [0, 1]
-        
-        detector = CNNDetector.load_from_scenario(3)
-        data = detector.predict_text(
-            [
-                "nama kamu siapa?",
-                "Kapolda Jatim Teddy Minahasa Dikabarkan Ditangkap Terkait Narkoba  https://t.co/LD9X6VFaUR",
-            ]
-        )
-        print(data)  # output: [0, 1]
-        
-        detector = IndoBERTweetDetector.load_from_scenario(5)
-        data = detector.predict_text(
-            [
-                "nama kamu siapa?",
-                "Kapolda Jatim Teddy Minahasa Dikabarkan Ditangkap Terkait Narkoba  https://t.co/LD9X6VFaUR",
-            ]
-        )
-        print(data)  # output: [0, 1]
-        
-        # 0 is non-headline
-        # 1 is headline
-        ```
-        
-        ## Paper
-        
-        Coming soon.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+
+# [headline_detector](https://github.com/kaenova/headline_detector)
+
+_Indonesian Headline Detection Python API_
+
+This is a Python library that provides APIs for detecting headlines in textual data, especially on social media platforms such as Twitter. The library utilizes a model that has been developed and trained on a dataset of Twitter posts containing both headline and non-headline texts, with the assistance of journalism professionals to ensure the data quality.
+
+```sh
+$ pip install headline-detector
+```
+
+## Available scenario and the performance
+
+| Model        | Scenario 1 | Scenario 2 | Scenario 3 | Scenario 4 | Scenario 5 | Scenario 6 |
+| ------------ | ---------- | ---------- | ---------- | ---------- | ---------- | ---------- |
+| Fasttext     | 0.8766     | 0.8714     | 0.8793     | 0.8714     | 0.8714     | 0.8661     |
+| CNN          | 0.9081     | 0.9081     | 0.8950     | 0.8898     | 0.8950     | 0.8898     |
+| IndoBERTweet | 0.9895     | 0.9921     | 0.9738     | 0.9580     | 0.9843     | 0.9685     |
+
+All meassured in accuracy
+
+### Model Throughput
+
+| Model        | Throughput (Â± Text/seconds) |
+| ------------ | --------------------------- |
+| IndoBERTweet | Â±1.3                        |
+| CNN          | Â±281.60                     |
+| Fasttext     | Â±2048.41                    |
+
+Tested on Intel i7-6700k and 32GB of RAM.
+
+## Usage
+
+Output either 0 (non-headline) and 1 (headline)
+
+```python
+from headline_detector import FasttextDetector, IndoBERTweetDetector, CNNDetector
+
+detector = FasttextDetector.load_from_scenario(1)
+data = detector.predict_text(
+    [
+        "nama kamu siapa?",
+        "Kapolda Jatim Teddy Minahasa Dikabarkan Ditangkap Terkait Narkoba  https://t.co/LD9X6VFaUR",
+    ]
+)
+print(data)  # output: [0, 1]
+
+detector = CNNDetector.load_from_scenario(3)
+data = detector.predict_text(
+    [
+        "nama kamu siapa?",
+        "Kapolda Jatim Teddy Minahasa Dikabarkan Ditangkap Terkait Narkoba  https://t.co/LD9X6VFaUR",
+    ]
+)
+print(data)  # output: [0, 1]
+
+detector = IndoBERTweetDetector.load_from_scenario(5)
+data = detector.predict_text(
+    [
+        "nama kamu siapa?",
+        "Kapolda Jatim Teddy Minahasa Dikabarkan Ditangkap Terkait Narkoba  https://t.co/LD9X6VFaUR",
+    ]
+)
+print(data)  # output: [0, 1]
+
+# 0 is non-headline
+# 1 is headline
+```
+
+## Paper
+
+Coming soon.
```

### Comparing `headline_detector-1.0.1/src/headline_detector.egg-info/SOURCES.txt` & `headline_detector-1.0.2/src/headline_detector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

