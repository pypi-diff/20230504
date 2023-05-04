# Comparing `tmp/chainbench-0.1.1.tar.gz` & `tmp/chainbench-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainbench-0.1.1.tar", max compression
+gzip compressed data, was "chainbench-0.1.2.tar", max compression
```

## Comparing `chainbench-0.1.1.tar` & `chainbench-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    11357 2023-04-25 15:14:09.028811 chainbench-0.1.1/LICENSE
--rw-r--r--   0        0        0     6162 2023-04-25 15:14:09.028811 chainbench-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-04-25 15:14:09.028811 chainbench-0.1.1/chainbench/__init__.py
--rw-r--r--   0        0        0       39 2023-04-25 15:14:09.028811 chainbench-0.1.1/chainbench/__main__.py
--rw-r--r--   0        0        0     5241 2023-04-25 15:14:09.028811 chainbench-0.1.1/chainbench/main.py
--rw-r--r--   0        0        0        0 2023-04-25 15:14:09.028811 chainbench-0.1.1/chainbench/profile/__init__.py
--rw-r--r--   0        0        0     3417 2023-04-25 15:14:09.028811 chainbench-0.1.1/chainbench/profile/avalanche.py
--rw-r--r--   0        0        0     2512 2023-04-25 15:14:09.028811 chainbench-0.1.1/chainbench/profile/bsc.py
--rw-r--r--   0        0        0     2794 2023-04-25 15:14:09.028811 chainbench-0.1.1/chainbench/profile/ethereum.py
--rw-r--r--   0        0        0     1829 2023-04-25 15:14:09.028811 chainbench-0.1.1/chainbench/profile/oasis.py
--rw-r--r--   0        0        0     2730 2023-04-25 15:14:09.028811 chainbench-0.1.1/chainbench/profile/polygon.py
--rw-r--r--   0        0        0      168 2023-04-25 15:14:09.028811 chainbench-0.1.1/chainbench/test_data/__init__.py
--rw-r--r--   0        0        0     4705 2023-04-25 15:14:09.028811 chainbench-0.1.1/chainbench/test_data/base.py
--rw-r--r--   0        0        0      166 2023-04-25 15:14:09.028811 chainbench-0.1.1/chainbench/test_data/dummy.py
--rw-r--r--   0        0        0     2596 2023-04-25 15:14:09.028811 chainbench-0.1.1/chainbench/test_data/evm.py
--rw-r--r--   0        0        0        0 2023-04-25 15:14:09.028811 chainbench-0.1.1/chainbench/user/__init__.py
--rw-r--r--   0        0        0     3477 2023-04-25 15:14:09.028811 chainbench-0.1.1/chainbench/user/base.py
--rw-r--r--   0        0        0     1225 2023-04-25 15:14:09.028811 chainbench-0.1.1/chainbench/user/evm.py
--rw-r--r--   0        0        0        0 2023-04-25 15:14:09.028811 chainbench-0.1.1/chainbench/util/__init__.py
--rw-r--r--   0        0        0     2499 2023-04-25 15:14:09.028811 chainbench-0.1.1/chainbench/util/cli.py
--rw-r--r--   0        0        0     2532 2023-04-25 15:14:09.028811 chainbench-0.1.1/chainbench/util/event.py
--rw-r--r--   0        0        0     3463 2023-04-25 15:14:09.028811 chainbench-0.1.1/chainbench/util/notify.py
--rw-r--r--   0        0        0      320 2023-04-25 15:14:09.028811 chainbench-0.1.1/chainbench/util/rpc.py
--rw-r--r--   0        0        0      438 2023-04-25 15:14:09.028811 chainbench-0.1.1/chainbench/util/timer.py
--rw-r--r--   0        0        0      746 2023-04-25 15:14:09.028811 chainbench-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     6628 1970-01-01 00:00:00.000000 chainbench-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-04 10:39:14.437426 chainbench-0.1.2/LICENSE
+-rw-r--r--   0        0        0     6162 2023-05-04 10:39:14.437426 chainbench-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-04 10:39:14.437426 chainbench-0.1.2/chainbench/__init__.py
+-rw-r--r--   0        0        0       39 2023-05-04 10:39:14.437426 chainbench-0.1.2/chainbench/__main__.py
+-rw-r--r--   0        0        0     5241 2023-05-04 10:39:14.437426 chainbench-0.1.2/chainbench/main.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:39:14.437426 chainbench-0.1.2/chainbench/profile/__init__.py
+-rw-r--r--   0        0        0     3417 2023-05-04 10:39:14.437426 chainbench-0.1.2/chainbench/profile/avalanche.py
+-rw-r--r--   0        0        0     2512 2023-05-04 10:39:14.437426 chainbench-0.1.2/chainbench/profile/bsc.py
+-rw-r--r--   0        0        0     2794 2023-05-04 10:39:14.437426 chainbench-0.1.2/chainbench/profile/ethereum.py
+-rw-r--r--   0        0        0     1829 2023-05-04 10:39:14.437426 chainbench-0.1.2/chainbench/profile/oasis.py
+-rw-r--r--   0        0        0     2730 2023-05-04 10:39:14.437426 chainbench-0.1.2/chainbench/profile/polygon.py
+-rw-r--r--   0        0        0      168 2023-05-04 10:39:14.437426 chainbench-0.1.2/chainbench/test_data/__init__.py
+-rw-r--r--   0        0        0     4705 2023-05-04 10:39:14.437426 chainbench-0.1.2/chainbench/test_data/base.py
+-rw-r--r--   0        0        0      166 2023-05-04 10:39:14.437426 chainbench-0.1.2/chainbench/test_data/dummy.py
+-rw-r--r--   0        0        0     2596 2023-05-04 10:39:14.441426 chainbench-0.1.2/chainbench/test_data/evm.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:39:14.441426 chainbench-0.1.2/chainbench/user/__init__.py
+-rw-r--r--   0        0        0     3438 2023-05-04 10:39:14.441426 chainbench-0.1.2/chainbench/user/base.py
+-rw-r--r--   0        0        0     1225 2023-05-04 10:39:14.441426 chainbench-0.1.2/chainbench/user/evm.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:39:14.441426 chainbench-0.1.2/chainbench/util/__init__.py
+-rw-r--r--   0        0        0     2499 2023-05-04 10:39:14.441426 chainbench-0.1.2/chainbench/util/cli.py
+-rw-r--r--   0        0        0     2532 2023-05-04 10:39:14.441426 chainbench-0.1.2/chainbench/util/event.py
+-rw-r--r--   0        0        0     3463 2023-05-04 10:39:14.441426 chainbench-0.1.2/chainbench/util/notify.py
+-rw-r--r--   0        0        0      320 2023-05-04 10:39:14.441426 chainbench-0.1.2/chainbench/util/rpc.py
+-rw-r--r--   0        0        0      438 2023-05-04 10:39:14.441426 chainbench-0.1.2/chainbench/util/timer.py
+-rw-r--r--   0        0        0      746 2023-05-04 10:39:14.441426 chainbench-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     6628 1970-01-01 00:00:00.000000 chainbench-0.1.2/PKG-INFO
```

### Comparing `chainbench-0.1.1/LICENSE` & `chainbench-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chainbench-0.1.1/README.md` & `chainbench-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `chainbench-0.1.1/chainbench/main.py` & `chainbench-0.1.2/chainbench/main.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.1.1/chainbench/profile/avalanche.py` & `chainbench-0.1.2/chainbench/profile/avalanche.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.1.1/chainbench/profile/bsc.py` & `chainbench-0.1.2/chainbench/profile/bsc.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.1.1/chainbench/profile/ethereum.py` & `chainbench-0.1.2/chainbench/profile/ethereum.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.1.1/chainbench/profile/oasis.py` & `chainbench-0.1.2/chainbench/profile/oasis.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.1.1/chainbench/profile/polygon.py` & `chainbench-0.1.2/chainbench/profile/polygon.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.1.1/chainbench/test_data/base.py` & `chainbench-0.1.2/chainbench/test_data/base.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.1.1/chainbench/test_data/evm.py` & `chainbench-0.1.2/chainbench/test_data/evm.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.1.1/chainbench/user/base.py` & `chainbench-0.1.2/chainbench/user/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 import logging
 import typing as t
 
-from locust import FastHttpUser, between
+from locust import FastHttpUser
 from locust.contrib.fasthttp import RestResponseContextManager
 from locust.exception import RescheduleTask
 
 from chainbench.test_data import BaseTestData, DummyTestData
 from chainbench.util.event import setup_event_listeners
 from chainbench.util.rpc import generate_request
 
 setup_event_listeners()
 
 
 class BaseBenchUser(FastHttpUser):
     """Base class for all benchmark users."""
 
     abstract = True
-    wait_time = between(0, 2)
 
     rpc_path: str = ""
 
     connection_timeout = 120
     network_timeout = 360
 
     test_data: BaseTestData = DummyTestData()
```

### Comparing `chainbench-0.1.1/chainbench/user/evm.py` & `chainbench-0.1.2/chainbench/user/evm.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.1.1/chainbench/util/cli.py` & `chainbench-0.1.2/chainbench/util/cli.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.1.1/chainbench/util/event.py` & `chainbench-0.1.2/chainbench/util/event.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.1.1/chainbench/util/notify.py` & `chainbench-0.1.2/chainbench/util/notify.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.1.1/pyproject.toml` & `chainbench-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chainbench"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Egor Molodik <egor.molodik@chainstack.com>"]
 readme = "README.md"
 packages = [{include = "chainbench"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `chainbench-0.1.1/PKG-INFO` & `chainbench-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainbench
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Egor Molodik
 Author-email: egor.molodik@chainstack.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

