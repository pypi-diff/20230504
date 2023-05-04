# Comparing `tmp/qoqo_myqlm-0.4.4.tar.gz` & `tmp/qoqo_myqlm-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qoqo_myqlm-0.4.4.tar", last modified: Mon Apr  3 14:48:25 2023, max compression
+gzip compressed data, was "qoqo_myqlm-0.4.6.tar", last modified: Thu May  4 12:07:48 2023, max compression
```

## Comparing `qoqo_myqlm-0.4.4.tar` & `qoqo_myqlm-0.4.6.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:48:25.144875 qoqo_myqlm-0.4.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:48:25.144875 qoqo_myqlm-0.4.4/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-03 14:48:06.000000 qoqo_myqlm-0.4.4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:48:25.144875 qoqo_myqlm-0.4.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-03 14:48:06.000000 qoqo_myqlm-0.4.4/.github/workflows/build_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-03 14:48:06.000000 qoqo_myqlm-0.4.4/.github/workflows/hqs-ci-lint-and-test-python.yml
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-03 14:48:06.000000 qoqo_myqlm-0.4.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-03 14:48:06.000000 qoqo_myqlm-0.4.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-03 14:48:06.000000 qoqo_myqlm-0.4.4/CONTRIBUTE.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-03 14:48:06.000000 qoqo_myqlm-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-04-03 14:48:25.144875 qoqo_myqlm-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-04-03 14:48:06.000000 qoqo_myqlm-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:48:25.144875 qoqo_myqlm-0.4.4/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-03 14:48:06.000000 qoqo_myqlm-0.4.4/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-04-03 14:48:06.000000 qoqo_myqlm-0.4.4/doc/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:48:25.144875 qoqo_myqlm-0.4.4/doc/generated/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:48:25.144875 qoqo_myqlm-0.4.4/doc/generated/generated/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-03 14:48:06.000000 qoqo_myqlm-0.4.4/doc/generated/generated/qoqo_myqlm.MyQLMBackend.rst
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-03 14:48:06.000000 qoqo_myqlm-0.4.4/doc/generated/generated/qoqo_myqlm.myqlm_call_circuit.rst
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-03 14:48:06.000000 qoqo_myqlm-0.4.4/doc/generated/generated/qoqo_myqlm.myqlm_call_operation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-03 14:48:06.000000 qoqo_myqlm-0.4.4/doc/generated/qoqo_myqlm.rst
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-03 14:48:06.000000 qoqo_myqlm-0.4.4/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-03 14:48:06.000000 qoqo_myqlm-0.4.4/doc/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-03 14:48:06.000000 qoqo_myqlm-0.4.4/doc/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-03 14:48:06.000000 qoqo_myqlm-0.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)   256743 2023-04-03 14:48:06.000000 qoqo_myqlm-0.4.4/qoqo_Logo_vertical_color.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:48:25.144875 qoqo_myqlm-0.4.4/qoqo_myqlm/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-03 14:48:06.000000 qoqo_myqlm-0.4.4/qoqo_myqlm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:48:25.144875 qoqo_myqlm-0.4.4/qoqo_myqlm/backend/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-03 14:48:06.000000 qoqo_myqlm-0.4.4/qoqo_myqlm/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:48:25.144875 qoqo_myqlm-0.4.4/qoqo_myqlm/backend/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-03 14:48:06.000000 qoqo_myqlm-0.4.4/qoqo_myqlm/backend/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     6091 2023-04-03 14:48:06.000000 qoqo_myqlm-0.4.4/qoqo_myqlm/backend/__pycache__/myqlm_backend.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     9288 2023-04-03 14:48:06.000000 qoqo_myqlm-0.4.4/qoqo_myqlm/backend/myqlm_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:48:25.144875 qoqo_myqlm-0.4.4/qoqo_myqlm/interface/
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-03 14:48:06.000000 qoqo_myqlm-0.4.4/qoqo_myqlm/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-04-03 14:48:06.000000 qoqo_myqlm-0.4.4/qoqo_myqlm/interface/myqlm_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:48:25.144875 qoqo_myqlm-0.4.4/qoqo_myqlm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-04-03 14:48:25.000000 qoqo_myqlm-0.4.4/qoqo_myqlm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-03 14:48:25.000000 qoqo_myqlm-0.4.4/qoqo_myqlm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 14:48:25.000000 qoqo_myqlm-0.4.4/qoqo_myqlm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-03 14:48:25.000000 qoqo_myqlm-0.4.4/qoqo_myqlm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-03 14:48:25.000000 qoqo_myqlm-0.4.4/qoqo_myqlm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 14:48:25.144875 qoqo_myqlm-0.4.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:48:25.140875 qoqo_myqlm-0.4.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:48:25.144875 qoqo_myqlm-0.4.4/tests/backend/
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-04-03 14:48:06.000000 qoqo_myqlm-0.4.4/tests/backend/test_myqlm_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:48:25.144875 qoqo_myqlm-0.4.4/tests/interface/
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-03 14:48:06.000000 qoqo_myqlm-0.4.4/tests/interface/test_myqlm_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:07:48.894777 qoqo_myqlm-0.4.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:07:48.890777 qoqo_myqlm-0.4.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-04 12:07:25.000000 qoqo_myqlm-0.4.6/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:07:48.890777 qoqo_myqlm-0.4.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-04 12:07:25.000000 qoqo_myqlm-0.4.6/.github/workflows/build_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-04 12:07:25.000000 qoqo_myqlm-0.4.6/.github/workflows/hqs-ci-lint-and-test-python.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-04 12:07:25.000000 qoqo_myqlm-0.4.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-04 12:07:25.000000 qoqo_myqlm-0.4.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-04 12:07:25.000000 qoqo_myqlm-0.4.6/CONTRIBUTE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-04 12:07:25.000000 qoqo_myqlm-0.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-05-04 12:07:48.894777 qoqo_myqlm-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-04 12:07:25.000000 qoqo_myqlm-0.4.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:07:48.890777 qoqo_myqlm-0.4.6/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-04 12:07:25.000000 qoqo_myqlm-0.4.6/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-05-04 12:07:25.000000 qoqo_myqlm-0.4.6/doc/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:07:48.890777 qoqo_myqlm-0.4.6/doc/generated/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:07:48.890777 qoqo_myqlm-0.4.6/doc/generated/generated/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-04 12:07:25.000000 qoqo_myqlm-0.4.6/doc/generated/generated/qoqo_myqlm.MyQLMBackend.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-04 12:07:25.000000 qoqo_myqlm-0.4.6/doc/generated/generated/qoqo_myqlm.myqlm_call_circuit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-04 12:07:25.000000 qoqo_myqlm-0.4.6/doc/generated/generated/qoqo_myqlm.myqlm_call_operation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-04 12:07:25.000000 qoqo_myqlm-0.4.6/doc/generated/qoqo_myqlm.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-04 12:07:25.000000 qoqo_myqlm-0.4.6/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-04 12:07:25.000000 qoqo_myqlm-0.4.6/doc/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-04 12:07:25.000000 qoqo_myqlm-0.4.6/doc/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-04 12:07:25.000000 qoqo_myqlm-0.4.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)   256743 2023-05-04 12:07:25.000000 qoqo_myqlm-0.4.6/qoqo_Logo_vertical_color.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:07:48.890777 qoqo_myqlm-0.4.6/qoqo_myqlm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-04 12:07:25.000000 qoqo_myqlm-0.4.6/qoqo_myqlm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:07:48.894777 qoqo_myqlm-0.4.6/qoqo_myqlm/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-04 12:07:25.000000 qoqo_myqlm-0.4.6/qoqo_myqlm/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:07:48.894777 qoqo_myqlm-0.4.6/qoqo_myqlm/backend/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-04 12:07:25.000000 qoqo_myqlm-0.4.6/qoqo_myqlm/backend/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     6091 2023-05-04 12:07:25.000000 qoqo_myqlm-0.4.6/qoqo_myqlm/backend/__pycache__/myqlm_backend.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     9288 2023-05-04 12:07:25.000000 qoqo_myqlm-0.4.6/qoqo_myqlm/backend/myqlm_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:07:48.894777 qoqo_myqlm-0.4.6/qoqo_myqlm/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-04 12:07:25.000000 qoqo_myqlm-0.4.6/qoqo_myqlm/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-05-04 12:07:25.000000 qoqo_myqlm-0.4.6/qoqo_myqlm/interface/myqlm_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:07:48.894777 qoqo_myqlm-0.4.6/qoqo_myqlm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-05-04 12:07:48.000000 qoqo_myqlm-0.4.6/qoqo_myqlm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-04 12:07:48.000000 qoqo_myqlm-0.4.6/qoqo_myqlm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 12:07:48.000000 qoqo_myqlm-0.4.6/qoqo_myqlm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-04 12:07:48.000000 qoqo_myqlm-0.4.6/qoqo_myqlm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-04 12:07:48.000000 qoqo_myqlm-0.4.6/qoqo_myqlm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 12:07:48.894777 qoqo_myqlm-0.4.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:07:48.890777 qoqo_myqlm-0.4.6/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:07:48.894777 qoqo_myqlm-0.4.6/tests/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-04 12:07:25.000000 qoqo_myqlm-0.4.6/tests/backend/test_myqlm_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:07:48.894777 qoqo_myqlm-0.4.6/tests/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-04 12:07:25.000000 qoqo_myqlm-0.4.6/tests/interface/test_myqlm_interface.py
```

### Comparing `qoqo_myqlm-0.4.4/.github/workflows/hqs-ci-lint-and-test-python.yml` & `qoqo_myqlm-0.4.6/.github/workflows/hqs-ci-lint-and-test-python.yml`

 * *Files identical despite different names*

### Comparing `qoqo_myqlm-0.4.4/CONTRIBUTE.md` & `qoqo_myqlm-0.4.6/CONTRIBUTE.md`

 * *Files identical despite different names*

### Comparing `qoqo_myqlm-0.4.4/LICENSE` & `qoqo_myqlm-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `qoqo_myqlm-0.4.4/PKG-INFO` & `qoqo_myqlm-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qoqo_myqlm
-Version: 0.4.4
+Version: 0.4.6
 Summary: An inteface to execute circuits from QOQO to MYQLM
 Author-email: HQS Quantum Simulation GmbH <info@quantumsimulations.de>
 Requires-Python: <3.11,>3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `qoqo_myqlm-0.4.4/README.md` & `qoqo_myqlm-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `qoqo_myqlm-0.4.4/doc/Makefile` & `qoqo_myqlm-0.4.6/doc/Makefile`

 * *Files identical despite different names*

### Comparing `qoqo_myqlm-0.4.4/doc/conf.py` & `qoqo_myqlm-0.4.6/doc/conf.py`

 * *Files identical despite different names*

### Comparing `qoqo_myqlm-0.4.4/pyproject.toml` & `qoqo_myqlm-0.4.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "qoqo_myqlm"
-version = "0.4.4"
+version = "0.4.6"
 description = "An inteface to execute circuits from QOQO to MYQLM"
 authors = [{name="HQS Quantum Simulation GmbH", email="info@quantumsimulations.de"}]
 readme = "README.md"
 requires-python = ">3.8, <3.11"
 dependencies = [
-    "qoqo>=1.2",
+    "qoqo>=1.4",
     'qoqo_calculator_pyo3>=1.1',
     "numpy",
     'myqlm'
 ]
 [project.optional-dependencies]
 tests = [
   'pytest',
```

### Comparing `qoqo_myqlm-0.4.4/qoqo_Logo_vertical_color.png` & `qoqo_myqlm-0.4.6/qoqo_Logo_vertical_color.png`

 * *Files identical despite different names*

### Comparing `qoqo_myqlm-0.4.4/qoqo_myqlm/__init__.py` & `qoqo_myqlm-0.4.6/qoqo_myqlm/__init__.py`

 * *Files identical despite different names*

### Comparing `qoqo_myqlm-0.4.4/qoqo_myqlm/backend/__init__.py` & `qoqo_myqlm-0.4.6/qoqo_myqlm/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `qoqo_myqlm-0.4.4/qoqo_myqlm/backend/__pycache__/myqlm_backend.cpython-38.pyc` & `qoqo_myqlm-0.4.6/qoqo_myqlm/backend/__pycache__/myqlm_backend.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `qoqo_myqlm-0.4.4/qoqo_myqlm/backend/myqlm_backend.py` & `qoqo_myqlm-0.4.6/qoqo_myqlm/backend/myqlm_backend.py`

 * *Files identical despite different names*

### Comparing `qoqo_myqlm-0.4.4/qoqo_myqlm/interface/__init__.py` & `qoqo_myqlm-0.4.6/qoqo_myqlm/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `qoqo_myqlm-0.4.4/qoqo_myqlm/interface/myqlm_interface.py` & `qoqo_myqlm-0.4.6/qoqo_myqlm/interface/myqlm_interface.py`

 * *Files identical despite different names*

### Comparing `qoqo_myqlm-0.4.4/qoqo_myqlm.egg-info/PKG-INFO` & `qoqo_myqlm-0.4.6/qoqo_myqlm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qoqo-myqlm
-Version: 0.4.4
+Version: 0.4.6
 Summary: An inteface to execute circuits from QOQO to MYQLM
 Author-email: HQS Quantum Simulation GmbH <info@quantumsimulations.de>
 Requires-Python: <3.11,>3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `qoqo_myqlm-0.4.4/qoqo_myqlm.egg-info/SOURCES.txt` & `qoqo_myqlm-0.4.6/qoqo_myqlm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qoqo_myqlm-0.4.4/tests/backend/test_myqlm_backend.py` & `qoqo_myqlm-0.4.6/tests/backend/test_myqlm_backend.py`

 * *Files identical despite different names*

### Comparing `qoqo_myqlm-0.4.4/tests/interface/test_myqlm_interface.py` & `qoqo_myqlm-0.4.6/tests/interface/test_myqlm_interface.py`

 * *Files identical despite different names*

