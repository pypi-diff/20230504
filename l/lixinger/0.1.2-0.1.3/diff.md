# Comparing `tmp/lixinger-0.1.2.tar.gz` & `tmp/lixinger-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lixinger-0.1.2.tar", last modified: Thu May  4 10:40:26 2023, max compression
+gzip compressed data, was "lixinger-0.1.3.tar", last modified: Thu May  4 14:33:31 2023, max compression
```

## Comparing `lixinger-0.1.2.tar` & `lixinger-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,28 @@
--rw-r--r--   0        0        0      705 2023-05-03 10:11:52.615764 lixinger-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-05-01 04:05:58.277552 lixinger-0.1.2/lixinger/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:33:35.225361 lixinger-0.1.2/lixinger/api/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:08:22.152169 lixinger-0.1.2/lixinger/api/cn/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:09:36.967425 lixinger-0.1.2/lixinger/api/cn/company/__init__.py
--rw-r--r--   0        0        0     2132 2023-05-04 10:40:12.138787 lixinger-0.1.2/lixinger/api/cn/company/base.py
--rw-r--r--   0        0        0        0 2023-05-01 05:10:55.043163 lixinger-0.1.2/lixinger/api/cn/index/__init__.py
--rw-r--r--   0        0        0     1721 2023-05-04 10:40:12.140548 lixinger-0.1.2/lixinger/api/cn/index/fundamental.py
--rw-r--r--   0        0        0        0 2023-05-01 04:08:31.838744 lixinger-0.1.2/lixinger/api/hk/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:09:00.179536 lixinger-0.1.2/lixinger/api/macro/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:08:44.656824 lixinger-0.1.2/lixinger/api/us/__init__.py
--rw-r--r--   0        0        0     1582 2023-05-04 10:40:12.141591 lixinger-0.1.2/lixinger/config.py
--rw-r--r--   0        0        0        0 2023-05-03 09:27:58.212202 lixinger-0.1.2/lixinger/py.typed
--rw-r--r--   0        0        0       75 2023-05-03 10:06:41.922780 lixinger-0.1.2/lixinger/settings.toml
--rw-r--r--   0        0        0      978 2023-05-04 10:40:12.142362 lixinger-0.1.2/lixinger/utils.py
--rw-r--r--   0        0        0     1013 2023-05-04 10:40:26.894124 lixinger-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-01 04:43:15.660305 lixinger-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:43:19.505533 lixinger-0.1.2/tests/api/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:43:24.536685 lixinger-0.1.2/tests/api/cn/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:43:30.757795 lixinger-0.1.2/tests/api/cn/company/__init__.py
--rw-r--r--   0        0        0      127 2023-05-03 10:00:15.081563 lixinger-0.1.2/tests/api/cn/company/test_base.py
--rw-r--r--   0        0        0        0 2023-05-01 05:16:11.323717 lixinger-0.1.2/tests/api/cn/index/__init__.py
--rw-r--r--   0        0        0      270 2023-05-03 09:27:22.076125 lixinger-0.1.2/tests/api/cn/index/test_fundamental.py
--rw-r--r--   0        0        0     1444 1970-01-01 00:00:00.000000 lixinger-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      705 2023-05-03 10:11:52.615764 lixinger-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-01 04:05:58.277552 lixinger-0.1.3/lixinger/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:33:35.225361 lixinger-0.1.3/lixinger/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:08:22.152169 lixinger-0.1.3/lixinger/api/cn/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:09:36.967425 lixinger-0.1.3/lixinger/api/cn/company/__init__.py
+-rw-r--r--   0        0        0     2132 2023-05-04 10:40:12.138787 lixinger-0.1.3/lixinger/api/cn/company/base.py
+-rw-r--r--   0        0        0        0 2023-05-04 14:21:25.826889 lixinger-0.1.3/lixinger/api/cn/fund/__init__.py
+-rw-r--r--   0        0        0     1161 2023-05-04 14:31:57.646244 lixinger-0.1.3/lixinger/api/cn/fund/total_net_value.py
+-rw-r--r--   0        0        0        0 2023-05-01 05:10:55.043163 lixinger-0.1.3/lixinger/api/cn/index/__init__.py
+-rw-r--r--   0        0        0     1721 2023-05-04 10:40:12.140548 lixinger-0.1.3/lixinger/api/cn/index/fundamental.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:08:31.838744 lixinger-0.1.3/lixinger/api/hk/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:09:00.179536 lixinger-0.1.3/lixinger/api/macro/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:08:44.656824 lixinger-0.1.3/lixinger/api/us/__init__.py
+-rw-r--r--   0        0        0     1582 2023-05-04 10:40:12.141591 lixinger-0.1.3/lixinger/config.py
+-rw-r--r--   0        0        0        0 2023-05-03 09:27:58.212202 lixinger-0.1.3/lixinger/py.typed
+-rw-r--r--   0        0        0       75 2023-05-03 10:06:41.922780 lixinger-0.1.3/lixinger/settings.toml
+-rw-r--r--   0        0        0      978 2023-05-04 10:40:12.142362 lixinger-0.1.3/lixinger/utils.py
+-rw-r--r--   0        0        0      986 2023-05-04 14:33:31.621192 lixinger-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-01 04:43:15.660305 lixinger-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:43:19.505533 lixinger-0.1.3/tests/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:43:24.536685 lixinger-0.1.3/tests/api/cn/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:43:30.757795 lixinger-0.1.3/tests/api/cn/company/__init__.py
+-rw-r--r--   0        0        0      127 2023-05-03 10:00:15.081563 lixinger-0.1.3/tests/api/cn/company/test_base.py
+-rw-r--r--   0        0        0        0 2023-05-04 14:30:00.736254 lixinger-0.1.3/tests/api/cn/fund/__init__.py
+-rw-r--r--   0        0        0      229 2023-05-04 14:32:35.703103 lixinger-0.1.3/tests/api/cn/fund/test_total_net_value.py
+-rw-r--r--   0        0        0        0 2023-05-01 05:16:11.323717 lixinger-0.1.3/tests/api/cn/index/__init__.py
+-rw-r--r--   0        0        0      270 2023-05-03 09:27:22.076125 lixinger-0.1.3/tests/api/cn/index/test_fundamental.py
+-rw-r--r--   0        0        0     1431 1970-01-01 00:00:00.000000 lixinger-0.1.3/PKG-INFO
```

### Comparing `lixinger-0.1.2/README.md` & `lixinger-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `lixinger-0.1.2/lixinger/api/cn/company/base.py` & `lixinger-0.1.3/lixinger/api/cn/company/base.py`

 * *Files identical despite different names*

### Comparing `lixinger-0.1.2/lixinger/api/cn/index/fundamental.py` & `lixinger-0.1.3/lixinger/api/cn/index/fundamental.py`

 * *Files identical despite different names*

### Comparing `lixinger-0.1.2/lixinger/config.py` & `lixinger-0.1.3/lixinger/config.py`

 * *Files identical despite different names*

### Comparing `lixinger-0.1.2/lixinger/utils.py` & `lixinger-0.1.3/lixinger/utils.py`

 * *Files identical despite different names*

### Comparing `lixinger-0.1.2/pyproject.toml` & `lixinger-0.1.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -6,31 +6,29 @@
 [tool.pytest.ini_options]
 cache_dir = ".pytest_cache/"
 addopts = "-s -p no:warnings"
 asyncio_mode = "auto"
 
 [project]
 name = "lixinger"
-version = "0.1.2"
+version = "0.1.3"
 description = "Lixinger SDK for Python (Unofficial)"
 authors = [
     { name = "Chaoying", email = "chaoying2022@gmail.com" },
 ]
 dependencies = [
     "pandera>=0.14.5",
     "pydantic>=1.10.7",
     "requests>=2.29.0",
     "dynaconf>=3.1.12",
 ]
 requires-python = ">=3.7"
 readme = "README.md"
 keywords = [
-    "github",
-    "storage",
-    "pandas",
+    "lixinger",
 ]
 classifiers = [
     "Topic :: Software Development :: Build Tools",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
```

### Comparing `lixinger-0.1.2/PKG-INFO` & `lixinger-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: lixinger
-Version: 0.1.2
+Version: 0.1.3
 Summary: Lixinger SDK for Python (Unofficial)
-Keywords: github storage pandas
+Keywords: lixinger
 Author-Email: Chaoying <chaoying2022@gmail.com>
 License: MIT
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

