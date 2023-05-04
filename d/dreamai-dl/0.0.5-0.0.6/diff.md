# Comparing `tmp/dreamai_dl-0.0.5.tar.gz` & `tmp/dreamai_dl-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dreamai_dl-0.0.5.tar", last modified: Wed May  3 21:10:49 2023, max compression
+gzip compressed data, was "dreamai_dl-0.0.6.tar", last modified: Thu May  4 00:29:08 2023, max compression
```

## Comparing `dreamai_dl-0.0.5.tar` & `dreamai_dl-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-03 21:10:49.252658 dreamai_dl-0.0.5/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)    11337 2023-04-27 10:12:58.000000 dreamai_dl-0.0.5/LICENSE
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      111 2023-04-27 10:12:58.000000 dreamai_dl-0.0.5/MANIFEST.in
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      919 2023-05-03 21:10:49.252658 dreamai_dl-0.0.5/PKG-INFO
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      136 2023-05-02 16:23:03.000000 dreamai_dl-0.0.5/README.md
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-03 21:10:49.252658 dreamai_dl-0.0.5/dreamai_dl/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       22 2023-05-03 21:10:43.000000 dreamai_dl-0.0.5/dreamai_dl/__init__.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      708 2023-05-03 21:10:43.000000 dreamai_dl-0.0.5/dreamai_dl/_modidx.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      165 2023-05-03 21:10:43.000000 dreamai_dl-0.0.5/dreamai_dl/core.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      690 2023-05-02 21:02:32.000000 dreamai_dl-0.0.5/dreamai_dl/imports.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      724 2023-05-03 21:10:43.000000 dreamai_dl-0.0.5/dreamai_dl/utils.py
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-03 21:10:49.252658 dreamai_dl-0.0.5/dreamai_dl.egg-info/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      919 2023-05-03 21:10:49.000000 dreamai_dl-0.0.5/dreamai_dl.egg-info/PKG-INFO
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      396 2023-05-03 21:10:49.000000 dreamai_dl-0.0.5/dreamai_dl.egg-info/SOURCES.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-05-03 21:10:49.000000 dreamai_dl-0.0.5/dreamai_dl.egg-info/dependency_links.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       42 2023-05-03 21:10:49.000000 dreamai_dl-0.0.5/dreamai_dl.egg-info/entry_points.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-05-01 22:18:59.000000 dreamai_dl-0.0.5/dreamai_dl.egg-info/not-zip-safe
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     2185 2023-05-03 21:10:49.000000 dreamai_dl-0.0.5/dreamai_dl.egg-info/requires.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       11 2023-05-03 21:10:49.000000 dreamai_dl-0.0.5/dreamai_dl.egg-info/top_level.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     2864 2023-05-03 21:10:31.000000 dreamai_dl-0.0.5/settings.ini
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       38 2023-05-03 21:10:49.252658 dreamai_dl-0.0.5/setup.cfg
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     2596 2023-04-27 10:12:58.000000 dreamai_dl-0.0.5/setup.py
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-04 00:29:08.727478 dreamai_dl-0.0.6/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)    11337 2023-04-27 10:12:58.000000 dreamai_dl-0.0.6/LICENSE
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      111 2023-04-27 10:12:58.000000 dreamai_dl-0.0.6/MANIFEST.in
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      919 2023-05-04 00:29:08.727478 dreamai_dl-0.0.6/PKG-INFO
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      136 2023-05-02 16:23:03.000000 dreamai_dl-0.0.6/README.md
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-04 00:29:08.727478 dreamai_dl-0.0.6/dreamai_dl/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       22 2023-05-04 00:28:51.000000 dreamai_dl-0.0.6/dreamai_dl/__init__.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      708 2023-05-04 00:28:51.000000 dreamai_dl-0.0.6/dreamai_dl/_modidx.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      165 2023-05-04 00:28:51.000000 dreamai_dl-0.0.6/dreamai_dl/core.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      690 2023-05-02 21:02:32.000000 dreamai_dl-0.0.6/dreamai_dl/imports.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      724 2023-05-04 00:28:51.000000 dreamai_dl-0.0.6/dreamai_dl/utils.py
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-04 00:29:08.727478 dreamai_dl-0.0.6/dreamai_dl.egg-info/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      919 2023-05-04 00:29:08.000000 dreamai_dl-0.0.6/dreamai_dl.egg-info/PKG-INFO
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      396 2023-05-04 00:29:08.000000 dreamai_dl-0.0.6/dreamai_dl.egg-info/SOURCES.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-05-04 00:29:08.000000 dreamai_dl-0.0.6/dreamai_dl.egg-info/dependency_links.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       42 2023-05-04 00:29:08.000000 dreamai_dl-0.0.6/dreamai_dl.egg-info/entry_points.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-05-01 22:18:59.000000 dreamai_dl-0.0.6/dreamai_dl.egg-info/not-zip-safe
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     2185 2023-05-04 00:29:08.000000 dreamai_dl-0.0.6/dreamai_dl.egg-info/requires.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       11 2023-05-04 00:29:08.000000 dreamai_dl-0.0.6/dreamai_dl.egg-info/top_level.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     2864 2023-05-04 00:27:32.000000 dreamai_dl-0.0.6/settings.ini
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       38 2023-05-04 00:29:08.727478 dreamai_dl-0.0.6/setup.cfg
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     2596 2023-04-27 10:12:58.000000 dreamai_dl-0.0.6/setup.py
```

### Comparing `dreamai_dl-0.0.5/LICENSE` & `dreamai_dl-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dreamai_dl-0.0.5/PKG-INFO` & `dreamai_dl-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreamai_dl
-Version: 0.0.5
+Version: 0.0.6
 Summary: Deep Learning tools based on dreamai.
 Home-page: https://github.com/HamzaFarhan/dreamai_dl
 Author: HamzaFarhan
 Author-email: thehamza96@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dreamai_dl-0.0.5/dreamai_dl/_modidx.py` & `dreamai_dl-0.0.6/dreamai_dl/_modidx.py`

 * *Files identical despite different names*

### Comparing `dreamai_dl-0.0.5/dreamai_dl/imports.py` & `dreamai_dl-0.0.6/dreamai_dl/imports.py`

 * *Files identical despite different names*

### Comparing `dreamai_dl-0.0.5/dreamai_dl/utils.py` & `dreamai_dl-0.0.6/dreamai_dl/utils.py`

 * *Files identical despite different names*

### Comparing `dreamai_dl-0.0.5/dreamai_dl.egg-info/PKG-INFO` & `dreamai_dl-0.0.6/dreamai_dl.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreamai-dl
-Version: 0.0.5
+Version: 0.0.6
 Summary: Deep Learning tools based on dreamai.
 Home-page: https://github.com/HamzaFarhan/dreamai_dl
 Author: HamzaFarhan
 Author-email: thehamza96@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dreamai_dl-0.0.5/dreamai_dl.egg-info/requires.txt` & `dreamai_dl-0.0.6/dreamai_dl.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 multimethod==1.9.1
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
 phik==0.12.3
 pillow==9.5.0
 pkginfo==1.9.6
 preshed==3.0.8
 pydantic==1.10.7
```

### Comparing `dreamai_dl-0.0.5/settings.ini` & `dreamai_dl-0.0.6/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = dreamai_dl
 lib_name = %(repo)s
-version = 0.0.5
+version = 0.0.6
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = dreamai_dl
 nbs_path = nbs
 recursive = True
@@ -22,9 +22,9 @@
 author_email = thehamza96@gmail.com
 copyright = 2023 onwards, %(author)s
 description = Deep Learning tools based on dreamai.
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = HamzaFarhan
-pip_requirements = aiohttp==3.8.4 aiosignal==1.3.1 arrow==1.2.3 astunparse==1.6.3 async-timeout==4.0.2 blessed==1.20.0 blis==0.7.9 catalogue==2.0.8 certifi==2022.12.7 charset-normalizer==3.1.0 click==8.1.3 cmake==3.26.3 confection==0.0.4 contourpy==1.0.7 croniter==1.3.14 cryptography==40.0.2 cycler==0.11.0 cymem==2.0.7 dateutils==0.6.12 deepdiff==6.3.0 diskcache==5.6.1 docutils==0.19 dreamai==0.8.0 duckduckgo-search==2.9.1 execnb==0.1.5 fastai==2.7.12 fastapi==0.88.0 fastcore==1.5.29 fastdownload==0.0.7 fastprogress==1.0.3 filelock==3.12.0 fonttools==4.39.3 frozenlist==1.3.3 fsspec==2023.4.0 ghapi==1.0.3 h11==0.14.0 htmlmin==0.1.12 huggingface-hub==0.14.1 imagehash==4.3.1 importlib-metadata==6.6.0 imutils==0.5.4 inquirer==3.1.3 ipywidgets==8.0.6 itsdangerous==2.1.2 jaraco-classes==3.2.3 jeepney==0.8.0 joblib==1.1.1 jupyterlab-widgets==3.0.7 keyring==23.13.1 kiwisolver==1.4.4 langcodes==3.3.0 lightning==2.0.2 lightning-cloud==0.5.34 lightning-utilities==0.8.0 lit==16.0.2 markdown-it-py==2.2.0 matplotlib==3.7.1 mdurl==0.1.2 missingno==0.5.2 more-itertools==9.1.0 mpmath==1.3.0 multidict==6.0.4 multimethod==1.9.1 murmurhash==1.0.9 nbdev==2.3.12 networkx==3.1 numpy==1.24.3 opencv-python==4.7.0.72 ordered-set==4.1.0 pandas==2.0.1 pandas-profiling==3.2.0 pathy==0.10.1 phik==0.12.3 pillow==9.5.0 pkginfo==1.9.6 preshed==3.0.8 pydantic==1.10.7 pygments==2.15.1 pyjwt==2.6.0 pyparsing==3.0.9 python-editor==1.0.4 python-multipart==0.0.6 pytorch-lightning==2.0.2 pytz==2023.3 pywavelets==1.4.1 pyyaml==6.0 readchar==4.0.5 readme-renderer==37.3 requests==2.29.0 requests-toolbelt==1.0.0 rfc3986==2.0.0 rich==13.3.5 scikit-learn==1.2.2 scipy==1.10.1 seaborn==0.12.2 secretstorage==3.3.3 smart-open==6.3.0 spacy==3.5.2 spacy-legacy==3.0.12 spacy-loggers==1.0.4 srsly==2.4.6 starlette==0.22.0 starsessions==1.3.0 sympy==1.11.1 tangled-up-in-unicode==0.2.0 thinc==8.1.9 threadpoolctl==3.1.0 timm==0.6.13 torch==2.0.0 torchaudio==2.0.1 torchmetrics==0.11.4 torchvision==0.15.1 tqdm==4.65.0 triton==2.0.0 twine==4.0.2 typer==0.7.0 tzdata==2023.3 urllib3==1.26.15 uvicorn==0.22.0 visions==0.7.4 wasabi==1.1.1 watchdog==3.0.0 websockets==11.0.2 widgetsnbextension==4.0.7 yarl==1.9.2 zipp==3.15.0
+pip_requirements = aiohttp==3.8.4 aiosignal==1.3.1 arrow==1.2.3 astunparse==1.6.3 async-timeout==4.0.2 blessed==1.20.0 blis==0.7.9 catalogue==2.0.8 certifi==2022.12.7 charset-normalizer==3.1.0 click==8.1.3 cmake==3.26.3 confection==0.0.4 contourpy==1.0.7 croniter==1.3.14 cryptography==40.0.2 cycler==0.11.0 cymem==2.0.7 dateutils==0.6.12 deepdiff==6.3.0 diskcache==5.6.1 docutils==0.19 dreamai==0.8.0 duckduckgo-search==2.9.1 execnb==0.1.5 fastai==2.7.12 fastapi==0.88.0 fastcore==1.5.29 fastdownload==0.0.7 fastprogress==1.0.3 filelock==3.12.0 fonttools==4.39.3 frozenlist==1.3.3 fsspec==2023.4.0 ghapi==1.0.3 h11==0.14.0 htmlmin==0.1.12 huggingface-hub==0.14.1 imagehash==4.3.1 importlib-metadata==6.6.0 imutils==0.5.4 inquirer==3.1.3 ipywidgets==8.0.6 itsdangerous==2.1.2 jaraco-classes==3.2.3 jeepney==0.8.0 joblib==1.1.1 jupyterlab-widgets==3.0.7 keyring==23.13.1 kiwisolver==1.4.4 langcodes==3.3.0 lightning==2.0.2 lightning-cloud==0.5.34 lightning-utilities==0.8.0 lit==16.0.2 markdown-it-py==2.2.0 matplotlib==3.7.1 mdurl==0.1.2 missingno==0.5.2 more-itertools==9.1.0 mpmath==1.3.0 multidict==6.0.4 multimethod==1.9.1 murmurhash==1.0.9 nbdev==2.3.12 networkx==3.1 numpy==1.24.3 opencv-python==4.7.0.72 ordered-set==4.1.0 pandas==1.5.3 pandas-profiling==3.2.0 pathy==0.10.1 phik==0.12.3 pillow==9.5.0 pkginfo==1.9.6 preshed==3.0.8 pydantic==1.10.7 pygments==2.15.1 pyjwt==2.6.0 pyparsing==3.0.9 python-editor==1.0.4 python-multipart==0.0.6 pytorch-lightning==2.0.2 pytz==2023.3 pywavelets==1.4.1 pyyaml==6.0 readchar==4.0.5 readme-renderer==37.3 requests==2.29.0 requests-toolbelt==1.0.0 rfc3986==2.0.0 rich==13.3.5 scikit-learn==1.2.2 scipy==1.10.1 seaborn==0.12.2 secretstorage==3.3.3 smart-open==6.3.0 spacy==3.5.2 spacy-legacy==3.0.12 spacy-loggers==1.0.4 srsly==2.4.6 starlette==0.22.0 starsessions==1.3.0 sympy==1.11.1 tangled-up-in-unicode==0.2.0 thinc==8.1.9 threadpoolctl==3.1.0 timm==0.6.13 torch==2.0.0 torchaudio==2.0.1 torchmetrics==0.11.4 torchvision==0.15.1 tqdm==4.65.0 triton==2.0.0 twine==4.0.2 typer==0.7.0 tzdata==2023.3 urllib3==1.26.15 uvicorn==0.22.0 visions==0.7.4 wasabi==1.1.1 watchdog==3.0.0 websockets==11.0.2 widgetsnbextension==4.0.7 yarl==1.9.2 zipp==3.15.0
```

### Comparing `dreamai_dl-0.0.5/setup.py` & `dreamai_dl-0.0.6/setup.py`

 * *Files identical despite different names*

