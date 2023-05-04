# Comparing `tmp/dreamai_pdf-0.0.7.tar.gz` & `tmp/dreamai_pdf-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dreamai_pdf-0.0.7.tar", last modified: Wed May  3 23:24:13 2023, max compression
+gzip compressed data, was "dreamai_pdf-0.0.8.tar", last modified: Thu May  4 00:32:55 2023, max compression
```

## Comparing `dreamai_pdf-0.0.7.tar` & `dreamai_pdf-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-03 23:24:13.956343 dreamai_pdf-0.0.7/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)    11337 2023-04-27 10:12:58.000000 dreamai_pdf-0.0.7/LICENSE
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      111 2023-04-27 10:12:58.000000 dreamai_pdf-0.0.7/MANIFEST.in
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      927 2023-05-03 23:24:13.956343 dreamai_pdf-0.0.7/PKG-INFO
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      138 2023-05-02 22:37:14.000000 dreamai_pdf-0.0.7/README.md
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-03 23:24:13.956343 dreamai_pdf-0.0.7/dreamai_pdf/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       22 2023-05-03 21:14:31.000000 dreamai_pdf-0.0.7/dreamai_pdf/__init__.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     5569 2023-05-03 21:14:31.000000 dreamai_pdf-0.0.7/dreamai_pdf/_modidx.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     3434 2023-05-03 21:14:31.000000 dreamai_pdf-0.0.7/dreamai_pdf/core.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      494 2023-05-02 20:33:15.000000 dreamai_pdf-0.0.7/dreamai_pdf/imports.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     9207 2023-05-03 21:14:31.000000 dreamai_pdf-0.0.7/dreamai_pdf/parse.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     2285 2023-05-03 21:14:31.000000 dreamai_pdf-0.0.7/dreamai_pdf/segment.py
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-03 23:24:13.956343 dreamai_pdf-0.0.7/dreamai_pdf.egg-info/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      927 2023-05-03 23:24:13.000000 dreamai_pdf-0.0.7/dreamai_pdf.egg-info/PKG-INFO
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      431 2023-05-03 23:24:13.000000 dreamai_pdf-0.0.7/dreamai_pdf.egg-info/SOURCES.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-05-03 23:24:13.000000 dreamai_pdf-0.0.7/dreamai_pdf.egg-info/dependency_links.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       44 2023-05-03 23:24:13.000000 dreamai_pdf-0.0.7/dreamai_pdf.egg-info/entry_points.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-04-28 14:00:17.000000 dreamai_pdf-0.0.7/dreamai_pdf.egg-info/not-zip-safe
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     2951 2023-05-03 23:24:13.000000 dreamai_pdf-0.0.7/dreamai_pdf.egg-info/requires.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       12 2023-05-03 23:24:13.000000 dreamai_pdf-0.0.7/dreamai_pdf.egg-info/top_level.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     3636 2023-05-03 21:12:49.000000 dreamai_pdf-0.0.7/settings.ini
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       38 2023-05-03 23:24:13.956343 dreamai_pdf-0.0.7/setup.cfg
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     2596 2023-04-27 10:12:58.000000 dreamai_pdf-0.0.7/setup.py
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-04 00:32:55.475934 dreamai_pdf-0.0.8/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)    11337 2023-04-27 10:12:58.000000 dreamai_pdf-0.0.8/LICENSE
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      111 2023-04-27 10:12:58.000000 dreamai_pdf-0.0.8/MANIFEST.in
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      927 2023-05-04 00:32:55.475934 dreamai_pdf-0.0.8/PKG-INFO
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      138 2023-05-02 22:37:14.000000 dreamai_pdf-0.0.8/README.md
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-04 00:32:55.475934 dreamai_pdf-0.0.8/dreamai_pdf/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       22 2023-05-04 00:32:44.000000 dreamai_pdf-0.0.8/dreamai_pdf/__init__.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     5569 2023-05-04 00:32:44.000000 dreamai_pdf-0.0.8/dreamai_pdf/_modidx.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     3434 2023-05-04 00:32:44.000000 dreamai_pdf-0.0.8/dreamai_pdf/core.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      494 2023-05-02 20:33:15.000000 dreamai_pdf-0.0.8/dreamai_pdf/imports.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     9207 2023-05-04 00:32:44.000000 dreamai_pdf-0.0.8/dreamai_pdf/parse.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     2285 2023-05-04 00:32:44.000000 dreamai_pdf-0.0.8/dreamai_pdf/segment.py
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-04 00:32:55.475934 dreamai_pdf-0.0.8/dreamai_pdf.egg-info/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      927 2023-05-04 00:32:55.000000 dreamai_pdf-0.0.8/dreamai_pdf.egg-info/PKG-INFO
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      431 2023-05-04 00:32:55.000000 dreamai_pdf-0.0.8/dreamai_pdf.egg-info/SOURCES.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-05-04 00:32:55.000000 dreamai_pdf-0.0.8/dreamai_pdf.egg-info/dependency_links.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       44 2023-05-04 00:32:55.000000 dreamai_pdf-0.0.8/dreamai_pdf.egg-info/entry_points.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-04-28 14:00:17.000000 dreamai_pdf-0.0.8/dreamai_pdf.egg-info/not-zip-safe
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     2951 2023-05-04 00:32:55.000000 dreamai_pdf-0.0.8/dreamai_pdf.egg-info/requires.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       12 2023-05-04 00:32:55.000000 dreamai_pdf-0.0.8/dreamai_pdf.egg-info/top_level.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     3636 2023-05-04 00:30:45.000000 dreamai_pdf-0.0.8/settings.ini
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       38 2023-05-04 00:32:55.475934 dreamai_pdf-0.0.8/setup.cfg
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     2596 2023-04-27 10:12:58.000000 dreamai_pdf-0.0.8/setup.py
```

### Comparing `dreamai_pdf-0.0.7/LICENSE` & `dreamai_pdf-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dreamai_pdf-0.0.7/PKG-INFO` & `dreamai_pdf-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreamai_pdf
-Version: 0.0.7
+Version: 0.0.8
 Summary: Library based on dreamai for parsing PDFs
 Home-page: https://github.com/HamzaFarhan/dreamai_pdf
 Author: HamzaFarhan
 Author-email: thehamza96@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dreamai_pdf-0.0.7/dreamai_pdf/_modidx.py` & `dreamai_pdf-0.0.8/dreamai_pdf/_modidx.py`

 * *Files identical despite different names*

### Comparing `dreamai_pdf-0.0.7/dreamai_pdf/core.py` & `dreamai_pdf-0.0.8/dreamai_pdf/core.py`

 * *Files identical despite different names*

### Comparing `dreamai_pdf-0.0.7/dreamai_pdf/parse.py` & `dreamai_pdf-0.0.8/dreamai_pdf/parse.py`

 * *Files identical despite different names*

### Comparing `dreamai_pdf-0.0.7/dreamai_pdf/segment.py` & `dreamai_pdf-0.0.8/dreamai_pdf/segment.py`

 * *Files identical despite different names*

### Comparing `dreamai_pdf-0.0.7/dreamai_pdf.egg-info/PKG-INFO` & `dreamai_pdf-0.0.8/dreamai_pdf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreamai-pdf
-Version: 0.0.7
+Version: 0.0.8
 Summary: Library based on dreamai for parsing PDFs
 Home-page: https://github.com/HamzaFarhan/dreamai_pdf
 Author: HamzaFarhan
 Author-email: thehamza96@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dreamai_pdf-0.0.7/dreamai_pdf.egg-info/requires.txt` & `dreamai_pdf-0.0.8/dreamai_pdf.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 dateutils==0.6.12
 deepdiff==6.3.0
 deprecated==1.2.13
 dill==0.3.6
 diskcache==5.6.1
 docutils==0.19
 dreamai==0.8.0
-dreamai-dl==0.0.5
+dreamai-dl==0.0.6
 duckduckgo-search==2.9.1
 execnb==0.1.5
 faiss-cpu==1.7.4
 fastai==2.7.12
 fastapi==0.88.0
 fastcore==1.5.29
 fastdownload==0.0.7
@@ -84,15 +84,15 @@
 multiprocess==0.70.14
 murmurhash==1.0.9
 nbdev==2.3.12
 networkx==3.1
 numpy==1.24.3
 opencv-python==4.7.0.72
 ordered-set==4.1.0
-pandas==2.0.1
+pandas==1.5.3
 pandas-profiling==3.2.0
 pathy==0.10.1
 pdfminer-six==20221105
 pdfplumber==0.9.0
 phik==0.12.3
 pillow==9.5.0
 pkginfo==1.9.6
```

### Comparing `dreamai_pdf-0.0.7/settings.ini` & `dreamai_pdf-0.0.8/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = dreamai_pdf
 lib_name = %(repo)s
-version = 0.0.7
+version = 0.0.8
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = dreamai_pdf
 nbs_path = nbs
 recursive = True
@@ -22,9 +22,9 @@
 author_email = thehamza96@gmail.com
 copyright = 2023 onwards, %(author)s
 description = Library based on dreamai for parsing PDFs
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = HamzaFarhan
-pip_requirements = aiohttp==3.8.4 aiosignal==1.3.1 arrow==1.2.3 astunparse==1.6.3 async-timeout==4.0.2 blessed==1.20.0 blis==0.7.9 boto3==1.26.122 botocore==1.29.122 bpemb==0.3.4 catalogue==2.0.8 certifi==2022.12.7 charset-normalizer==3.1.0 click==8.1.3 cloudpickle==2.2.1 cmake==3.26.3 confection==0.0.4 conllu==4.5.2 contourpy==1.0.7 croniter==1.3.14 cryptography==40.0.2 cycler==0.11.0 cymem==2.0.7 datasets==2.12.0 dateutils==0.6.12 deepdiff==6.3.0 deprecated==1.2.13 dill==0.3.6 diskcache==5.6.1 docutils==0.19 dreamai==0.8.0 dreamai-dl==0.0.5 duckduckgo-search==2.9.1 execnb==0.1.5 faiss-cpu==1.7.4 fastai==2.7.12 fastapi==0.88.0 fastcore==1.5.29 fastdownload==0.0.7 fastprogress==1.0.3 filelock==3.12.0 flair==0.12.2 fonttools==4.39.3 frozenlist==1.3.3 fsspec==2023.4.0 ftfy==6.1.1 future==0.18.3 gdown==4.4.0 gensim==4.3.1 ghapi==1.0.3 h11==0.14.0 htmlmin==0.1.12 huggingface-hub==0.14.1 hyperopt==0.2.7 imagehash==4.3.1 importlib-metadata==6.6.0 imutils==0.5.4 inquirer==3.1.3 ipywidgets==8.0.6 itsdangerous==2.1.2 janome==0.4.2 jaraco-classes==3.2.3 jeepney==0.8.0 jmespath==1.0.1 joblib==1.1.1 jupyterlab-widgets==3.0.7 keyring==23.13.1 kiwisolver==1.4.4 langcodes==3.3.0 langdetect==1.0.9 lightning==2.0.2 lightning-cloud==0.5.34 lightning-utilities==0.8.0 lit==16.0.2 markdown-it-py==2.2.0 matplotlib==3.7.1 mdurl==0.1.2 missingno==0.5.2 more-itertools==9.1.0 mpld3==0.3 mpmath==1.3.0 multidict==6.0.4 multimethod==1.9.1 multiprocess==0.70.14 murmurhash==1.0.9 nbdev==2.3.12 networkx==3.1 numpy==1.24.3 opencv-python==4.7.0.72 ordered-set==4.1.0 pandas==2.0.1 pandas-profiling==3.2.0 pathy==0.10.1 pdfminer-six==20221105 pdfplumber==0.9.0 phik==0.12.3 pillow==9.5.0 pkginfo==1.9.6 pptree==3.1 preshed==3.0.8 protobuf==3.20.2 py4j==0.10.9.7 pyarrow==11.0.0 pydantic==1.10.7 pygments==2.15.1 pyjwt==2.6.0 pyparsing==3.0.9 pysocks==1.7.1 python-editor==1.0.4 python-multipart==0.0.6 pytorch-lightning==2.0.2 pytorch-revgrad==0.2.0 pytz==2023.3 pywavelets==1.4.1 pyyaml==6.0 readchar==4.0.5 readme-renderer==37.3 regex==2023.3.23 requests==2.29.0 requests-toolbelt==1.0.0 responses==0.18.0 rfc3986==2.0.0 rich==13.3.5 s3transfer==0.6.0 scikit-learn==1.2.2 scipy==1.10.1 seaborn==0.12.2 secretstorage==3.3.3 segtok==1.5.11 sentencepiece==0.1.98 smart-open==6.3.0 spacy==3.5.2 spacy-legacy==3.0.12 spacy-loggers==1.0.4 sqlitedict==2.1.0 srsly==2.4.6 starlette==0.22.0 starsessions==1.3.0 sympy==1.11.1 tabulate==0.9.0 tangled-up-in-unicode==0.2.0 thinc==8.1.9 threadpoolctl==3.1.0 timm==0.6.13 tokenizers==0.13.3 torch==2.0.0 torchaudio==2.0.1 torchmetrics==0.11.4 torchvision==0.15.1 tqdm==4.65.0 transformer-smaller-training-vocab==0.2.3 transformers==4.28.1 triton==2.0.0 twine==4.0.2 txtai==5.5.1 typer==0.7.0 tzdata==2023.3 urllib3==1.26.15 uvicorn==0.22.0 visions==0.7.4 wand==0.6.11 wasabi==1.1.1 watchdog==3.0.0 websockets==11.0.2 widgetsnbextension==4.0.7 wikipedia-api==0.5.8 wrapt==1.15.0 xxhash==3.2.0 yarl==1.9.2 yellowbrick==1.5 zipp==3.15.0
+pip_requirements = aiohttp==3.8.4 aiosignal==1.3.1 arrow==1.2.3 astunparse==1.6.3 async-timeout==4.0.2 blessed==1.20.0 blis==0.7.9 boto3==1.26.122 botocore==1.29.122 bpemb==0.3.4 catalogue==2.0.8 certifi==2022.12.7 charset-normalizer==3.1.0 click==8.1.3 cloudpickle==2.2.1 cmake==3.26.3 confection==0.0.4 conllu==4.5.2 contourpy==1.0.7 croniter==1.3.14 cryptography==40.0.2 cycler==0.11.0 cymem==2.0.7 datasets==2.12.0 dateutils==0.6.12 deepdiff==6.3.0 deprecated==1.2.13 dill==0.3.6 diskcache==5.6.1 docutils==0.19 dreamai==0.8.0 dreamai-dl==0.0.6 duckduckgo-search==2.9.1 execnb==0.1.5 faiss-cpu==1.7.4 fastai==2.7.12 fastapi==0.88.0 fastcore==1.5.29 fastdownload==0.0.7 fastprogress==1.0.3 filelock==3.12.0 flair==0.12.2 fonttools==4.39.3 frozenlist==1.3.3 fsspec==2023.4.0 ftfy==6.1.1 future==0.18.3 gdown==4.4.0 gensim==4.3.1 ghapi==1.0.3 h11==0.14.0 htmlmin==0.1.12 huggingface-hub==0.14.1 hyperopt==0.2.7 imagehash==4.3.1 importlib-metadata==6.6.0 imutils==0.5.4 inquirer==3.1.3 ipywidgets==8.0.6 itsdangerous==2.1.2 janome==0.4.2 jaraco-classes==3.2.3 jeepney==0.8.0 jmespath==1.0.1 joblib==1.1.1 jupyterlab-widgets==3.0.7 keyring==23.13.1 kiwisolver==1.4.4 langcodes==3.3.0 langdetect==1.0.9 lightning==2.0.2 lightning-cloud==0.5.34 lightning-utilities==0.8.0 lit==16.0.2 markdown-it-py==2.2.0 matplotlib==3.7.1 mdurl==0.1.2 missingno==0.5.2 more-itertools==9.1.0 mpld3==0.3 mpmath==1.3.0 multidict==6.0.4 multimethod==1.9.1 multiprocess==0.70.14 murmurhash==1.0.9 nbdev==2.3.12 networkx==3.1 numpy==1.24.3 opencv-python==4.7.0.72 ordered-set==4.1.0 pandas==1.5.3 pandas-profiling==3.2.0 pathy==0.10.1 pdfminer-six==20221105 pdfplumber==0.9.0 phik==0.12.3 pillow==9.5.0 pkginfo==1.9.6 pptree==3.1 preshed==3.0.8 protobuf==3.20.2 py4j==0.10.9.7 pyarrow==11.0.0 pydantic==1.10.7 pygments==2.15.1 pyjwt==2.6.0 pyparsing==3.0.9 pysocks==1.7.1 python-editor==1.0.4 python-multipart==0.0.6 pytorch-lightning==2.0.2 pytorch-revgrad==0.2.0 pytz==2023.3 pywavelets==1.4.1 pyyaml==6.0 readchar==4.0.5 readme-renderer==37.3 regex==2023.3.23 requests==2.29.0 requests-toolbelt==1.0.0 responses==0.18.0 rfc3986==2.0.0 rich==13.3.5 s3transfer==0.6.0 scikit-learn==1.2.2 scipy==1.10.1 seaborn==0.12.2 secretstorage==3.3.3 segtok==1.5.11 sentencepiece==0.1.98 smart-open==6.3.0 spacy==3.5.2 spacy-legacy==3.0.12 spacy-loggers==1.0.4 sqlitedict==2.1.0 srsly==2.4.6 starlette==0.22.0 starsessions==1.3.0 sympy==1.11.1 tabulate==0.9.0 tangled-up-in-unicode==0.2.0 thinc==8.1.9 threadpoolctl==3.1.0 timm==0.6.13 tokenizers==0.13.3 torch==2.0.0 torchaudio==2.0.1 torchmetrics==0.11.4 torchvision==0.15.1 tqdm==4.65.0 transformer-smaller-training-vocab==0.2.3 transformers==4.28.1 triton==2.0.0 twine==4.0.2 txtai==5.5.1 typer==0.7.0 tzdata==2023.3 urllib3==1.26.15 uvicorn==0.22.0 visions==0.7.4 wand==0.6.11 wasabi==1.1.1 watchdog==3.0.0 websockets==11.0.2 widgetsnbextension==4.0.7 wikipedia-api==0.5.8 wrapt==1.15.0 xxhash==3.2.0 yarl==1.9.2 yellowbrick==1.5 zipp==3.15.0
```

### Comparing `dreamai_pdf-0.0.7/setup.py` & `dreamai_pdf-0.0.8/setup.py`

 * *Files identical despite different names*

