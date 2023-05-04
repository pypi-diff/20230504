# Comparing `tmp/monotonic derivative-0.11.tar.gz` & `tmp/monotonic derivative-0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monotonic derivative-0.11.tar", last modified: Wed May  3 15:25:42 2023, max compression
+gzip compressed data, was "monotonic derivative-0.12.tar", last modified: Thu May  4 08:11:37 2023, max compression
```

## Comparing `monotonic derivative-0.11.tar` & `monotonic derivative-0.12.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:25:42.763061 monotonic derivative-0.11/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-03 15:25:31.000000 monotonic derivative-0.11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-03 15:25:42.763061 monotonic derivative-0.11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-03 15:25:31.000000 monotonic derivative-0.11/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:25:42.763061 monotonic derivative-0.11/monotonic_derivative/
--rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-05-03 15:25:31.000000 monotonic derivative-0.11/monotonic_derivative/monotonic_derivative.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:25:42.763061 monotonic derivative-0.11/monotonic_derivative.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-03 15:25:42.000000 monotonic derivative-0.11/monotonic_derivative.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-03 15:25:42.000000 monotonic derivative-0.11/monotonic_derivative.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 15:25:42.000000 monotonic derivative-0.11/monotonic_derivative.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-03 15:25:42.000000 monotonic derivative-0.11/monotonic_derivative.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-03 15:25:42.000000 monotonic derivative-0.11/monotonic_derivative.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 15:25:42.763061 monotonic derivative-0.11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-03 15:25:31.000000 monotonic derivative-0.11/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:11:37.595023 monotonic derivative-0.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-04 08:11:18.000000 monotonic derivative-0.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-04 08:11:37.595023 monotonic derivative-0.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-04 08:11:18.000000 monotonic derivative-0.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:11:37.591023 monotonic derivative-0.12/monotonic_derivative/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-04 08:11:18.000000 monotonic derivative-0.12/monotonic_derivative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-04 08:11:18.000000 monotonic derivative-0.12/monotonic_derivative/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-05-04 08:11:18.000000 monotonic derivative-0.12/monotonic_derivative/monotonic_derivative.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:11:37.595023 monotonic derivative-0.12/monotonic_derivative.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-04 08:11:37.000000 monotonic derivative-0.12/monotonic_derivative.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-04 08:11:37.000000 monotonic derivative-0.12/monotonic_derivative.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 08:11:37.000000 monotonic derivative-0.12/monotonic_derivative.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-04 08:11:37.000000 monotonic derivative-0.12/monotonic_derivative.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-04 08:11:37.000000 monotonic derivative-0.12/monotonic_derivative.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 08:11:37.595023 monotonic derivative-0.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-04 08:11:18.000000 monotonic derivative-0.12/setup.py
```

### Comparing `monotonic derivative-0.11/LICENSE` & `monotonic derivative-0.12/LICENSE`

 * *Files identical despite different names*

### Comparing `monotonic derivative-0.11/README.md` & `monotonic derivative-0.12/README.md`

 * *Files identical despite different names*

### Comparing `monotonic derivative-0.11/monotonic_derivative/monotonic_derivative.py` & `monotonic derivative-0.12/monotonic_derivative/monotonic_derivative.py`

 * *Files identical despite different names*

### Comparing `monotonic derivative-0.11/setup.py` & `monotonic derivative-0.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
 setup(
     name="monotonic derivative",
-    version="0.11",
+    version="0.12",
     description="Monotonic Derivative is a Python library designed to modify real-life data to ensure that the specified degree derivative of the cubic spline is always monotonically increasing or decreasing. This library can be particularly useful in applications where the derivatives of the given data must follow specific monotonicity constraints, such as in scientific modeling or engineering applications.",
     author="Adam Wecker",
     packages=["monotonic_derivative"],
     install_requires=["numpy", "scipy", "matplotlib", "imageio"],
 )
```

