# Comparing `tmp/openlimit-0.2.5.tar.gz` & `tmp/openlimit-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlimit-0.2.5.tar", last modified: Tue Apr 25 12:10:09 2023, max compression
+gzip compressed data, was "openlimit-0.2.6.tar", last modified: Thu May  4 13:03:38 2023, max compression
```

## Comparing `openlimit-0.2.5.tar` & `openlimit-0.2.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-04-25 12:10:09.808933 openlimit-0.2.5/
--rw-r--r--   0 jshobrook   (501) staff       (20)      351 2023-04-25 12:10:09.808765 openlimit-0.2.5/PKG-INFO
--rw-r--r--   0 jshobrook   (501) staff       (20)     3216 2023-04-23 12:13:25.000000 openlimit-0.2.5/README.md
-drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-04-25 12:10:09.806305 openlimit-0.2.5/openlimit/
--rw-r--r--   0 jshobrook   (501) staff       (20)      226 2023-04-23 11:35:43.000000 openlimit-0.2.5/openlimit/__init__.py
-drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-04-25 12:10:09.807598 openlimit-0.2.5/openlimit/buckets/
--rw-r--r--   0 jshobrook   (501) staff       (20)       98 2023-04-23 11:38:27.000000 openlimit-0.2.5/openlimit/buckets/__init__.py
--rw-r--r--   0 jshobrook   (501) staff       (20)      988 2023-04-23 11:03:59.000000 openlimit-0.2.5/openlimit/buckets/bucket.py
--rw-r--r--   0 jshobrook   (501) staff       (20)     1869 2023-04-23 11:01:20.000000 openlimit-0.2.5/openlimit/buckets/redis_bucket.py
--rw-r--r--   0 jshobrook   (501) staff       (20)     1792 2023-04-25 12:08:59.000000 openlimit-0.2.5/openlimit/rate_limiters.py
--rw-r--r--   0 jshobrook   (501) staff       (20)     2928 2023-04-25 12:09:39.000000 openlimit-0.2.5/openlimit/redis_rate_limiters.py
-drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-04-25 12:10:09.808400 openlimit-0.2.5/openlimit/utilities/
--rw-r--r--   0 jshobrook   (501) staff       (20)      252 2023-04-23 11:41:16.000000 openlimit-0.2.5/openlimit/utilities/__init__.py
--rw-r--r--   0 jshobrook   (501) staff       (20)     1576 2023-04-23 11:03:35.000000 openlimit-0.2.5/openlimit/utilities/context_decorators.py
--rw-r--r--   0 jshobrook   (501) staff       (20)     1681 2023-04-20 01:13:53.000000 openlimit-0.2.5/openlimit/utilities/token_counters.py
-drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-04-25 12:10:09.807016 openlimit-0.2.5/openlimit.egg-info/
--rw-r--r--   0 jshobrook   (501) staff       (20)      351 2023-04-25 12:10:09.000000 openlimit-0.2.5/openlimit.egg-info/PKG-INFO
--rw-r--r--   0 jshobrook   (501) staff       (20)      468 2023-04-25 12:10:09.000000 openlimit-0.2.5/openlimit.egg-info/SOURCES.txt
--rw-r--r--   0 jshobrook   (501) staff       (20)        1 2023-04-25 12:10:09.000000 openlimit-0.2.5/openlimit.egg-info/dependency_links.txt
--rw-r--r--   0 jshobrook   (501) staff       (20)       15 2023-04-25 12:10:09.000000 openlimit-0.2.5/openlimit.egg-info/requires.txt
--rw-r--r--   0 jshobrook   (501) staff       (20)       10 2023-04-25 12:10:09.000000 openlimit-0.2.5/openlimit.egg-info/top_level.txt
--rw-r--r--   0 jshobrook   (501) staff       (20)       38 2023-04-25 12:10:09.809013 openlimit-0.2.5/setup.cfg
--rw-r--r--   0 jshobrook   (501) staff       (20)      559 2023-04-25 12:10:05.000000 openlimit-0.2.5/setup.py
+drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-05-04 13:03:38.562792 openlimit-0.2.6/
+-rw-r--r--   0 jshobrook   (501) staff       (20)      351 2023-05-04 13:03:38.562679 openlimit-0.2.6/PKG-INFO
+-rw-r--r--   0 jshobrook   (501) staff       (20)     3216 2023-04-23 12:13:25.000000 openlimit-0.2.6/README.md
+drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-05-04 13:03:38.560601 openlimit-0.2.6/openlimit/
+-rw-r--r--   0 jshobrook   (501) staff       (20)      226 2023-04-23 11:35:43.000000 openlimit-0.2.6/openlimit/__init__.py
+drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-05-04 13:03:38.561807 openlimit-0.2.6/openlimit/buckets/
+-rw-r--r--   0 jshobrook   (501) staff       (20)       98 2023-04-23 11:38:27.000000 openlimit-0.2.6/openlimit/buckets/__init__.py
+-rw-r--r--   0 jshobrook   (501) staff       (20)      988 2023-04-23 11:03:59.000000 openlimit-0.2.6/openlimit/buckets/bucket.py
+-rw-r--r--   0 jshobrook   (501) staff       (20)     1869 2023-04-23 11:01:20.000000 openlimit-0.2.6/openlimit/buckets/redis_bucket.py
+-rw-r--r--   0 jshobrook   (501) staff       (20)     1792 2023-05-01 20:23:40.000000 openlimit-0.2.6/openlimit/rate_limiters.py
+-rw-r--r--   0 jshobrook   (501) staff       (20)     2928 2023-04-25 12:09:39.000000 openlimit-0.2.6/openlimit/redis_rate_limiters.py
+drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-05-04 13:03:38.562427 openlimit-0.2.6/openlimit/utilities/
+-rw-r--r--   0 jshobrook   (501) staff       (20)      252 2023-04-23 11:41:16.000000 openlimit-0.2.6/openlimit/utilities/__init__.py
+-rw-r--r--   0 jshobrook   (501) staff       (20)     1576 2023-04-23 11:03:35.000000 openlimit-0.2.6/openlimit/utilities/context_decorators.py
+-rw-r--r--   0 jshobrook   (501) staff       (20)     1641 2023-05-04 13:02:49.000000 openlimit-0.2.6/openlimit/utilities/token_counters.py
+drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-05-04 13:03:38.561195 openlimit-0.2.6/openlimit.egg-info/
+-rw-r--r--   0 jshobrook   (501) staff       (20)      351 2023-05-04 13:03:38.000000 openlimit-0.2.6/openlimit.egg-info/PKG-INFO
+-rw-r--r--   0 jshobrook   (501) staff       (20)      468 2023-05-04 13:03:38.000000 openlimit-0.2.6/openlimit.egg-info/SOURCES.txt
+-rw-r--r--   0 jshobrook   (501) staff       (20)        1 2023-05-04 13:03:38.000000 openlimit-0.2.6/openlimit.egg-info/dependency_links.txt
+-rw-r--r--   0 jshobrook   (501) staff       (20)       15 2023-05-04 13:03:38.000000 openlimit-0.2.6/openlimit.egg-info/requires.txt
+-rw-r--r--   0 jshobrook   (501) staff       (20)       10 2023-05-04 13:03:38.000000 openlimit-0.2.6/openlimit.egg-info/top_level.txt
+-rw-r--r--   0 jshobrook   (501) staff       (20)       38 2023-05-04 13:03:38.562831 openlimit-0.2.6/setup.cfg
+-rw-r--r--   0 jshobrook   (501) staff       (20)      559 2023-05-04 13:03:33.000000 openlimit-0.2.6/setup.py
```

### Comparing `openlimit-0.2.5/README.md` & `openlimit-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `openlimit-0.2.5/openlimit/buckets/bucket.py` & `openlimit-0.2.6/openlimit/buckets/bucket.py`

 * *Files identical despite different names*

### Comparing `openlimit-0.2.5/openlimit/buckets/redis_bucket.py` & `openlimit-0.2.6/openlimit/buckets/redis_bucket.py`

 * *Files identical despite different names*

### Comparing `openlimit-0.2.5/openlimit/rate_limiters.py` & `openlimit-0.2.6/openlimit/rate_limiters.py`

 * *Files identical despite different names*

### Comparing `openlimit-0.2.5/openlimit/redis_rate_limiters.py` & `openlimit-0.2.6/openlimit/redis_rate_limiters.py`

 * *Files identical despite different names*

### Comparing `openlimit-0.2.5/openlimit/utilities/context_decorators.py` & `openlimit-0.2.6/openlimit/utilities/context_decorators.py`

 * *Files identical despite different names*

### Comparing `openlimit-0.2.5/openlimit/utilities/token_counters.py` & `openlimit-0.2.6/openlimit/utilities/token_counters.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,14 @@
     return num_tokens
     
 
 def num_tokens_consumed_by_completion_request(prompt, max_tokens=15, n=1, **kwargs):
     num_tokens = n * max_tokens
     if isinstance(prompt, str): # Single prompt
         num_tokens += len(P50K_ENCODER.encode(prompt))
-        num_tokens += completion_tokens
     elif isinstance(prompt, list): # Multiple prompts
         num_tokens *= len(prompt)
         num_tokens += sum([len(P50K_ENCODER.encode(p) for p in prompt)])
     else:
         raise TypeError("Either a string or list of strings expected for 'prompt' field in completion request.")
     
     return num_tokens
```

### Comparing `openlimit-0.2.5/setup.py` & `openlimit-0.2.6/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 from setuptools import setup
 
 setup(
     name="openlimit",
     description="Rate limiter for the OpenAI API",
-    version="v0.2.5",
+    version="v0.2.6",
     packages=["openlimit", "openlimit.utilities", "openlimit.buckets"],
     python_requires=">=3",
     url="https://github.com/shobrook/openlimit",
     author="shobrook",
     author_email="shobrookj@gmail.com",
     # classifiers=[],
     install_requires=["redis", "tiktoken"],
```

