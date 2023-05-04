# Comparing `tmp/chatglm-llm-1.0.2.tar.gz` & `tmp/chatglm-llm-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatglm-llm-1.0.2.tar", last modified: Thu May  4 01:15:10 2023, max compression
+gzip compressed data, was "chatglm-llm-1.0.3.tar", last modified: Thu May  4 01:33:28 2023, max compression
```

## Comparing `chatglm-llm-1.0.2.tar` & `chatglm-llm-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-05-04 01:15:10.713543 chatglm-llm-1.0.2/
--rw-r--r--   0 mroy       (501) staff       (20)      192 2023-05-04 01:15:10.713430 chatglm-llm-1.0.2/PKG-INFO
--rw-r--r--   0 mroy       (501) staff       (20)     1887 2023-05-04 01:08:28.000000 chatglm-llm-1.0.2/README.md
-drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-05-04 01:15:10.712742 chatglm-llm-1.0.2/chatglm_llm.egg-info/
--rw-r--r--   0 mroy       (501) staff       (20)      192 2023-05-04 01:15:10.000000 chatglm-llm-1.0.2/chatglm_llm.egg-info/PKG-INFO
--rw-r--r--   0 mroy       (501) staff       (20)      351 2023-05-04 01:15:10.000000 chatglm-llm-1.0.2/chatglm_llm.egg-info/SOURCES.txt
--rw-r--r--   0 mroy       (501) staff       (20)        1 2023-05-04 01:15:10.000000 chatglm-llm-1.0.2/chatglm_llm.egg-info/dependency_links.txt
--rw-r--r--   0 mroy       (501) staff       (20)       53 2023-05-04 01:15:10.000000 chatglm-llm-1.0.2/chatglm_llm.egg-info/entry_points.txt
--rw-r--r--   0 mroy       (501) staff       (20)        1 2023-05-04 01:12:10.000000 chatglm-llm-1.0.2/chatglm_llm.egg-info/not-zip-safe
--rw-r--r--   0 mroy       (501) staff       (20)      185 2023-05-04 01:15:10.000000 chatglm-llm-1.0.2/chatglm_llm.egg-info/requires.txt
--rw-r--r--   0 mroy       (501) staff       (20)       12 2023-05-04 01:15:10.000000 chatglm-llm-1.0.2/chatglm_llm.egg-info/top_level.txt
-drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-05-04 01:15:10.713190 chatglm-llm-1.0.2/chatglm_src/
--rw-r--r--   0 mroy       (501) staff       (20)       27 2023-05-04 01:08:28.000000 chatglm-llm-1.0.2/chatglm_src/__init__.py
--rw-r--r--   0 mroy       (501) staff       (20)     3963 2023-05-04 01:13:37.000000 chatglm-llm-1.0.2/chatglm_src/callbacks.py
--rw-r--r--   0 mroy       (501) staff       (20)      443 2023-05-04 01:08:28.000000 chatglm-llm-1.0.2/chatglm_src/cmd.py
--rw-r--r--   0 mroy       (501) staff       (20)    16989 2023-05-04 01:09:03.000000 chatglm-llm-1.0.2/chatglm_src/llm.py
--rw-r--r--   0 mroy       (501) staff       (20)       38 2023-05-04 01:15:10.713583 chatglm-llm-1.0.2/setup.cfg
--rw-r--r--   0 mroy       (501) staff       (20)      823 2023-05-04 01:13:51.000000 chatglm-llm-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 01:33:28.289258 chatglm-llm-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)      164 2023-05-04 01:33:28.289258 chatglm-llm-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1887 2023-05-04 01:30:19.000000 chatglm-llm-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 01:33:28.289258 chatglm-llm-1.0.3/chatglm_llm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      164 2023-05-04 01:33:28.000000 chatglm-llm-1.0.3/chatglm_llm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      351 2023-05-04 01:33:28.000000 chatglm-llm-1.0.3/chatglm_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 01:33:28.000000 chatglm-llm-1.0.3/chatglm_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-05-04 01:33:28.000000 chatglm-llm-1.0.3/chatglm_llm.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 01:30:33.000000 chatglm-llm-1.0.3/chatglm_llm.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      175 2023-05-04 01:33:28.000000 chatglm-llm-1.0.3/chatglm_llm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-04 01:33:28.000000 chatglm-llm-1.0.3/chatglm_llm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 01:33:28.289258 chatglm-llm-1.0.3/chatglm_src/
+-rw-r--r--   0 root         (0) root         (0)       27 2023-05-04 01:30:19.000000 chatglm-llm-1.0.3/chatglm_src/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3963 2023-05-04 01:30:19.000000 chatglm-llm-1.0.3/chatglm_src/callbacks.py
+-rw-r--r--   0 root         (0) root         (0)      443 2023-05-04 01:30:19.000000 chatglm-llm-1.0.3/chatglm_src/cmd.py
+-rw-r--r--   0 root         (0) root         (0)    16989 2023-05-04 01:30:19.000000 chatglm-llm-1.0.3/chatglm_src/llm.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-04 01:33:28.289258 chatglm-llm-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      802 2023-05-04 01:33:21.000000 chatglm-llm-1.0.3/setup.py
```

### Comparing `chatglm-llm-1.0.2/README.md` & `chatglm-llm-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.0.2/chatglm_src/callbacks.py` & `chatglm-llm-1.0.3/chatglm_src/callbacks.py`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.0.2/chatglm_src/llm.py` & `chatglm-llm-1.0.3/chatglm_src/llm.py`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.0.2/setup.py` & `chatglm-llm-1.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 
 setup(name='chatglm-llm',
-    version='1.0.2',
+    version='1.0.3',
     description='chatglm llm',
     url='https://github.com/xxx',
     author='auth',
     author_email='xxx@gmail.com',
     license='MIT',
     include_package_data=True,
     zip_safe=False,
@@ -20,15 +20,14 @@
         "mdtex2html",
         "sentencepiece",
         "accelerate",
         'torch',
         'termcolor',
         'tqdm',
         'websockets',
-        'websocket',
         'websocket-client',
         'transformers',
         'aiowebsocket',
         
         ],
     entry_points={
         'console_scripts': [
```

