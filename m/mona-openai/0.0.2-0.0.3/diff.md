# Comparing `tmp/mona-openai-0.0.2.tar.gz` & `tmp/mona-openai-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mona-openai-0.0.2.tar", last modified: Thu May  4 06:50:38 2023, max compression
+gzip compressed data, was "mona-openai-0.0.3.tar", last modified: Thu May  4 06:53:27 2023, max compression
```

## Comparing `mona-openai-0.0.2.tar` & `mona-openai-0.0.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-04 06:50:38.314731 mona-openai-0.0.2/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)    11356 2023-04-04 12:33:03.000000 mona-openai-0.0.2/LICENSE
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     8665 2023-05-04 06:50:38.314412 mona-openai-0.0.2/PKG-INFO
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     8071 2023-05-04 03:41:54.000000 mona-openai-0.0.2/README.md
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-04 06:50:38.312215 mona-openai-0.0.2/mona_openai/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)       77 2023-05-04 03:41:54.000000 mona-openai-0.0.2/mona_openai/__init__.py
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-04 06:50:38.313396 mona-openai-0.0.2/mona_openai/analysis/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     1192 2023-04-04 12:33:03.000000 mona-openai-0.0.2/mona_openai/analysis/analysis.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     2693 2023-04-04 12:33:03.000000 mona-openai-0.0.2/mona_openai/analysis/privacy.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      381 2023-04-04 12:33:03.000000 mona-openai-0.0.2/mona_openai/analysis/profanity.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     3748 2023-04-04 12:33:03.000000 mona-openai-0.0.2/mona_openai/analysis/textual.py
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-04 06:50:38.313512 mona-openai-0.0.2/mona_openai/endpoints/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     1786 2023-05-04 03:41:54.000000 mona-openai-0.0.2/mona_openai/endpoints/completion.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      167 2023-04-04 12:33:03.000000 mona-openai-0.0.2/mona_openai/exceptions.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     1379 2023-04-04 12:33:03.000000 mona-openai-0.0.2/mona_openai/mona_client.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)    13259 2023-05-04 03:41:54.000000 mona-openai-0.0.2/mona_openai/mona_openai.py
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-04 06:50:38.313856 mona-openai-0.0.2/mona_openai/util/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     1224 2023-04-04 12:33:03.000000 mona-openai-0.0.2/mona_openai/util/func_util.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      494 2023-04-04 12:33:03.000000 mona-openai-0.0.2/mona_openai/util/math.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      971 2023-04-04 12:33:03.000000 mona-openai-0.0.2/mona_openai/util/validation_util.py
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-04 06:50:38.312910 mona-openai-0.0.2/mona_openai.egg-info/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     8665 2023-05-04 06:50:38.000000 mona-openai-0.0.2/mona_openai.egg-info/PKG-INFO
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      610 2023-05-04 06:50:38.000000 mona-openai-0.0.2/mona_openai.egg-info/SOURCES.txt
--rw-r--r--   0 itaibarsinai   (501) staff       (20)        1 2023-05-04 06:50:38.000000 mona-openai-0.0.2/mona_openai.egg-info/dependency_links.txt
--rw-r--r--   0 itaibarsinai   (501) staff       (20)       38 2023-05-04 06:50:38.000000 mona-openai-0.0.2/mona_openai.egg-info/requires.txt
--rw-r--r--   0 itaibarsinai   (501) staff       (20)       12 2023-05-04 06:50:38.000000 mona-openai-0.0.2/mona_openai.egg-info/top_level.txt
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      818 2023-05-04 06:48:56.000000 mona-openai-0.0.2/pyproject.toml
--rw-r--r--   0 itaibarsinai   (501) staff       (20)       37 2023-05-04 06:43:07.000000 mona-openai-0.0.2/requirements.txt
--rw-r--r--   0 itaibarsinai   (501) staff       (20)       38 2023-05-04 06:50:38.314794 mona-openai-0.0.2/setup.cfg
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-04 06:50:38.314044 mona-openai-0.0.2/tests/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)    11664 2023-05-04 03:41:54.000000 mona-openai-0.0.2/tests/test_completion.py
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-04 06:53:27.363293 mona-openai-0.0.3/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)    11356 2023-04-04 12:33:03.000000 mona-openai-0.0.3/LICENSE
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     8665 2023-05-04 06:53:27.363069 mona-openai-0.0.3/PKG-INFO
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     8071 2023-05-04 03:41:54.000000 mona-openai-0.0.3/README.md
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-04 06:53:27.360457 mona-openai-0.0.3/mona_openai/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)       77 2023-05-04 03:41:54.000000 mona-openai-0.0.3/mona_openai/__init__.py
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-04 06:53:27.361741 mona-openai-0.0.3/mona_openai/analysis/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     1192 2023-04-04 12:33:03.000000 mona-openai-0.0.3/mona_openai/analysis/analysis.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     2693 2023-04-04 12:33:03.000000 mona-openai-0.0.3/mona_openai/analysis/privacy.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      381 2023-04-04 12:33:03.000000 mona-openai-0.0.3/mona_openai/analysis/profanity.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     3748 2023-04-04 12:33:03.000000 mona-openai-0.0.3/mona_openai/analysis/textual.py
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-04 06:53:27.361943 mona-openai-0.0.3/mona_openai/endpoints/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     1786 2023-05-04 03:41:54.000000 mona-openai-0.0.3/mona_openai/endpoints/completion.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      167 2023-04-04 12:33:03.000000 mona-openai-0.0.3/mona_openai/exceptions.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     1379 2023-04-04 12:33:03.000000 mona-openai-0.0.3/mona_openai/mona_client.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)    13259 2023-05-04 03:41:54.000000 mona-openai-0.0.3/mona_openai/mona_openai.py
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-04 06:53:27.362598 mona-openai-0.0.3/mona_openai/util/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     1224 2023-04-04 12:33:03.000000 mona-openai-0.0.3/mona_openai/util/func_util.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      494 2023-04-04 12:33:03.000000 mona-openai-0.0.3/mona_openai/util/math.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      971 2023-04-04 12:33:03.000000 mona-openai-0.0.3/mona_openai/util/validation_util.py
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-04 06:53:27.361194 mona-openai-0.0.3/mona_openai.egg-info/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     8665 2023-05-04 06:53:27.000000 mona-openai-0.0.3/mona_openai.egg-info/PKG-INFO
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      610 2023-05-04 06:53:27.000000 mona-openai-0.0.3/mona_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)        1 2023-05-04 06:53:27.000000 mona-openai-0.0.3/mona_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)       42 2023-05-04 06:53:27.000000 mona-openai-0.0.3/mona_openai.egg-info/requires.txt
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)       12 2023-05-04 06:53:27.000000 mona-openai-0.0.3/mona_openai.egg-info/top_level.txt
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      818 2023-05-04 06:53:09.000000 mona-openai-0.0.3/pyproject.toml
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)       41 2023-05-04 06:52:57.000000 mona-openai-0.0.3/requirements.txt
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)       38 2023-05-04 06:53:27.363334 mona-openai-0.0.3/setup.cfg
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-04 06:53:27.362741 mona-openai-0.0.3/tests/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)    11664 2023-05-04 03:41:54.000000 mona-openai-0.0.3/tests/test_completion.py
```

### Comparing `mona-openai-0.0.2/LICENSE` & `mona-openai-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.2/PKG-INFO` & `mona-openai-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mona-openai
-Version: 0.0.2
+Version: 0.0.3
 Summary: Integration client for monitoring OpenAI usage with Mona
 Author-email: Itai Bar Sinai <itai@monalabs.io>
 Project-URL: Homepage, https://github.com/monalabs/mona-openai
 Project-URL: Bug Tracker, https://github.com/monalabs/mona-openai/issues
 Keywords: OpenAI,LLMs,GPT,Mona,Monitoring,AI
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `mona-openai-0.0.2/README.md` & `mona-openai-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.2/mona_openai/analysis/analysis.py` & `mona-openai-0.0.3/mona_openai/analysis/analysis.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.2/mona_openai/analysis/privacy.py` & `mona-openai-0.0.3/mona_openai/analysis/privacy.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.2/mona_openai/analysis/textual.py` & `mona-openai-0.0.3/mona_openai/analysis/textual.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.2/mona_openai/endpoints/completion.py` & `mona-openai-0.0.3/mona_openai/endpoints/completion.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.2/mona_openai/mona_client.py` & `mona-openai-0.0.3/mona_openai/mona_client.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.2/mona_openai/mona_openai.py` & `mona-openai-0.0.3/mona_openai/mona_openai.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.2/mona_openai/util/func_util.py` & `mona-openai-0.0.3/mona_openai/util/func_util.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.2/mona_openai/util/validation_util.py` & `mona-openai-0.0.3/mona_openai/util/validation_util.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.2/mona_openai.egg-info/PKG-INFO` & `mona-openai-0.0.3/mona_openai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mona-openai
-Version: 0.0.2
+Version: 0.0.3
 Summary: Integration client for monitoring OpenAI usage with Mona
 Author-email: Itai Bar Sinai <itai@monalabs.io>
 Project-URL: Homepage, https://github.com/monalabs/mona-openai
 Project-URL: Bug Tracker, https://github.com/monalabs/mona-openai/issues
 Keywords: OpenAI,LLMs,GPT,Mona,Monitoring,AI
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `mona-openai-0.0.2/mona_openai.egg-info/SOURCES.txt` & `mona-openai-0.0.3/mona_openai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.2/pyproject.toml` & `mona-openai-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mona-openai"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Itai Bar Sinai", email="itai@monalabs.io" },
 ]
 description = "Integration client for monitoring OpenAI usage with Mona"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `mona-openai-0.0.2/tests/test_completion.py` & `mona-openai-0.0.3/tests/test_completion.py`

 * *Files identical despite different names*

