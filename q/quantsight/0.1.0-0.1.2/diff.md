# Comparing `tmp/quantsight-0.1.0.tar.gz` & `tmp/quantsight-0.1.2.linux-x86_64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantsight-0.1.0.tar", last modified: Thu May  4 12:13:27 2023, max compression
+gzip compressed data, was "quantsight-0.1.2.linux-x86_64.tar", last modified: Thu May  4 13:32:40 2023, max compression
```

## Comparing `quantsight-0.1.0.tar` & `quantsight-0.1.2.linux-x86_64.tar`

### file list

```diff
@@ -1,14 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:13:27.670793 quantsight-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-04 12:13:27.666793 quantsight-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-05-04 12:13:16.000000 quantsight-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:13:27.666793 quantsight-0.1.0/quantsight/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-04 12:13:16.000000 quantsight-0.1.0/quantsight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-04 12:13:16.000000 quantsight-0.1.0/quantsight/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:13:27.666793 quantsight-0.1.0/quantsight.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-04 12:13:27.000000 quantsight-0.1.0/quantsight.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-04 12:13:27.000000 quantsight-0.1.0/quantsight.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 12:13:27.000000 quantsight-0.1.0/quantsight.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-04 12:13:27.000000 quantsight-0.1.0/quantsight.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-04 12:13:27.000000 quantsight-0.1.0/quantsight.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 12:13:27.670793 quantsight-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-04 12:13:16.000000 quantsight-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:32:39.931388 ./
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:32:39.931388 ./opt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:32:39.931388 ./opt/hostedtoolcache/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:32:39.931388 ./opt/hostedtoolcache/Python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:32:39.931388 ./opt/hostedtoolcache/Python/3.11.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:32:39.931388 ./opt/hostedtoolcache/Python/3.11.3/x64/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:32:39.931388 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:32:39.931388 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:32:39.939388 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:32:39.935388 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-04 13:32:30.000000 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:32:39.935388 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-04 13:32:39.935388 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-05-04 13:32:39.935388 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/__pycache__/client.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-04 13:32:30.000000 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:32:39.939388 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight-0.1.2-py3.11.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-05-04 13:32:39.795388 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight-0.1.2-py3.11.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-04 13:32:39.815388 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight-0.1.2-py3.11.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 13:32:39.795388 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight-0.1.2-py3.11.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-04 13:32:39.795388 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight-0.1.2-py3.11.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-04 13:32:39.795388 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight-0.1.2-py3.11.egg-info/top_level.txt
```

### Comparing `quantsight-0.1.0/PKG-INFO` & `./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight-0.1.2-py3.11.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: quantsight
-Version: 0.1.0
+Version: 0.1.2
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
-
+[![Publish to PyPI](https://github.com/Unsigned-Research/quantsight-client/actions/workflows/publish-to-pypi.yml/badge.svg?branch=master)](https://github.com/Unsigned-Research/quantsight-client/actions/workflows/publish-to-pypi.yml) [![PyPI version](https://badge.fury.io/py/quantsight.svg)](https://badge.fury.io/py/quantsight)
 
 <img height="60" src="https://www.quantsight.dev/static/media/trades.2cd0b7149637f5303dd5.png"/>
 
-[![Publish to PyPI](https://github.com/Unsigned-Research/quantsight-client/actions/workflows/publish-to-pypi.yml/badge.svg)](https://github.com/Unsigned-Research/quantsight-client/actions/workflows/publish-to-pypi.yml)
-# Quantsight Data API Python Client
-
 This is a Python client for the Quantsight Data API, which allows you to fetch historical funding rates, candle data, and perform custom queries from supported exchanges. The client is easy to use and supports fetching data into a Pandas DataFrame for further analysis.
 
 ## Installation
 
 To install the Quantsight Data API Python client, use `pip`:
 
 ```bash
```

### Comparing `quantsight-0.1.0/quantsight/client.py` & `./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/client.py`

 * *Files identical despite different names*

