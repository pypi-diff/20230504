# Comparing `tmp/modelw_docker-2023.3.1.tar.gz` & `tmp/modelw_docker-2023.4.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelw_docker-2023.3.1.tar", max compression
+gzip compressed data, was "modelw_docker-2023.4.0b1.tar", max compression
```

## Comparing `modelw_docker-2023.3.1.tar` & `modelw_docker-2023.4.0b1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      484 2023-04-04 08:49:40.356271 modelw_docker-2023.3.1/LICENSE
--rw-r--r--   0        0        0     4666 2023-04-04 08:49:40.356271 modelw_docker-2023.3.1/README.md
--rw-r--r--   0        0        0     1182 2023-04-04 08:49:40.360271 modelw_docker-2023.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-04 08:49:40.360271 modelw_docker-2023.3.1/src/model_w/docker/__init__.py
--rw-r--r--   0        0        0     2753 2023-04-04 08:49:40.360271 modelw_docker-2023.3.1/src/model_w/docker/__main__.py
--rw-r--r--   0        0        0     1448 2023-04-04 08:49:40.360271 modelw_docker-2023.3.1/src/model_w/docker/build.py
--rw-r--r--   0        0        0     7307 2023-04-04 08:49:40.360271 modelw_docker-2023.3.1/src/model_w/docker/config.py
--rw-r--r--   0        0        0      209 2023-04-04 08:49:40.360271 modelw_docker-2023.3.1/src/model_w/docker/exceptions.py
--rw-r--r--   0        0        0     5183 2023-04-04 08:49:40.360271 modelw_docker-2023.3.1/src/model_w/docker/install.py
--rw-r--r--   0        0        0     7755 2023-04-04 08:49:40.360271 modelw_docker-2023.3.1/src/model_w/docker/output.py
--rw-r--r--   0        0        0     1662 2023-04-04 08:49:40.360271 modelw_docker-2023.3.1/src/model_w/docker/platform.py
--rw-r--r--   0        0        0        0 2023-04-04 08:49:40.360271 modelw_docker-2023.3.1/src/model_w/docker/py.typed
--rw-r--r--   0        0        0     2580 2023-04-04 08:49:40.360271 modelw_docker-2023.3.1/src/model_w/docker/run.py
--rw-r--r--   0        0        0     5915 2023-04-04 08:49:40.360271 modelw_docker-2023.3.1/src/model_w/docker/serve.py
--rw-r--r--   0        0        0     5881 1970-01-01 00:00:00.000000 modelw_docker-2023.3.1/PKG-INFO
+-rw-r--r--   0        0        0      484 2023-05-04 13:52:38.208276 modelw_docker-2023.4.0b1/LICENSE
+-rw-r--r--   0        0        0     4666 2023-05-04 13:52:38.208276 modelw_docker-2023.4.0b1/README.md
+-rw-r--r--   0        0        0     1201 2023-05-04 13:52:38.212276 modelw_docker-2023.4.0b1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-04 13:52:38.212276 modelw_docker-2023.4.0b1/src/model_w/docker/__init__.py
+-rw-r--r--   0        0        0     2753 2023-05-04 13:52:38.212276 modelw_docker-2023.4.0b1/src/model_w/docker/__main__.py
+-rw-r--r--   0        0        0     1494 2023-05-04 13:52:38.212276 modelw_docker-2023.4.0b1/src/model_w/docker/build.py
+-rw-r--r--   0        0        0     7307 2023-05-04 13:52:38.212276 modelw_docker-2023.4.0b1/src/model_w/docker/config.py
+-rw-r--r--   0        0        0      209 2023-05-04 13:52:38.212276 modelw_docker-2023.4.0b1/src/model_w/docker/exceptions.py
+-rw-r--r--   0        0        0     5229 2023-05-04 13:52:38.212276 modelw_docker-2023.4.0b1/src/model_w/docker/install.py
+-rw-r--r--   0        0        0     7755 2023-05-04 13:52:38.212276 modelw_docker-2023.4.0b1/src/model_w/docker/output.py
+-rw-r--r--   0        0        0     1662 2023-05-04 13:52:38.212276 modelw_docker-2023.4.0b1/src/model_w/docker/platform.py
+-rw-r--r--   0        0        0        0 2023-05-04 13:52:38.212276 modelw_docker-2023.4.0b1/src/model_w/docker/py.typed
+-rw-r--r--   0        0        0     2580 2023-05-04 13:52:38.212276 modelw_docker-2023.4.0b1/src/model_w/docker/run.py
+-rw-r--r--   0        0        0     5865 2023-05-04 13:52:38.212276 modelw_docker-2023.4.0b1/src/model_w/docker/serve.py
+-rw-r--r--   0        0        0     5909 1970-01-01 00:00:00.000000 modelw_docker-2023.4.0b1/PKG-INFO
```

### Comparing `modelw_docker-2023.3.1/README.md` & `modelw_docker-2023.4.0b1/README.md`

 * *Files identical despite different names*

### Comparing `modelw_docker-2023.3.1/pyproject.toml` & `modelw_docker-2023.4.0b1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "modelw-docker"
-version = "2023.3.1"
+version = "2023.4.0b1"
 description = "Utility to simplify Dockerfiles"
 authors = ["Rémy Sanchez <remy.sanchez@hyperthese.net>"]
 license = "WTFPL"
 readme = "README.md"
 packages = [{include = "model_w/docker", from = "src"}]
 repository = "https://github.com/ModelW/docker/"
 documentation = "https://github.com/ModelW/docker/"
@@ -23,14 +23,15 @@
 ]
 
 [tool.poetry.scripts]
 modelw-docker = "model_w.docker.__main__:__main__"
 
 [tool.poetry.dependencies]
 python = "^3.10"
+setuptools = "*"
 psutil = "^5.9.4"
 colorama = "^0.4.6"
 tomli = { version = "^2.0.1", python = "<3.11" }
 typefit = "^0.4.2"
 
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `modelw_docker-2023.3.1/src/model_w/docker/__main__.py` & `modelw_docker-2023.4.0b1/src/model_w/docker/__main__.py`

 * *Files identical despite different names*

### Comparing `modelw_docker-2023.3.1/src/model_w/docker/build.py` & `modelw_docker-2023.4.0b1/src/model_w/docker/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,16 @@
     Getting Nuxt to compile itself
     """
 
     printer = Printer.instance()
 
     printer.chapter("Building Nuxt project")
 
+    printer.env_patch["BUILD_MODE"] = "true"
+
     printer.exec(
         "Running Nuxt build",
         path,
         ["npm", "run", "build"],
     )
```

### Comparing `modelw_docker-2023.3.1/src/model_w/docker/config.py` & `modelw_docker-2023.4.0b1/src/model_w/docker/config.py`

 * *Files identical despite different names*

### Comparing `modelw_docker-2023.3.1/src/model_w/docker/install.py` & `modelw_docker-2023.4.0b1/src/model_w/docker/install.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,14 +169,16 @@
 
     printer = Printer.instance()
 
     install_system(config)
 
     printer.chapter("Installing node dependencies")
 
+    printer.env_patch["BUILD_MODE"] = "true"
+
     printer.exec(
         "Installing dependencies",
         path,
         ["npm", "install"],
     )
     printer.exec(
         "Clean NPM cache",
```

### Comparing `modelw_docker-2023.3.1/src/model_w/docker/output.py` & `modelw_docker-2023.4.0b1/src/model_w/docker/output.py`

 * *Files identical despite different names*

### Comparing `modelw_docker-2023.3.1/src/model_w/docker/platform.py` & `modelw_docker-2023.4.0b1/src/model_w/docker/platform.py`

 * *Files identical despite different names*

### Comparing `modelw_docker-2023.3.1/src/model_w/docker/run.py` & `modelw_docker-2023.4.0b1/src/model_w/docker/run.py`

 * *Files identical despite different names*

### Comparing `modelw_docker-2023.3.1/src/model_w/docker/serve.py` & `modelw_docker-2023.4.0b1/src/model_w/docker/serve.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,24 +194,19 @@
     """
 
     printer = Printer.instance()
 
     printer.chapter("Serving Nuxt project")
     port = getenv("PORT", "3000")
 
+    printer.env_patch.update({"HOST": "0.0.0.0", "PORT": f"{port}"})
     printer.handover(
         "Running Nuxt server",
         path,
-        [
-            *["npm", "run"],
-            "start",
-            "--",
-            *["--hostname", "0.0.0.0"],
-            *["--port", f"{port}"],
-        ],
+        ["node", ".output/server/index.mjs"],
     )
 
 
 def serve(config: Config, path: Path, variant: str) -> None:
     """
     Spins up the right server for the project
```

### Comparing `modelw_docker-2023.3.1/PKG-INFO` & `modelw_docker-2023.4.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelw-docker
-Version: 2023.3.1
+Version: 2023.4.0b1
 Summary: Utility to simplify Dockerfiles
 Home-page: https://github.com/ModelW/docker/
 License: WTFPL
 Keywords: docker,django,nuxt,dockerfile
 Author: Rémy Sanchez
 Author-email: remy.sanchez@hyperthese.net
 Requires-Python: >=3.10,<4.0
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Utilities
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: psutil (>=5.9.4,<6.0.0)
+Requires-Dist: setuptools
 Requires-Dist: tomli (>=2.0.1,<3.0.0) ; python_version < "3.11"
 Requires-Dist: typefit (>=0.4.2,<0.5.0)
 Project-URL: Documentation, https://github.com/ModelW/docker/
 Project-URL: Repository, https://github.com/ModelW/docker/
 Description-Content-Type: text/markdown
 
 # Model W Docker
```

