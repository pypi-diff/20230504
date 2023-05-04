# Comparing `tmp/modelw_docker-2023.4.0b3.tar.gz` & `tmp/modelw_docker-2023.4.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelw_docker-2023.4.0b3.tar", max compression
+gzip compressed data, was "modelw_docker-2023.4.0b4.tar", max compression
```

## Comparing `modelw_docker-2023.4.0b3.tar` & `modelw_docker-2023.4.0b4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      484 2023-05-04 14:37:28.926010 modelw_docker-2023.4.0b3/LICENSE
--rw-r--r--   0        0        0     4666 2023-05-04 14:37:28.926010 modelw_docker-2023.4.0b3/README.md
--rw-r--r--   0        0        0     1201 2023-05-04 14:37:28.930010 modelw_docker-2023.4.0b3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-04 14:37:28.930010 modelw_docker-2023.4.0b3/src/model_w/docker/__init__.py
--rw-r--r--   0        0        0     2753 2023-05-04 14:37:28.930010 modelw_docker-2023.4.0b3/src/model_w/docker/__main__.py
--rw-r--r--   0        0        0     1494 2023-05-04 14:37:28.930010 modelw_docker-2023.4.0b3/src/model_w/docker/build.py
--rw-r--r--   0        0        0     7307 2023-05-04 14:37:28.930010 modelw_docker-2023.4.0b3/src/model_w/docker/config.py
--rw-r--r--   0        0        0      209 2023-05-04 14:37:28.930010 modelw_docker-2023.4.0b3/src/model_w/docker/exceptions.py
--rw-r--r--   0        0        0     5229 2023-05-04 14:37:28.930010 modelw_docker-2023.4.0b3/src/model_w/docker/install.py
--rw-r--r--   0        0        0     7755 2023-05-04 14:37:28.930010 modelw_docker-2023.4.0b3/src/model_w/docker/output.py
--rw-r--r--   0        0        0     1662 2023-05-04 14:37:28.930010 modelw_docker-2023.4.0b3/src/model_w/docker/platform.py
--rw-r--r--   0        0        0        0 2023-05-04 14:37:28.930010 modelw_docker-2023.4.0b3/src/model_w/docker/py.typed
--rw-r--r--   0        0        0     2580 2023-05-04 14:37:28.930010 modelw_docker-2023.4.0b3/src/model_w/docker/run.py
--rw-r--r--   0        0        0     5865 2023-05-04 14:37:28.930010 modelw_docker-2023.4.0b3/src/model_w/docker/serve.py
--rw-r--r--   0        0        0     5909 1970-01-01 00:00:00.000000 modelw_docker-2023.4.0b3/PKG-INFO
+-rw-r--r--   0        0        0      484 2023-05-04 15:27:48.554730 modelw_docker-2023.4.0b4/LICENSE
+-rw-r--r--   0        0        0     4666 2023-05-04 15:27:48.554730 modelw_docker-2023.4.0b4/README.md
+-rw-r--r--   0        0        0     1201 2023-05-04 15:27:48.558730 modelw_docker-2023.4.0b4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-04 15:27:48.558730 modelw_docker-2023.4.0b4/src/model_w/docker/__init__.py
+-rw-r--r--   0        0        0     2753 2023-05-04 15:27:48.558730 modelw_docker-2023.4.0b4/src/model_w/docker/__main__.py
+-rw-r--r--   0        0        0     1494 2023-05-04 15:27:48.558730 modelw_docker-2023.4.0b4/src/model_w/docker/build.py
+-rw-r--r--   0        0        0     7307 2023-05-04 15:27:48.558730 modelw_docker-2023.4.0b4/src/model_w/docker/config.py
+-rw-r--r--   0        0        0      209 2023-05-04 15:27:48.558730 modelw_docker-2023.4.0b4/src/model_w/docker/exceptions.py
+-rw-r--r--   0        0        0     5229 2023-05-04 15:27:48.558730 modelw_docker-2023.4.0b4/src/model_w/docker/install.py
+-rw-r--r--   0        0        0     7755 2023-05-04 15:27:48.558730 modelw_docker-2023.4.0b4/src/model_w/docker/output.py
+-rw-r--r--   0        0        0     1662 2023-05-04 15:27:48.558730 modelw_docker-2023.4.0b4/src/model_w/docker/platform.py
+-rw-r--r--   0        0        0        0 2023-05-04 15:27:48.558730 modelw_docker-2023.4.0b4/src/model_w/docker/py.typed
+-rw-r--r--   0        0        0     2580 2023-05-04 15:27:48.558730 modelw_docker-2023.4.0b4/src/model_w/docker/run.py
+-rw-r--r--   0        0        0     5865 2023-05-04 15:27:48.558730 modelw_docker-2023.4.0b4/src/model_w/docker/serve.py
+-rw-r--r--   0        0        0     5909 1970-01-01 00:00:00.000000 modelw_docker-2023.4.0b4/PKG-INFO
```

### Comparing `modelw_docker-2023.4.0b3/README.md` & `modelw_docker-2023.4.0b4/README.md`

 * *Files identical despite different names*

### Comparing `modelw_docker-2023.4.0b3/pyproject.toml` & `modelw_docker-2023.4.0b4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "modelw-docker"
-version = "2023.4.0b3"
+version = "2023.4.0b4"
 description = "Utility to simplify Dockerfiles"
 authors = ["Rémy Sanchez <remy.sanchez@hyperthese.net>"]
 license = "WTFPL"
 readme = "README.md"
 packages = [{include = "model_w/docker", from = "src"}]
 repository = "https://github.com/ModelW/docker/"
 documentation = "https://github.com/ModelW/docker/"
```

### Comparing `modelw_docker-2023.4.0b3/src/model_w/docker/__main__.py` & `modelw_docker-2023.4.0b4/src/model_w/docker/__main__.py`

 * *Files identical despite different names*

### Comparing `modelw_docker-2023.4.0b3/src/model_w/docker/build.py` & `modelw_docker-2023.4.0b4/src/model_w/docker/build.py`

 * *Files identical despite different names*

### Comparing `modelw_docker-2023.4.0b3/src/model_w/docker/config.py` & `modelw_docker-2023.4.0b4/src/model_w/docker/config.py`

 * *Files identical despite different names*

### Comparing `modelw_docker-2023.4.0b3/src/model_w/docker/install.py` & `modelw_docker-2023.4.0b4/src/model_w/docker/install.py`

 * *Files identical despite different names*

### Comparing `modelw_docker-2023.4.0b3/src/model_w/docker/output.py` & `modelw_docker-2023.4.0b4/src/model_w/docker/output.py`

 * *Files identical despite different names*

### Comparing `modelw_docker-2023.4.0b3/src/model_w/docker/platform.py` & `modelw_docker-2023.4.0b4/src/model_w/docker/platform.py`

 * *Files identical despite different names*

### Comparing `modelw_docker-2023.4.0b3/src/model_w/docker/run.py` & `modelw_docker-2023.4.0b4/src/model_w/docker/run.py`

 * *Files identical despite different names*

### Comparing `modelw_docker-2023.4.0b3/src/model_w/docker/serve.py` & `modelw_docker-2023.4.0b4/src/model_w/docker/serve.py`

 * *Files identical despite different names*

### Comparing `modelw_docker-2023.4.0b3/PKG-INFO` & `modelw_docker-2023.4.0b4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelw-docker
-Version: 2023.4.0b3
+Version: 2023.4.0b4
 Summary: Utility to simplify Dockerfiles
 Home-page: https://github.com/ModelW/docker/
 License: WTFPL
 Keywords: docker,django,nuxt,dockerfile
 Author: Rémy Sanchez
 Author-email: remy.sanchez@hyperthese.net
 Requires-Python: >=3.10,<4.0
```

