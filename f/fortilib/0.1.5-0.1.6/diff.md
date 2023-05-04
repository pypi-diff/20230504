# Comparing `tmp/fortilib-0.1.5.tar.gz` & `tmp/fortilib-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fortilib-0.1.5.tar", max compression
+gzip compressed data, was "fortilib-0.1.6.tar", max compression
```

## Comparing `fortilib-0.1.5.tar` & `fortilib-0.1.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    35149 2023-03-21 14:58:40.601294 fortilib-0.1.5/LICENSE
--rw-r--r--   0        0        0     1423 2023-03-21 14:58:40.601294 fortilib-0.1.5/README.md
--rw-r--r--   0        0        0      530 2023-03-21 14:58:40.605294 fortilib-0.1.5/fortilib/__init__.py
--rw-r--r--   0        0        0     4616 2023-03-21 14:58:40.605294 fortilib-0.1.5/fortilib/address.py
--rw-r--r--   0        0        0     1456 2023-03-21 14:58:40.605294 fortilib-0.1.5/fortilib/addressgroup.py
--rw-r--r--   0        0        0     1925 2023-03-21 14:58:40.605294 fortilib-0.1.5/fortilib/base.py
--rw-r--r--   0        0        0     1403 2023-03-21 14:58:40.605294 fortilib-0.1.5/fortilib/exceptions.py
--rw-r--r--   0        0        0    30493 2023-03-21 14:58:40.605294 fortilib-0.1.5/fortilib/firewall.py
--rw-r--r--   0        0        0    35749 2023-03-21 14:58:40.605294 fortilib-0.1.5/fortilib/fortigateapi.py
--rw-r--r--   0        0        0      338 2023-03-21 14:58:40.605294 fortilib-0.1.5/fortilib/fortilib.iml
--rw-r--r--   0        0        0     1625 2023-03-21 14:58:40.605294 fortilib-0.1.5/fortilib/interface.py
--rw-r--r--   0        0        0     2186 2023-03-21 14:58:40.605294 fortilib-0.1.5/fortilib/ippool.py
--rw-r--r--   0        0        0        0 2023-03-21 14:58:40.605294 fortilib-0.1.5/fortilib/mixins/__init__.py
--rw-r--r--   0        0        0      637 2023-03-21 14:58:40.605294 fortilib-0.1.5/fortilib/mixins/group.py
--rw-r--r--   0        0        0      635 2023-03-21 14:58:40.605294 fortilib-0.1.5/fortilib/mixins/interface.py
--rw-r--r--   0        0        0    10030 2023-03-21 14:58:40.605294 fortilib-0.1.5/fortilib/policy.py
--rw-r--r--   0        0        0     1690 2023-03-21 14:58:40.605294 fortilib-0.1.5/fortilib/proxyaddress.py
--rw-r--r--   0        0        0     1760 2023-03-21 14:58:40.605294 fortilib-0.1.5/fortilib/proxyaddressgroup.py
--rw-r--r--   0        0        0    10406 2023-03-21 14:58:40.605294 fortilib-0.1.5/fortilib/proxypolicy.py
--rw-r--r--   0        0        0     2918 2023-03-21 14:58:40.605294 fortilib-0.1.5/fortilib/routes.py
--rw-r--r--   0        0        0     6579 2023-03-21 14:58:40.605294 fortilib-0.1.5/fortilib/service.py
--rw-r--r--   0        0        0     1682 2023-03-21 14:58:40.605294 fortilib-0.1.5/fortilib/servicegroup.py
--rw-r--r--   0        0        0     5249 2023-03-21 14:58:40.605294 fortilib-0.1.5/fortilib/vip.py
--rw-r--r--   0        0        0     1795 2023-03-21 14:58:40.605294 fortilib-0.1.5/fortilib/vipgroup.py
--rw-r--r--   0        0        0      875 2023-03-21 14:58:40.605294 fortilib-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1971 1970-01-01 00:00:00.000000 fortilib-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-04 08:28:19.946205 fortilib-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1423 2023-05-04 08:28:19.946205 fortilib-0.1.6/README.md
+-rw-r--r--   0        0        0      530 2023-05-04 08:28:19.946205 fortilib-0.1.6/fortilib/__init__.py
+-rw-r--r--   0        0        0     4616 2023-05-04 08:28:19.946205 fortilib-0.1.6/fortilib/address.py
+-rw-r--r--   0        0        0     1456 2023-05-04 08:28:19.946205 fortilib-0.1.6/fortilib/addressgroup.py
+-rw-r--r--   0        0        0     1925 2023-05-04 08:28:19.946205 fortilib-0.1.6/fortilib/base.py
+-rw-r--r--   0        0        0     1403 2023-05-04 08:28:19.946205 fortilib-0.1.6/fortilib/exceptions.py
+-rw-r--r--   0        0        0    30493 2023-05-04 08:28:19.946205 fortilib-0.1.6/fortilib/firewall.py
+-rw-r--r--   0        0        0    35749 2023-05-04 08:28:19.946205 fortilib-0.1.6/fortilib/fortigateapi.py
+-rw-r--r--   0        0        0      338 2023-05-04 08:28:19.946205 fortilib-0.1.6/fortilib/fortilib.iml
+-rw-r--r--   0        0        0     1625 2023-05-04 08:28:19.946205 fortilib-0.1.6/fortilib/interface.py
+-rw-r--r--   0        0        0     2186 2023-05-04 08:28:19.946205 fortilib-0.1.6/fortilib/ippool.py
+-rw-r--r--   0        0        0        0 2023-05-04 08:28:19.946205 fortilib-0.1.6/fortilib/mixins/__init__.py
+-rw-r--r--   0        0        0      637 2023-05-04 08:28:19.946205 fortilib-0.1.6/fortilib/mixins/group.py
+-rw-r--r--   0        0        0      635 2023-05-04 08:28:19.946205 fortilib-0.1.6/fortilib/mixins/interface.py
+-rw-r--r--   0        0        0    10030 2023-05-04 08:28:19.946205 fortilib-0.1.6/fortilib/policy.py
+-rw-r--r--   0        0        0     1690 2023-05-04 08:28:19.946205 fortilib-0.1.6/fortilib/proxyaddress.py
+-rw-r--r--   0        0        0     1760 2023-05-04 08:28:19.946205 fortilib-0.1.6/fortilib/proxyaddressgroup.py
+-rw-r--r--   0        0        0    10406 2023-05-04 08:28:19.946205 fortilib-0.1.6/fortilib/proxypolicy.py
+-rw-r--r--   0        0        0     2918 2023-05-04 08:28:19.946205 fortilib-0.1.6/fortilib/routes.py
+-rw-r--r--   0        0        0     6579 2023-05-04 08:28:19.946205 fortilib-0.1.6/fortilib/service.py
+-rw-r--r--   0        0        0     1682 2023-05-04 08:28:19.946205 fortilib-0.1.6/fortilib/servicegroup.py
+-rw-r--r--   0        0        0     5249 2023-05-04 08:28:19.946205 fortilib-0.1.6/fortilib/vip.py
+-rw-r--r--   0        0        0     1795 2023-05-04 08:28:19.946205 fortilib-0.1.6/fortilib/vipgroup.py
+-rw-r--r--   0        0        0      888 2023-05-04 08:28:19.946205 fortilib-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1963 1970-01-01 00:00:00.000000 fortilib-0.1.6/PKG-INFO
```

### Comparing `fortilib-0.1.5/LICENSE` & `fortilib-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fortilib-0.1.5/README.md` & `fortilib-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `fortilib-0.1.5/fortilib/__init__.py` & `fortilib-0.1.6/fortilib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.1.5"
+__version__ = "0.1.6"
 
 from typing import (
     Dict,
     List,
 )
```

### Comparing `fortilib-0.1.5/fortilib/address.py` & `fortilib-0.1.6/fortilib/address.py`

 * *Files identical despite different names*

### Comparing `fortilib-0.1.5/fortilib/addressgroup.py` & `fortilib-0.1.6/fortilib/addressgroup.py`

 * *Files identical despite different names*

### Comparing `fortilib-0.1.5/fortilib/base.py` & `fortilib-0.1.6/fortilib/base.py`

 * *Files identical despite different names*

### Comparing `fortilib-0.1.5/fortilib/exceptions.py` & `fortilib-0.1.6/fortilib/exceptions.py`

 * *Files identical despite different names*

### Comparing `fortilib-0.1.5/fortilib/firewall.py` & `fortilib-0.1.6/fortilib/firewall.py`

 * *Files identical despite different names*

### Comparing `fortilib-0.1.5/fortilib/fortigateapi.py` & `fortilib-0.1.6/fortilib/fortigateapi.py`

 * *Files identical despite different names*

### Comparing `fortilib-0.1.5/fortilib/interface.py` & `fortilib-0.1.6/fortilib/interface.py`

 * *Files identical despite different names*

### Comparing `fortilib-0.1.5/fortilib/ippool.py` & `fortilib-0.1.6/fortilib/ippool.py`

 * *Files identical despite different names*

### Comparing `fortilib-0.1.5/fortilib/mixins/group.py` & `fortilib-0.1.6/fortilib/mixins/group.py`

 * *Files identical despite different names*

### Comparing `fortilib-0.1.5/fortilib/mixins/interface.py` & `fortilib-0.1.6/fortilib/mixins/interface.py`

 * *Files identical despite different names*

### Comparing `fortilib-0.1.5/fortilib/policy.py` & `fortilib-0.1.6/fortilib/policy.py`

 * *Files identical despite different names*

### Comparing `fortilib-0.1.5/fortilib/proxyaddress.py` & `fortilib-0.1.6/fortilib/proxyaddress.py`

 * *Files identical despite different names*

### Comparing `fortilib-0.1.5/fortilib/proxyaddressgroup.py` & `fortilib-0.1.6/fortilib/proxyaddressgroup.py`

 * *Files identical despite different names*

### Comparing `fortilib-0.1.5/fortilib/proxypolicy.py` & `fortilib-0.1.6/fortilib/proxypolicy.py`

 * *Files identical despite different names*

### Comparing `fortilib-0.1.5/fortilib/routes.py` & `fortilib-0.1.6/fortilib/routes.py`

 * *Files identical despite different names*

### Comparing `fortilib-0.1.5/fortilib/service.py` & `fortilib-0.1.6/fortilib/service.py`

 * *Files identical despite different names*

### Comparing `fortilib-0.1.5/fortilib/servicegroup.py` & `fortilib-0.1.6/fortilib/servicegroup.py`

 * *Files identical despite different names*

### Comparing `fortilib-0.1.5/fortilib/vip.py` & `fortilib-0.1.6/fortilib/vip.py`

 * *Files identical despite different names*

### Comparing `fortilib-0.1.5/fortilib/vipgroup.py` & `fortilib-0.1.6/fortilib/vipgroup.py`

 * *Files identical despite different names*

### Comparing `fortilib-0.1.5/pyproject.toml` & `fortilib-0.1.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [tool.poetry]
 name = "fortilib"
-version = "0.1.5"
+version = "0.1.6"
 description = "fortilib - a Python Library to interact with Fortigate Firewalls"
 readme = "README.md"
 authors = [
     "Daniel Zinke <Daniel.Zinke@t-systems.com>",
     "Benjamin Böhm <Benjamin.Boehm@t-systems.com>",
     "Philipp Funk <Philipp.Funk@t-systems.com>",
     "André Ellguth <Andre.Ellguth@t-systems.com>",
     "Martin Neubert <Martin.Neubert@t-systems.com>"
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
-httpx = "^0.23.0"
+httpx = ">=0.23.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.1.2"
-tox = "^4.0.0"
-black = "^22.6.0"
-isort = "^5.10.1"
-coverage = "^6.4.2"
-pytest-integration = "^0.2.2"
-pytest-cov = "^4.0.0"
-pytest-order = "^1.0.1"
-Sphinx = "^5.1.1"
-flake8 = "^5.0.4"
-flake8-gl-codeclimate = "^0.1.6"
-sphinx-rtd-theme = "^1.0.0"
+pytest = ">=7.1.2"
+tox = ">=4.0.0"
+black = ">=22.6.0"
+isort = ">=5.10.1"
+coverage = ">=6.4.2"
+pytest-integration = ">=0.2.2"
+pytest-cov = ">=4.0.0"
+pytest-order = ">=1.0.1"
+Sphinx = ">=5.1.1"
+flake8 = ">=5.0.4"
+flake8-gl-codeclimate = ">=0.1.6"
+sphinx-rtd-theme = ">=1.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `fortilib-0.1.5/PKG-INFO` & `fortilib-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: fortilib
-Version: 0.1.5
+Version: 0.1.6
 Summary: fortilib - a Python Library to interact with Fortigate Firewalls
 Author: Daniel Zinke
 Author-email: Daniel.Zinke@t-systems.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: httpx (>=0.23.0,<0.24.0)
+Requires-Dist: httpx (>=0.23.0)
 Description-Content-Type: text/markdown
 
 # fortilib - a Python Library to interact with Fortigate Firewalls
 
 This Python module contains the ability to get and configure following object on [Fortigate Firewalls](https://www.fortinet.com/products/next-generation-firewall):
 * Addresses
 * Address Groups
```

