# Comparing `tmp/TigerASI-0.0.8.tar.gz` & `tmp/TigerASI-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TigerASI-0.0.8.tar", last modified: Tue Jan 31 19:36:25 2023, max compression
+gzip compressed data, was "TigerASI-0.0.9.tar", last modified: Tue Jan 31 19:38:52 2023, max compression
```

## Comparing `TigerASI-0.0.8.tar` & `TigerASI-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:36:25.647509 TigerASI-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-01-31 19:36:04.000000 TigerASI-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-01-31 19:36:25.647509 TigerASI-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-01-31 19:36:04.000000 TigerASI-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:36:25.643509 TigerASI-0.0.8/TigerASI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-01-31 19:36:25.000000 TigerASI-0.0.8/TigerASI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-01-31 19:36:25.000000 TigerASI-0.0.8/TigerASI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 19:36:25.000000 TigerASI-0.0.8/TigerASI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-01-31 19:36:25.000000 TigerASI-0.0.8/TigerASI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-31 19:36:25.000000 TigerASI-0.0.8/TigerASI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-31 19:36:25.647509 TigerASI-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-01-31 19:36:05.000000 TigerASI-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:36:25.643509 TigerASI-0.0.8/tigerasi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 19:36:04.000000 TigerASI-0.0.8/tigerasi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-01-31 19:36:04.000000 TigerASI-0.0.8/tigerasi/device_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-01-31 19:36:04.000000 TigerASI-0.0.8/tigerasi/sim_tiger_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    54517 2023-01-31 19:36:04.000000 TigerASI-0.0.8/tigerasi/tiger_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:38:52.591055 TigerASI-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-01-31 19:38:34.000000 TigerASI-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-01-31 19:38:52.591055 TigerASI-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-01-31 19:38:34.000000 TigerASI-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:38:52.591055 TigerASI-0.0.9/TigerASI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-01-31 19:38:52.000000 TigerASI-0.0.9/TigerASI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-01-31 19:38:52.000000 TigerASI-0.0.9/TigerASI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 19:38:52.000000 TigerASI-0.0.9/TigerASI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-01-31 19:38:52.000000 TigerASI-0.0.9/TigerASI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-31 19:38:52.000000 TigerASI-0.0.9/TigerASI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-31 19:38:52.591055 TigerASI-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-01-31 19:38:34.000000 TigerASI-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:38:52.591055 TigerASI-0.0.9/tigerasi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 19:38:34.000000 TigerASI-0.0.9/tigerasi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-01-31 19:38:34.000000 TigerASI-0.0.9/tigerasi/device_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-01-31 19:38:34.000000 TigerASI-0.0.9/tigerasi/sim_tiger_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54517 2023-01-31 19:38:34.000000 TigerASI-0.0.9/tigerasi/tiger_controller.py
```

### Comparing `TigerASI-0.0.8/LICENSE` & `TigerASI-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `TigerASI-0.0.8/PKG-INFO` & `TigerASI-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TigerASI
-Version: 0.0.8
+Version: 0.0.9
 Summary: a lightweight python interface for ASI brand Tiger Controllers
 Home-page: https://github.com/AllenNeuralDynamics/TigerASI
 Author: Joshua Vasquez
 Author-email: joshua.vasquez@alleninstitute.org
 License: MIT
 Keywords: driver,asi,tigercontroller
 Classifier: Development Status :: 4 - Beta
@@ -104,26 +104,22 @@
 This list includes joystick enabling/disabling and remapping, setting stage travel limits, queuing moves into the hardware buffer, and many other more nuanced features.
 For a breakdown of what commands have been exposed, have a look at the [examples folder](https://github.com/AllenNeuralDynamics/TigerASI/tree/main/examples) and the docs.
 
 ## Documentation
 Docs can be generated via Sphinx.
 Stay tuned for docs made available online.
 
-
-
-## Logging
-
 ## Implementation Details
 
 ### Blocking or Non-Blocking?
 All commands to the Tigerbox return a reply.
 Commands that query the Tigerbox state will also return data with that reply.
 
 Waiting for a reply introduces 10-20[ms] of execution time before the function returns an 'ACK'knowledgement.
 By default, methods *will block* until receiving this acknowledgement unless otherwise specified, like this:
 ````python
-box.move_absolute(x=1000, y=25, wait_for_output=False, wait_for_reply=False) # will not block.
+box.move_absolute(x=1000, y=25, wait=False) # will not block.
 ````
 This behavior can only be used for commands to change the Tigerbox state.
 Commands that query the Tigerbox state will always block until they receive a hardware reply.
```

### Comparing `TigerASI-0.0.8/README.md` & `TigerASI-0.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -87,26 +87,22 @@
 This list includes joystick enabling/disabling and remapping, setting stage travel limits, queuing moves into the hardware buffer, and many other more nuanced features.
 For a breakdown of what commands have been exposed, have a look at the [examples folder](https://github.com/AllenNeuralDynamics/TigerASI/tree/main/examples) and the docs.
 
 ## Documentation
 Docs can be generated via Sphinx.
 Stay tuned for docs made available online.
 
-
-
-## Logging
-
 ## Implementation Details
 
 ### Blocking or Non-Blocking?
 All commands to the Tigerbox return a reply.
 Commands that query the Tigerbox state will also return data with that reply.
 
 Waiting for a reply introduces 10-20[ms] of execution time before the function returns an 'ACK'knowledgement.
 By default, methods *will block* until receiving this acknowledgement unless otherwise specified, like this:
 ````python
-box.move_absolute(x=1000, y=25, wait_for_output=False, wait_for_reply=False) # will not block.
+box.move_absolute(x=1000, y=25, wait=False) # will not block.
 ````
 This behavior can only be used for commands to change the Tigerbox state.
 Commands that query the Tigerbox state will always block until they receive a hardware reply.
```

### Comparing `TigerASI-0.0.8/TigerASI.egg-info/PKG-INFO` & `TigerASI-0.0.9/TigerASI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TigerASI
-Version: 0.0.8
+Version: 0.0.9
 Summary: a lightweight python interface for ASI brand Tiger Controllers
 Home-page: https://github.com/AllenNeuralDynamics/TigerASI
 Author: Joshua Vasquez
 Author-email: joshua.vasquez@alleninstitute.org
 License: MIT
 Keywords: driver,asi,tigercontroller
 Classifier: Development Status :: 4 - Beta
@@ -104,26 +104,22 @@
 This list includes joystick enabling/disabling and remapping, setting stage travel limits, queuing moves into the hardware buffer, and many other more nuanced features.
 For a breakdown of what commands have been exposed, have a look at the [examples folder](https://github.com/AllenNeuralDynamics/TigerASI/tree/main/examples) and the docs.
 
 ## Documentation
 Docs can be generated via Sphinx.
 Stay tuned for docs made available online.
 
-
-
-## Logging
-
 ## Implementation Details
 
 ### Blocking or Non-Blocking?
 All commands to the Tigerbox return a reply.
 Commands that query the Tigerbox state will also return data with that reply.
 
 Waiting for a reply introduces 10-20[ms] of execution time before the function returns an 'ACK'knowledgement.
 By default, methods *will block* until receiving this acknowledgement unless otherwise specified, like this:
 ````python
-box.move_absolute(x=1000, y=25, wait_for_output=False, wait_for_reply=False) # will not block.
+box.move_absolute(x=1000, y=25, wait=False) # will not block.
 ````
 This behavior can only be used for commands to change the Tigerbox state.
 Commands that query the Tigerbox state will always block until they receive a hardware reply.
```

### Comparing `TigerASI-0.0.8/setup.py` & `TigerASI-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", newline="", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="TigerASI",
-    version="0.0.8",
+    version="0.0.9",
     author="Joshua Vasquez",
     author_email="joshua.vasquez@alleninstitute.org",
     description="a lightweight python interface for ASI brand Tiger Controllers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AllenNeuralDynamics/TigerASI",
     license="MIT",
```

### Comparing `TigerASI-0.0.8/tigerasi/device_codes.py` & `TigerASI-0.0.9/tigerasi/device_codes.py`

 * *Files identical despite different names*

### Comparing `TigerASI-0.0.8/tigerasi/sim_tiger_controller.py` & `TigerASI-0.0.9/tigerasi/sim_tiger_controller.py`

 * *Files identical despite different names*

### Comparing `TigerASI-0.0.8/tigerasi/tiger_controller.py` & `TigerASI-0.0.9/tigerasi/tiger_controller.py`

 * *Files identical despite different names*

