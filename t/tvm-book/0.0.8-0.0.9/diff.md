# Comparing `tmp/tvm-book-0.0.8.tar.gz` & `tmp/tvm-book-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tvm-book-0.0.8.tar", last modified: Fri Feb 17 05:32:00 2023, max compression
+gzip compressed data, was "tvm-book-0.0.9.tar", last modified: Fri Feb 17 07:44:58 2023, max compression
```

## Comparing `tvm-book-0.0.8.tar` & `tvm-book-0.0.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rwxr-xr-x   0        0        0    11357 2022-12-28 05:44:56.193075 tvm-book-0.0.8/LICENSE
--rwxr-xr-x   0        0        0     2135 2023-02-08 04:56:53.536146 tvm-book-0.0.8/README.md
--rw-r--r--   0        0        0     1262 2023-02-17 04:51:28.763242 tvm-book-0.0.8/pyproject.toml
--rw-r--r--   0        0        0       21 2023-02-17 05:31:57.973055 tvm-book-0.0.8/src/tvm_book/__about__.py
--rwxr-xr-x   0        0        0       51 2023-02-08 13:29:08.146532 tvm-book-0.0.8/src/tvm_book/__init__.py
--rwxr-xr-x   0        0        0       43 2023-01-31 11:51:45.271844 tvm-book-0.0.8/src/tvm_book/contrib/d2ltvm/__init__.py
--rwxr-xr-x   0        0        0    25396 2023-01-31 11:51:45.271844 tvm-book-0.0.8/src/tvm_book/contrib/d2ltvm/_d2ltvm.py
--rwxr-xr-x   0        0        0    22451 2023-01-31 11:51:45.271844 tvm-book-0.0.8/src/tvm_book/contrib/d2ltvm/d2ltvm.py
--rwxr-xr-x   0        0        0        0 2023-01-31 11:51:45.271844 tvm-book-0.0.8/src/tvm_book/contrib/mxnet/__init__.py
--rwxr-xr-x   0        0        0     3592 2023-01-31 11:51:45.271844 tvm-book-0.0.8/src/tvm_book/contrib/mxnet/model.py
--rwxr-xr-x   0        0        0     1922 2023-01-31 11:51:45.271844 tvm-book-0.0.8/src/tvm_book/contrib/mxnet/tools.py
--rwxr-xr-x   0        0        0        0 2023-01-31 11:51:45.275844 tvm-book-0.0.8/src/tvm_book/contrib/tvm/__init__.py
--rwxr-xr-x   0        0        0      389 2023-01-31 11:51:45.275844 tvm-book-0.0.8/src/tvm_book/contrib/tvm/config.py
--rwxr-xr-x   0        0        0      986 2023-01-31 11:51:45.275844 tvm-book-0.0.8/src/tvm_book/contrib/tvm/model.py
--rwxr-xr-x   0        0        0     1436 2023-01-31 11:51:45.275844 tvm-book-0.0.8/src/tvm_book/contrib/tvm/quantize.py
--rwxr-xr-x   0        0        0     2043 2023-01-31 11:51:45.275844 tvm-book-0.0.8/src/tvm_book/contrib/tvm/test.py
--rwxr-xr-x   0        0        0        0 2023-01-31 11:51:45.275844 tvm-book-0.0.8/src/tvm_book/image/__init__.py
--rwxr-xr-x   0        0        0     1654 2023-01-31 11:51:45.275844 tvm-book-0.0.8/src/tvm_book/image/process.py
--rwxr-xr-x   0        0        0        0 2023-01-31 11:51:45.275844 tvm-book-0.0.8/src/tvm_book/mxnet/__init__.py
--rwxr-xr-x   0        0        0     2985 2023-01-31 11:51:45.275844 tvm-book-0.0.8/src/tvm_book/mxnet/imagenet.py
--rw-r--r--   0        0        0       19 2023-01-31 11:51:45.279845 tvm-book-0.0.8/src/tvm_book/numpy/__init__.py
--rw-r--r--   0        0        0       68 2023-01-31 11:51:45.279845 tvm-book-0.0.8/src/tvm_book/numpy/nn/__init__.py
--rw-r--r--   0        0        0     3120 2023-01-31 11:51:45.279845 tvm-book-0.0.8/src/tvm_book/numpy/nn/conv.py
--rw-r--r--   0        0        0      395 2023-01-31 11:51:45.279845 tvm-book-0.0.8/src/tvm_book/numpy/nn/padding.py
--rwxr-xr-x   0        0        0      172 2023-01-31 11:51:45.279845 tvm-book-0.0.8/src/tvm_book/testing/relay/let.py
--rwxr-xr-x   0        0        0      726 2023-01-31 11:51:45.279845 tvm-book-0.0.8/src/tvm_book/testing/relay/viz.py
--rwxr-xr-x   0        0        0        0 2023-01-31 11:51:45.279845 tvm-book-0.0.8/src/tvm_book/tvm_utils/__init__.py
--rw-r--r--   0        0        0        0 2023-02-17 05:21:58.006956 tvm-book-0.0.8/src/tvm_book/tvm_utils/config/__init__.py
--rwxr-xr-x   0        0        0      954 2023-01-31 11:51:45.283845 tvm-book-0.0.8/src/tvm_book/tvm_utils/config/_env.py
--rw-r--r--   0        0        0      228 2023-02-17 05:24:42.842740 tvm-book-0.0.8/src/tvm_book/tvm_utils/config/env.py
--rwxr-xr-x   0        0        0      938 2023-01-31 11:51:45.283845 tvm-book-0.0.8/src/tvm_book/tvm_utils/remote.py
--rwxr-xr-x   0        0        0     1582 2023-01-31 11:51:45.283845 tvm-book-0.0.8/src/tvm_book/tvm_utils/viz_relay.py
--rwxr-xr-x   0        0        0        0 2023-01-31 11:51:45.283845 tvm-book-0.0.8/src/tvm_book/vta/__init__.py
--rwxr-xr-x   0        0        0     1912 2023-01-31 11:51:45.283845 tvm-book-0.0.8/src/tvm_book/vta/remote.py
--rwxr-xr-x   0        0        0     3928 2023-01-31 11:51:45.283845 tvm-book-0.0.8/src/tvm_book/vta/vtac.py
--rw-r--r--   0        0        0     2507 1970-01-01 00:00:00.000000 tvm-book-0.0.8/PKG-INFO
+-rwxr-xr-x   0        0        0    11357 2022-12-28 05:44:56.193075 tvm-book-0.0.9/LICENSE
+-rwxr-xr-x   0        0        0     2135 2023-02-08 04:56:53.536146 tvm-book-0.0.9/README.md
+-rw-r--r--   0        0        0     1204 2023-02-17 07:42:42.556297 tvm-book-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-02-17 07:44:34.067262 tvm-book-0.0.9/src/tvm_book/__about__.py
+-rwxr-xr-x   0        0        0       51 2023-02-08 13:29:08.146532 tvm-book-0.0.9/src/tvm_book/__init__.py
+-rwxr-xr-x   0        0        0       43 2023-01-31 11:51:45.271844 tvm-book-0.0.9/src/tvm_book/contrib/d2ltvm/__init__.py
+-rwxr-xr-x   0        0        0    25396 2023-01-31 11:51:45.271844 tvm-book-0.0.9/src/tvm_book/contrib/d2ltvm/_d2ltvm.py
+-rwxr-xr-x   0        0        0    22451 2023-01-31 11:51:45.271844 tvm-book-0.0.9/src/tvm_book/contrib/d2ltvm/d2ltvm.py
+-rwxr-xr-x   0        0        0        0 2023-01-31 11:51:45.271844 tvm-book-0.0.9/src/tvm_book/contrib/mxnet/__init__.py
+-rwxr-xr-x   0        0        0     3592 2023-01-31 11:51:45.271844 tvm-book-0.0.9/src/tvm_book/contrib/mxnet/model.py
+-rwxr-xr-x   0        0        0     1922 2023-01-31 11:51:45.271844 tvm-book-0.0.9/src/tvm_book/contrib/mxnet/tools.py
+-rwxr-xr-x   0        0        0        0 2023-01-31 11:51:45.275844 tvm-book-0.0.9/src/tvm_book/contrib/tvm/__init__.py
+-rwxr-xr-x   0        0        0      389 2023-01-31 11:51:45.275844 tvm-book-0.0.9/src/tvm_book/contrib/tvm/config.py
+-rwxr-xr-x   0        0        0      986 2023-01-31 11:51:45.275844 tvm-book-0.0.9/src/tvm_book/contrib/tvm/model.py
+-rwxr-xr-x   0        0        0     1436 2023-01-31 11:51:45.275844 tvm-book-0.0.9/src/tvm_book/contrib/tvm/quantize.py
+-rwxr-xr-x   0        0        0     2043 2023-01-31 11:51:45.275844 tvm-book-0.0.9/src/tvm_book/contrib/tvm/test.py
+-rwxr-xr-x   0        0        0        0 2023-01-31 11:51:45.275844 tvm-book-0.0.9/src/tvm_book/image/__init__.py
+-rwxr-xr-x   0        0        0     1654 2023-01-31 11:51:45.275844 tvm-book-0.0.9/src/tvm_book/image/process.py
+-rwxr-xr-x   0        0        0        0 2023-01-31 11:51:45.275844 tvm-book-0.0.9/src/tvm_book/mxnet/__init__.py
+-rwxr-xr-x   0        0        0     2985 2023-01-31 11:51:45.275844 tvm-book-0.0.9/src/tvm_book/mxnet/imagenet.py
+-rw-r--r--   0        0        0       19 2023-01-31 11:51:45.279845 tvm-book-0.0.9/src/tvm_book/numpy/__init__.py
+-rw-r--r--   0        0        0       68 2023-01-31 11:51:45.279845 tvm-book-0.0.9/src/tvm_book/numpy/nn/__init__.py
+-rw-r--r--   0        0        0     3120 2023-01-31 11:51:45.279845 tvm-book-0.0.9/src/tvm_book/numpy/nn/conv.py
+-rw-r--r--   0        0        0      395 2023-01-31 11:51:45.279845 tvm-book-0.0.9/src/tvm_book/numpy/nn/padding.py
+-rwxr-xr-x   0        0        0      172 2023-01-31 11:51:45.279845 tvm-book-0.0.9/src/tvm_book/testing/relay/let.py
+-rwxr-xr-x   0        0        0      726 2023-01-31 11:51:45.279845 tvm-book-0.0.9/src/tvm_book/testing/relay/viz.py
+-rwxr-xr-x   0        0        0        0 2023-01-31 11:51:45.279845 tvm-book-0.0.9/src/tvm_book/tvm_utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-17 05:21:58.006956 tvm-book-0.0.9/src/tvm_book/tvm_utils/config/__init__.py
+-rwxr-xr-x   0        0        0      954 2023-01-31 11:51:45.283845 tvm-book-0.0.9/src/tvm_book/tvm_utils/config/_env.py
+-rw-r--r--   0        0        0      228 2023-02-17 05:24:42.842740 tvm-book-0.0.9/src/tvm_book/tvm_utils/config/env.py
+-rwxr-xr-x   0        0        0      938 2023-01-31 11:51:45.283845 tvm-book-0.0.9/src/tvm_book/tvm_utils/remote.py
+-rwxr-xr-x   0        0        0     1582 2023-01-31 11:51:45.283845 tvm-book-0.0.9/src/tvm_book/tvm_utils/viz_relay.py
+-rwxr-xr-x   0        0        0        0 2023-01-31 11:51:45.283845 tvm-book-0.0.9/src/tvm_book/vta/__init__.py
+-rwxr-xr-x   0        0        0     1912 2023-01-31 11:51:45.283845 tvm-book-0.0.9/src/tvm_book/vta/remote.py
+-rwxr-xr-x   0        0        0     3928 2023-01-31 11:51:45.283845 tvm-book-0.0.9/src/tvm_book/vta/vtac.py
+-rw-r--r--   0        0        0     2507 1970-01-01 00:00:00.000000 tvm-book-0.0.9/PKG-INFO
```

### Comparing `tvm-book-0.0.8/LICENSE` & `tvm-book-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tvm-book-0.0.8/README.md` & `tvm-book-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `tvm-book-0.0.8/pyproject.toml` & `tvm-book-0.0.9/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -2,17 +2,15 @@
 allow_prereleases = true
 
 [tool.pdm.version]
 source = "file"
 path = "src/tvm_book/__about__.py"
 
 [tool.pdm.dev-dependencies]
-npu = [
-    "tvmx @ file:///media/pc/data/lxw/ai/tvm/xinetzone",
-]
+npu = []
 
 [tool.pdm.build]
 excludes = [
     "doc",
     ".github",
 ]
 source-includes = [
@@ -26,15 +24,15 @@
     { name = "xinetzone", email = "xinzone@outlook.com" },
 ]
 dependencies = [
     "importlib-metadata>=4.12",
 ]
 requires-python = ">=3.10"
 readme = "README.md"
-version = "0.0.8"
+version = "0.0.9"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Homepage = "https://xinetzone.github.io/tvm-book"
 Repository = "https://github.com/xinetzone/tvm-book"
```

### Comparing `tvm-book-0.0.8/src/tvm_book/contrib/d2ltvm/_d2ltvm.py` & `tvm-book-0.0.9/src/tvm_book/contrib/d2ltvm/_d2ltvm.py`

 * *Files identical despite different names*

### Comparing `tvm-book-0.0.8/src/tvm_book/contrib/d2ltvm/d2ltvm.py` & `tvm-book-0.0.9/src/tvm_book/contrib/d2ltvm/d2ltvm.py`

 * *Files identical despite different names*

### Comparing `tvm-book-0.0.8/src/tvm_book/contrib/mxnet/model.py` & `tvm-book-0.0.9/src/tvm_book/contrib/mxnet/model.py`

 * *Files identical despite different names*

### Comparing `tvm-book-0.0.8/src/tvm_book/contrib/mxnet/tools.py` & `tvm-book-0.0.9/src/tvm_book/contrib/mxnet/tools.py`

 * *Files identical despite different names*

### Comparing `tvm-book-0.0.8/src/tvm_book/contrib/tvm/model.py` & `tvm-book-0.0.9/src/tvm_book/contrib/tvm/model.py`

 * *Files identical despite different names*

### Comparing `tvm-book-0.0.8/src/tvm_book/contrib/tvm/quantize.py` & `tvm-book-0.0.9/src/tvm_book/contrib/tvm/quantize.py`

 * *Files identical despite different names*

### Comparing `tvm-book-0.0.8/src/tvm_book/contrib/tvm/test.py` & `tvm-book-0.0.9/src/tvm_book/contrib/tvm/test.py`

 * *Files identical despite different names*

### Comparing `tvm-book-0.0.8/src/tvm_book/image/process.py` & `tvm-book-0.0.9/src/tvm_book/image/process.py`

 * *Files identical despite different names*

### Comparing `tvm-book-0.0.8/src/tvm_book/mxnet/imagenet.py` & `tvm-book-0.0.9/src/tvm_book/mxnet/imagenet.py`

 * *Files identical despite different names*

### Comparing `tvm-book-0.0.8/src/tvm_book/numpy/nn/conv.py` & `tvm-book-0.0.9/src/tvm_book/numpy/nn/conv.py`

 * *Files identical despite different names*

### Comparing `tvm-book-0.0.8/src/tvm_book/testing/relay/viz.py` & `tvm-book-0.0.9/src/tvm_book/testing/relay/viz.py`

 * *Files identical despite different names*

### Comparing `tvm-book-0.0.8/src/tvm_book/tvm_utils/config/_env.py` & `tvm-book-0.0.9/src/tvm_book/tvm_utils/config/_env.py`

 * *Files identical despite different names*

### Comparing `tvm-book-0.0.8/src/tvm_book/tvm_utils/remote.py` & `tvm-book-0.0.9/src/tvm_book/tvm_utils/remote.py`

 * *Files identical despite different names*

### Comparing `tvm-book-0.0.8/src/tvm_book/tvm_utils/viz_relay.py` & `tvm-book-0.0.9/src/tvm_book/tvm_utils/viz_relay.py`

 * *Files identical despite different names*

### Comparing `tvm-book-0.0.8/src/tvm_book/vta/remote.py` & `tvm-book-0.0.9/src/tvm_book/vta/remote.py`

 * *Files identical despite different names*

### Comparing `tvm-book-0.0.8/src/tvm_book/vta/vtac.py` & `tvm-book-0.0.9/src/tvm_book/vta/vtac.py`

 * *Files identical despite different names*

### Comparing `tvm-book-0.0.8/PKG-INFO` & `tvm-book-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvm-book
-Version: 0.0.8
+Version: 0.0.9
 Author-email: xinetzone <xinzone@outlook.com>
 Requires-Python: >=3.10
 Provides-Extra: doc
 Project-URL: Documentation, https://xinetzone.github.io/tvm-book
 Project-URL: Homepage, https://xinetzone.github.io/tvm-book
 Project-URL: Repository, https://github.com/xinetzone/tvm-book
 Description-Content-Type: text/markdown
```

