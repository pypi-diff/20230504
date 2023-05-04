# Comparing `tmp/mona_openai-0.0.0.tar.gz` & `tmp/mona-openai-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mona_openai-0.0.0.tar", last modified: Thu May  4 06:14:42 2023, max compression
+gzip compressed data, was "mona-openai-0.0.1.tar", last modified: Thu May  4 06:21:39 2023, max compression
```

## Comparing `mona_openai-0.0.0.tar` & `mona-openai-0.0.1.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-04 06:14:42.845272 mona_openai-0.0.0/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)    11356 2023-04-04 12:33:03.000000 mona_openai-0.0.0/LICENSE
--rw-r--r--   0 itaibarsinai   (501) staff       (20)       77 2023-05-04 06:14:42.845160 mona_openai-0.0.0/PKG-INFO
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     8071 2023-05-04 03:41:54.000000 mona_openai-0.0.0/README.md
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-04 06:14:42.843133 mona_openai-0.0.0/mona_openai/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)       77 2023-05-04 03:41:54.000000 mona_openai-0.0.0/mona_openai/__init__.py
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-04 06:14:42.844239 mona_openai-0.0.0/mona_openai/analysis/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     1192 2023-04-04 12:33:03.000000 mona_openai-0.0.0/mona_openai/analysis/analysis.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     2693 2023-04-04 12:33:03.000000 mona_openai-0.0.0/mona_openai/analysis/privacy.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      381 2023-04-04 12:33:03.000000 mona_openai-0.0.0/mona_openai/analysis/profanity.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     3748 2023-04-04 12:33:03.000000 mona_openai-0.0.0/mona_openai/analysis/textual.py
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-04 06:14:42.844390 mona_openai-0.0.0/mona_openai/endpoints/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     1786 2023-05-04 03:41:54.000000 mona_openai-0.0.0/mona_openai/endpoints/completion.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      167 2023-04-04 12:33:03.000000 mona_openai-0.0.0/mona_openai/exceptions.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     1379 2023-04-04 12:33:03.000000 mona_openai-0.0.0/mona_openai/mona_client.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)    13259 2023-05-04 03:41:54.000000 mona_openai-0.0.0/mona_openai/mona_openai.py
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-04 06:14:42.844839 mona_openai-0.0.0/mona_openai/util/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     1224 2023-04-04 12:33:03.000000 mona_openai-0.0.0/mona_openai/util/func_util.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      494 2023-04-04 12:33:03.000000 mona_openai-0.0.0/mona_openai/util/math.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      971 2023-04-04 12:33:03.000000 mona_openai-0.0.0/mona_openai/util/validation_util.py
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-04 06:14:42.843682 mona_openai-0.0.0/mona_openai.egg-info/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)       77 2023-05-04 06:14:42.000000 mona_openai-0.0.0/mona_openai.egg-info/PKG-INFO
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      559 2023-05-04 06:14:42.000000 mona_openai-0.0.0/mona_openai.egg-info/SOURCES.txt
--rw-r--r--   0 itaibarsinai   (501) staff       (20)        1 2023-05-04 06:14:42.000000 mona_openai-0.0.0/mona_openai.egg-info/dependency_links.txt
--rw-r--r--   0 itaibarsinai   (501) staff       (20)       12 2023-05-04 06:14:42.000000 mona_openai-0.0.0/mona_openai.egg-info/top_level.txt
--rw-r--r--   0 itaibarsinai   (501) staff       (20)       30 2023-04-04 12:33:03.000000 mona_openai-0.0.0/pyproject.toml
--rw-r--r--   0 itaibarsinai   (501) staff       (20)       38 2023-05-04 06:14:42.845313 mona_openai-0.0.0/setup.cfg
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-04 06:14:42.844990 mona_openai-0.0.0/tests/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)    11664 2023-05-04 03:41:54.000000 mona_openai-0.0.0/tests/test_completion.py
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-04 06:21:39.795971 mona-openai-0.0.1/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)    11356 2023-04-04 12:33:03.000000 mona-openai-0.0.1/LICENSE
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     8665 2023-05-04 06:21:39.795768 mona-openai-0.0.1/PKG-INFO
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     8071 2023-05-04 03:41:54.000000 mona-openai-0.0.1/README.md
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-04 06:21:39.793235 mona-openai-0.0.1/mona_openai/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)       77 2023-05-04 03:41:54.000000 mona-openai-0.0.1/mona_openai/__init__.py
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-04 06:21:39.794755 mona-openai-0.0.1/mona_openai/analysis/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     1192 2023-04-04 12:33:03.000000 mona-openai-0.0.1/mona_openai/analysis/analysis.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     2693 2023-04-04 12:33:03.000000 mona-openai-0.0.1/mona_openai/analysis/privacy.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      381 2023-04-04 12:33:03.000000 mona-openai-0.0.1/mona_openai/analysis/profanity.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     3748 2023-04-04 12:33:03.000000 mona-openai-0.0.1/mona_openai/analysis/textual.py
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-04 06:21:39.794919 mona-openai-0.0.1/mona_openai/endpoints/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     1786 2023-05-04 03:41:54.000000 mona-openai-0.0.1/mona_openai/endpoints/completion.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      167 2023-04-04 12:33:03.000000 mona-openai-0.0.1/mona_openai/exceptions.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     1379 2023-04-04 12:33:03.000000 mona-openai-0.0.1/mona_openai/mona_client.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)    13259 2023-05-04 03:41:54.000000 mona-openai-0.0.1/mona_openai/mona_openai.py
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-04 06:21:39.795391 mona-openai-0.0.1/mona_openai/util/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     1224 2023-04-04 12:33:03.000000 mona-openai-0.0.1/mona_openai/util/func_util.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      494 2023-04-04 12:33:03.000000 mona-openai-0.0.1/mona_openai/util/math.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      971 2023-04-04 12:33:03.000000 mona-openai-0.0.1/mona_openai/util/validation_util.py
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-04 06:21:39.794105 mona-openai-0.0.1/mona_openai.egg-info/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     8665 2023-05-04 06:21:39.000000 mona-openai-0.0.1/mona_openai.egg-info/PKG-INFO
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      610 2023-05-04 06:21:39.000000 mona-openai-0.0.1/mona_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)        1 2023-05-04 06:21:39.000000 mona-openai-0.0.1/mona_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)       25 2023-05-04 06:21:39.000000 mona-openai-0.0.1/mona_openai.egg-info/requires.txt
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)       12 2023-05-04 06:21:39.000000 mona-openai-0.0.1/mona_openai.egg-info/top_level.txt
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      818 2023-05-04 06:19:05.000000 mona-openai-0.0.1/pyproject.toml
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)       24 2023-05-04 06:21:30.000000 mona-openai-0.0.1/requirements.txt
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)       38 2023-05-04 06:21:39.796013 mona-openai-0.0.1/setup.cfg
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-04 06:21:39.795543 mona-openai-0.0.1/tests/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)    11664 2023-05-04 03:41:54.000000 mona-openai-0.0.1/tests/test_completion.py
```

### Comparing `mona_openai-0.0.0/LICENSE` & `mona-openai-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mona_openai-0.0.0/README.md` & `mona-openai-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `mona_openai-0.0.0/mona_openai/analysis/analysis.py` & `mona-openai-0.0.1/mona_openai/analysis/analysis.py`

 * *Files identical despite different names*

### Comparing `mona_openai-0.0.0/mona_openai/analysis/privacy.py` & `mona-openai-0.0.1/mona_openai/analysis/privacy.py`

 * *Files identical despite different names*

### Comparing `mona_openai-0.0.0/mona_openai/analysis/textual.py` & `mona-openai-0.0.1/mona_openai/analysis/textual.py`

 * *Files identical despite different names*

### Comparing `mona_openai-0.0.0/mona_openai/endpoints/completion.py` & `mona-openai-0.0.1/mona_openai/endpoints/completion.py`

 * *Files identical despite different names*

### Comparing `mona_openai-0.0.0/mona_openai/mona_client.py` & `mona-openai-0.0.1/mona_openai/mona_client.py`

 * *Files identical despite different names*

### Comparing `mona_openai-0.0.0/mona_openai/mona_openai.py` & `mona-openai-0.0.1/mona_openai/mona_openai.py`

 * *Files identical despite different names*

### Comparing `mona_openai-0.0.0/mona_openai/util/func_util.py` & `mona-openai-0.0.1/mona_openai/util/func_util.py`

 * *Files identical despite different names*

### Comparing `mona_openai-0.0.0/mona_openai/util/validation_util.py` & `mona-openai-0.0.1/mona_openai/util/validation_util.py`

 * *Files identical despite different names*

### Comparing `mona_openai-0.0.0/mona_openai.egg-info/SOURCES.txt` & `mona-openai-0.0.1/mona_openai.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 LICENSE
 README.md
 pyproject.toml
+requirements.txt
 mona_openai/__init__.py
 mona_openai/exceptions.py
 mona_openai/mona_client.py
 mona_openai/mona_openai.py
 mona_openai.egg-info/PKG-INFO
 mona_openai.egg-info/SOURCES.txt
 mona_openai.egg-info/dependency_links.txt
+mona_openai.egg-info/requires.txt
 mona_openai.egg-info/top_level.txt
 mona_openai/analysis/analysis.py
 mona_openai/analysis/privacy.py
 mona_openai/analysis/profanity.py
 mona_openai/analysis/textual.py
 mona_openai/endpoints/completion.py
 mona_openai/util/func_util.py
```

### Comparing `mona_openai-0.0.0/tests/test_completion.py` & `mona-openai-0.0.1/tests/test_completion.py`

 * *Files identical despite different names*

