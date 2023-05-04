# Comparing `tmp/zeroconf-0.61.0.tar.gz` & `tmp/zeroconf-0.62.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeroconf-0.61.0.tar", max compression
+gzip compressed data, was "zeroconf-0.62.0.tar", max compression
```

## Comparing `zeroconf-0.61.0.tar` & `zeroconf-0.62.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0    50674 2023-05-03 20:19:57.628415 zeroconf-0.61.0/CHANGELOG.md
--rw-r--r--   0        0        0    24380 2023-05-03 20:19:56.648405 zeroconf-0.61.0/COPYING
--rw-r--r--   0        0        0     4407 2023-05-03 20:19:56.648405 zeroconf-0.61.0/README.rst
--rw-r--r--   0        0        0     1060 2023-05-03 20:19:56.648405 zeroconf-0.61.0/build_ext.py
--rw-r--r--   0        0        0     6770 2023-05-03 20:19:56.648405 zeroconf-0.61.0/docs/Makefile
--rw-r--r--   0        0        0      234 2023-05-03 20:19:56.648405 zeroconf-0.61.0/docs/api.rst
--rw-r--r--   0        0        0     8145 2023-05-03 20:19:56.648405 zeroconf-0.61.0/docs/conf.py
--rw-r--r--   0        0        0      991 2023-05-03 20:19:56.648405 zeroconf-0.61.0/docs/index.rst
--rw-r--r--   0        0        0     3995 2023-05-03 20:19:57.712416 zeroconf-0.61.0/pyproject.toml
--rw-r--r--   0        0        0     3868 2023-05-03 20:19:57.640416 zeroconf-0.61.0/src/zeroconf/__init__.py
--rw-r--r--   0        0        0      511 2023-05-03 20:19:56.652406 zeroconf-0.61.0/src/zeroconf/_cache.pxd
--rw-r--r--   0        0        0     8493 2023-05-03 20:19:56.652406 zeroconf-0.61.0/src/zeroconf/_cache.py
--rw-r--r--   0        0        0    39043 2023-05-03 20:19:56.652406 zeroconf-0.61.0/src/zeroconf/_core.py
--rw-r--r--   0        0        0     2061 2023-05-03 20:19:56.652406 zeroconf-0.61.0/src/zeroconf/_dns.pxd
--rw-r--r--   0        0        0    18218 2023-05-03 20:19:56.652406 zeroconf-0.61.0/src/zeroconf/_dns.py
--rw-r--r--   0        0        0     2167 2023-05-03 20:19:56.652406 zeroconf-0.61.0/src/zeroconf/_exceptions.py
--rw-r--r--   0        0        0    25863 2023-05-03 20:19:56.652406 zeroconf-0.61.0/src/zeroconf/_handlers.py
--rw-r--r--   0        0        0     2916 2023-05-03 20:19:56.652406 zeroconf-0.61.0/src/zeroconf/_history.py
--rw-r--r--   0        0        0     2980 2023-05-03 20:19:56.652406 zeroconf-0.61.0/src/zeroconf/_logger.py
--rw-r--r--   0        0        0      971 2023-05-03 20:19:56.652406 zeroconf-0.61.0/src/zeroconf/_protocol/__init__.py
--rw-r--r--   0        0        0     2573 2023-05-03 20:19:56.652406 zeroconf-0.61.0/src/zeroconf/_protocol/incoming.pxd
--rw-r--r--   0        0        0    13999 2023-05-03 20:19:56.652406 zeroconf-0.61.0/src/zeroconf/_protocol/incoming.py
--rw-r--r--   0        0        0     1950 2023-05-03 20:19:56.652406 zeroconf-0.61.0/src/zeroconf/_protocol/outgoing.pxd
--rw-r--r--   0        0        0    17758 2023-05-03 20:19:56.652406 zeroconf-0.61.0/src/zeroconf/_protocol/outgoing.py
--rw-r--r--   0        0        0     2355 2023-05-03 20:19:56.652406 zeroconf-0.61.0/src/zeroconf/_services/__init__.py
--rw-r--r--   0        0        0    22113 2023-05-03 20:19:56.652406 zeroconf-0.61.0/src/zeroconf/_services/browser.py
--rw-r--r--   0        0        0    25364 2023-05-03 20:19:56.652406 zeroconf-0.61.0/src/zeroconf/_services/info.py
--rw-r--r--   0        0        0     3964 2023-05-03 20:19:56.652406 zeroconf-0.61.0/src/zeroconf/_services/registry.py
--rw-r--r--   0        0        0     3003 2023-05-03 20:19:56.652406 zeroconf-0.61.0/src/zeroconf/_services/types.py
--rw-r--r--   0        0        0     2909 2023-05-03 20:19:56.652406 zeroconf-0.61.0/src/zeroconf/_updates.py
--rw-r--r--   0        0        0      971 2023-05-03 20:19:56.652406 zeroconf-0.61.0/src/zeroconf/_utils/__init__.py
--rw-r--r--   0        0        0     4144 2023-05-03 20:19:56.652406 zeroconf-0.61.0/src/zeroconf/_utils/asyncio.py
--rw-r--r--   0        0        0     6904 2023-05-03 20:19:56.652406 zeroconf-0.61.0/src/zeroconf/_utils/name.py
--rw-r--r--   0        0        0    15252 2023-05-03 20:19:56.652406 zeroconf-0.61.0/src/zeroconf/_utils/net.py
--rw-r--r--   0        0        0     1308 2023-05-03 20:19:56.652406 zeroconf-0.61.0/src/zeroconf/_utils/time.py
--rw-r--r--   0        0        0    11084 2023-05-03 20:19:56.652406 zeroconf-0.61.0/src/zeroconf/asyncio.py
--rw-r--r--   0        0        0     4469 2023-05-03 20:19:56.652406 zeroconf-0.61.0/src/zeroconf/const.py
--rw-r--r--   0        0        0        0 2023-05-03 20:19:56.652406 zeroconf-0.61.0/src/zeroconf/py.typed
--rw-r--r--   0        0        0     2416 2023-05-03 20:19:56.652406 zeroconf-0.61.0/tests/__init__.py
--rw-r--r--   0        0        0      668 2023-05-03 20:19:56.652406 zeroconf-0.61.0/tests/conftest.py
--rw-r--r--   0        0        0      971 2023-05-03 20:19:56.652406 zeroconf-0.61.0/tests/services/__init__.py
--rw-r--r--   0        0        0    42950 2023-05-03 20:19:56.656406 zeroconf-0.61.0/tests/services/test_browser.py
--rw-r--r--   0        0        0    45244 2023-05-03 20:19:56.656406 zeroconf-0.61.0/tests/services/test_info.py
--rw-r--r--   0        0        0     4923 2023-05-03 20:19:56.656406 zeroconf-0.61.0/tests/services/test_registry.py
--rw-r--r--   0        0        0     6273 2023-05-03 20:19:56.656406 zeroconf-0.61.0/tests/services/test_types.py
--rw-r--r--   0        0        0    41883 2023-05-03 20:19:56.656406 zeroconf-0.61.0/tests/test_asyncio.py
--rw-r--r--   0        0        0     8830 2023-05-03 20:19:56.656406 zeroconf-0.61.0/tests/test_cache.py
--rw-r--r--   0        0        0    29468 2023-05-03 20:19:56.656406 zeroconf-0.61.0/tests/test_core.py
--rw-r--r--   0        0        0    14686 2023-05-03 20:19:56.656406 zeroconf-0.61.0/tests/test_dns.py
--rw-r--r--   0        0        0     5022 2023-05-03 20:19:56.656406 zeroconf-0.61.0/tests/test_exceptions.py
--rw-r--r--   0        0        0    63127 2023-05-03 20:19:56.656406 zeroconf-0.61.0/tests/test_handlers.py
--rw-r--r--   0        0        0     2580 2023-05-03 20:19:56.656406 zeroconf-0.61.0/tests/test_history.py
--rw-r--r--   0        0        0     6640 2023-05-03 20:19:56.656406 zeroconf-0.61.0/tests/test_init.py
--rw-r--r--   0        0        0     3396 2023-05-03 20:19:56.656406 zeroconf-0.61.0/tests/test_logger.py
--rw-r--r--   0        0        0    41672 2023-05-03 20:19:56.656406 zeroconf-0.61.0/tests/test_protocol.py
--rw-r--r--   0        0        0     9477 2023-05-03 20:19:56.656406 zeroconf-0.61.0/tests/test_services.py
--rw-r--r--   0        0        0     2240 2023-05-03 20:19:56.656406 zeroconf-0.61.0/tests/test_updates.py
--rw-r--r--   0        0        0      971 2023-05-03 20:19:56.656406 zeroconf-0.61.0/tests/utils/__init__.py
--rw-r--r--   0        0        0     5101 2023-05-03 20:19:56.656406 zeroconf-0.61.0/tests/utils/test_asyncio.py
--rw-r--r--   0        0        0     2045 2023-05-03 20:19:56.656406 zeroconf-0.61.0/tests/utils/test_name.py
--rw-r--r--   0        0        0     9413 2023-05-03 20:19:56.656406 zeroconf-0.61.0/tests/utils/test_net.py
--rw-r--r--   0        0        0     5527 1970-01-01 00:00:00.000000 zeroconf-0.61.0/setup.py
--rw-r--r--   0        0        0     6297 1970-01-01 00:00:00.000000 zeroconf-0.61.0/PKG-INFO
+-rw-r--r--   0        0        0    50964 2023-05-04 00:48:01.431215 zeroconf-0.62.0/CHANGELOG.md
+-rw-r--r--   0        0        0    24380 2023-05-04 00:48:00.591214 zeroconf-0.62.0/COPYING
+-rw-r--r--   0        0        0     4407 2023-05-04 00:48:00.595214 zeroconf-0.62.0/README.rst
+-rw-r--r--   0        0        0     1060 2023-05-04 00:48:00.595214 zeroconf-0.62.0/build_ext.py
+-rw-r--r--   0        0        0     6770 2023-05-04 00:48:00.595214 zeroconf-0.62.0/docs/Makefile
+-rw-r--r--   0        0        0      234 2023-05-04 00:48:00.595214 zeroconf-0.62.0/docs/api.rst
+-rw-r--r--   0        0        0     8145 2023-05-04 00:48:00.595214 zeroconf-0.62.0/docs/conf.py
+-rw-r--r--   0        0        0      991 2023-05-04 00:48:00.595214 zeroconf-0.62.0/docs/index.rst
+-rw-r--r--   0        0        0     3995 2023-05-04 00:48:01.511215 zeroconf-0.62.0/pyproject.toml
+-rw-r--r--   0        0        0     3868 2023-05-04 00:48:01.443215 zeroconf-0.62.0/src/zeroconf/__init__.py
+-rw-r--r--   0        0        0      511 2023-05-04 00:48:00.595214 zeroconf-0.62.0/src/zeroconf/_cache.pxd
+-rw-r--r--   0        0        0     8493 2023-05-04 00:48:00.595214 zeroconf-0.62.0/src/zeroconf/_cache.py
+-rw-r--r--   0        0        0    39043 2023-05-04 00:48:00.595214 zeroconf-0.62.0/src/zeroconf/_core.py
+-rw-r--r--   0        0        0     2061 2023-05-04 00:48:00.595214 zeroconf-0.62.0/src/zeroconf/_dns.pxd
+-rw-r--r--   0        0        0    18218 2023-05-04 00:48:00.595214 zeroconf-0.62.0/src/zeroconf/_dns.py
+-rw-r--r--   0        0        0     2167 2023-05-04 00:48:00.595214 zeroconf-0.62.0/src/zeroconf/_exceptions.py
+-rw-r--r--   0        0        0    25863 2023-05-04 00:48:00.595214 zeroconf-0.62.0/src/zeroconf/_handlers.py
+-rw-r--r--   0        0        0     2916 2023-05-04 00:48:00.595214 zeroconf-0.62.0/src/zeroconf/_history.py
+-rw-r--r--   0        0        0     2980 2023-05-04 00:48:00.595214 zeroconf-0.62.0/src/zeroconf/_logger.py
+-rw-r--r--   0        0        0      971 2023-05-04 00:48:00.595214 zeroconf-0.62.0/src/zeroconf/_protocol/__init__.py
+-rw-r--r--   0        0        0     2573 2023-05-04 00:48:00.595214 zeroconf-0.62.0/src/zeroconf/_protocol/incoming.pxd
+-rw-r--r--   0        0        0    13999 2023-05-04 00:48:00.595214 zeroconf-0.62.0/src/zeroconf/_protocol/incoming.py
+-rw-r--r--   0        0        0     1950 2023-05-04 00:48:00.595214 zeroconf-0.62.0/src/zeroconf/_protocol/outgoing.pxd
+-rw-r--r--   0        0        0    17758 2023-05-04 00:48:00.595214 zeroconf-0.62.0/src/zeroconf/_protocol/outgoing.py
+-rw-r--r--   0        0        0     2355 2023-05-04 00:48:00.595214 zeroconf-0.62.0/src/zeroconf/_services/__init__.py
+-rw-r--r--   0        0        0    22413 2023-05-04 00:48:00.595214 zeroconf-0.62.0/src/zeroconf/_services/browser.py
+-rw-r--r--   0        0        0    25364 2023-05-04 00:48:00.595214 zeroconf-0.62.0/src/zeroconf/_services/info.py
+-rw-r--r--   0        0        0     3964 2023-05-04 00:48:00.595214 zeroconf-0.62.0/src/zeroconf/_services/registry.py
+-rw-r--r--   0        0        0     3003 2023-05-04 00:48:00.595214 zeroconf-0.62.0/src/zeroconf/_services/types.py
+-rw-r--r--   0        0        0     2909 2023-05-04 00:48:00.595214 zeroconf-0.62.0/src/zeroconf/_updates.py
+-rw-r--r--   0        0        0      971 2023-05-04 00:48:00.595214 zeroconf-0.62.0/src/zeroconf/_utils/__init__.py
+-rw-r--r--   0        0        0     4144 2023-05-04 00:48:00.595214 zeroconf-0.62.0/src/zeroconf/_utils/asyncio.py
+-rw-r--r--   0        0        0     6904 2023-05-04 00:48:00.595214 zeroconf-0.62.0/src/zeroconf/_utils/name.py
+-rw-r--r--   0        0        0    15252 2023-05-04 00:48:00.595214 zeroconf-0.62.0/src/zeroconf/_utils/net.py
+-rw-r--r--   0        0        0     1308 2023-05-04 00:48:00.599214 zeroconf-0.62.0/src/zeroconf/_utils/time.py
+-rw-r--r--   0        0        0    11084 2023-05-04 00:48:00.599214 zeroconf-0.62.0/src/zeroconf/asyncio.py
+-rw-r--r--   0        0        0     4469 2023-05-04 00:48:00.599214 zeroconf-0.62.0/src/zeroconf/const.py
+-rw-r--r--   0        0        0        0 2023-05-04 00:48:00.599214 zeroconf-0.62.0/src/zeroconf/py.typed
+-rw-r--r--   0        0        0     2416 2023-05-04 00:48:00.599214 zeroconf-0.62.0/tests/__init__.py
+-rw-r--r--   0        0        0      668 2023-05-04 00:48:00.599214 zeroconf-0.62.0/tests/conftest.py
+-rw-r--r--   0        0        0      971 2023-05-04 00:48:00.599214 zeroconf-0.62.0/tests/services/__init__.py
+-rw-r--r--   0        0        0    42950 2023-05-04 00:48:00.599214 zeroconf-0.62.0/tests/services/test_browser.py
+-rw-r--r--   0        0        0    45244 2023-05-04 00:48:00.599214 zeroconf-0.62.0/tests/services/test_info.py
+-rw-r--r--   0        0        0     4923 2023-05-04 00:48:00.599214 zeroconf-0.62.0/tests/services/test_registry.py
+-rw-r--r--   0        0        0     6273 2023-05-04 00:48:00.599214 zeroconf-0.62.0/tests/services/test_types.py
+-rw-r--r--   0        0        0    45016 2023-05-04 00:48:00.599214 zeroconf-0.62.0/tests/test_asyncio.py
+-rw-r--r--   0        0        0     8830 2023-05-04 00:48:00.599214 zeroconf-0.62.0/tests/test_cache.py
+-rw-r--r--   0        0        0    29468 2023-05-04 00:48:00.599214 zeroconf-0.62.0/tests/test_core.py
+-rw-r--r--   0        0        0    14686 2023-05-04 00:48:00.599214 zeroconf-0.62.0/tests/test_dns.py
+-rw-r--r--   0        0        0     5022 2023-05-04 00:48:00.599214 zeroconf-0.62.0/tests/test_exceptions.py
+-rw-r--r--   0        0        0    63127 2023-05-04 00:48:00.599214 zeroconf-0.62.0/tests/test_handlers.py
+-rw-r--r--   0        0        0     2580 2023-05-04 00:48:00.599214 zeroconf-0.62.0/tests/test_history.py
+-rw-r--r--   0        0        0     6640 2023-05-04 00:48:00.599214 zeroconf-0.62.0/tests/test_init.py
+-rw-r--r--   0        0        0     3396 2023-05-04 00:48:00.599214 zeroconf-0.62.0/tests/test_logger.py
+-rw-r--r--   0        0        0    41672 2023-05-04 00:48:00.599214 zeroconf-0.62.0/tests/test_protocol.py
+-rw-r--r--   0        0        0     9477 2023-05-04 00:48:00.599214 zeroconf-0.62.0/tests/test_services.py
+-rw-r--r--   0        0        0     2240 2023-05-04 00:48:00.599214 zeroconf-0.62.0/tests/test_updates.py
+-rw-r--r--   0        0        0      971 2023-05-04 00:48:00.599214 zeroconf-0.62.0/tests/utils/__init__.py
+-rw-r--r--   0        0        0     5101 2023-05-04 00:48:00.599214 zeroconf-0.62.0/tests/utils/test_asyncio.py
+-rw-r--r--   0        0        0     2045 2023-05-04 00:48:00.599214 zeroconf-0.62.0/tests/utils/test_name.py
+-rw-r--r--   0        0        0     9413 2023-05-04 00:48:00.599214 zeroconf-0.62.0/tests/utils/test_net.py
+-rw-r--r--   0        0        0     5527 1970-01-01 00:00:00.000000 zeroconf-0.62.0/setup.py
+-rw-r--r--   0        0        0     6297 1970-01-01 00:00:00.000000 zeroconf-0.62.0/PKG-INFO
```

### Comparing `zeroconf-0.61.0/CHANGELOG.md` & `zeroconf-0.62.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.62.0 (2023-05-04)
+### Feature
+* Improve performance of ServiceBrowser outgoing query scheduler ([#1170](https://github.com/python-zeroconf/python-zeroconf/issues/1170)) ([`963d022`](https://github.com/python-zeroconf/python-zeroconf/commit/963d022ef82b615540fa7521d164a98a6c6f5209))
+
 ## v0.61.0 (2023-05-03)
 ### Feature
 * Speed up parsing NSEC records ([#1169](https://github.com/python-zeroconf/python-zeroconf/issues/1169)) ([`06fa94d`](https://github.com/python-zeroconf/python-zeroconf/commit/06fa94d87b4f0451cb475a921ce1d8e9562e0f26))
 
 ## v0.60.0 (2023-05-01)
 ### Feature
 * Speed up processing incoming data ([#1167](https://github.com/python-zeroconf/python-zeroconf/issues/1167)) ([`fbaaf7b`](https://github.com/python-zeroconf/python-zeroconf/commit/fbaaf7bb6ff985bdabb85feb6cba144f12d4f1d6))
```

### Comparing `zeroconf-0.61.0/COPYING` & `zeroconf-0.62.0/COPYING`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/README.rst` & `zeroconf-0.62.0/README.rst`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/build_ext.py` & `zeroconf-0.62.0/build_ext.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/docs/Makefile` & `zeroconf-0.62.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/docs/conf.py` & `zeroconf-0.62.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/docs/index.rst` & `zeroconf-0.62.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/pyproject.toml` & `zeroconf-0.62.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zeroconf"
-version = "0.61.0"
+version = "0.62.0"
 description = "A pure python implementation of multicast DNS service discovery"
 authors = ["Paul Scott-Murphy", "William McBrine", "Jakub Stasiak", "J. Nick Koston"]
 license = "LGPL"
 readme = "README.rst"
 repository = "https://github.com/python-zeroconf/python-zeroconf"
 documentation = "https://python-zeroconf.readthedocs.io"
 classifiers=[
```

### Comparing `zeroconf-0.61.0/src/zeroconf/__init__.py` & `zeroconf-0.62.0/src/zeroconf/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 from ._utils.time import (  # noqa # import needed for backwards compat
     current_time_millis,
     millis_to_seconds,
 )
 
 __author__ = 'Paul Scott-Murphy, William McBrine'
 __maintainer__ = 'Jakub Stasiak <jakub@stasiak.at>'
-__version__ = '0.61.0'
+__version__ = '0.62.0'
 __license__ = 'LGPL'
 
 
 __all__ = [
     "__version__",
     "Zeroconf",
     "ServiceInfo",
```

### Comparing `zeroconf-0.61.0/src/zeroconf/_cache.py` & `zeroconf-0.62.0/src/zeroconf/_cache.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/src/zeroconf/_core.py` & `zeroconf-0.62.0/src/zeroconf/_core.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/src/zeroconf/_dns.pxd` & `zeroconf-0.62.0/src/zeroconf/_dns.pxd`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/src/zeroconf/_dns.py` & `zeroconf-0.62.0/src/zeroconf/_dns.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/src/zeroconf/_exceptions.py` & `zeroconf-0.62.0/src/zeroconf/_exceptions.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/src/zeroconf/_handlers.py` & `zeroconf-0.62.0/src/zeroconf/_handlers.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/src/zeroconf/_history.py` & `zeroconf-0.62.0/src/zeroconf/_history.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/src/zeroconf/_logger.py` & `zeroconf-0.62.0/src/zeroconf/_logger.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/src/zeroconf/_protocol/__init__.py` & `zeroconf-0.62.0/src/zeroconf/_protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/src/zeroconf/_protocol/incoming.pxd` & `zeroconf-0.62.0/src/zeroconf/_protocol/incoming.pxd`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/src/zeroconf/_protocol/incoming.py` & `zeroconf-0.62.0/src/zeroconf/_protocol/incoming.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/src/zeroconf/_protocol/outgoing.pxd` & `zeroconf-0.62.0/src/zeroconf/_protocol/outgoing.pxd`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/src/zeroconf/_protocol/outgoing.py` & `zeroconf-0.62.0/src/zeroconf/_protocol/outgoing.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/src/zeroconf/_services/__init__.py` & `zeroconf-0.62.0/src/zeroconf/_services/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/src/zeroconf/_services/browser.py` & `zeroconf-0.62.0/src/zeroconf/_services/browser.py`

 * *Files 1% similar despite different names*

```diff
@@ -456,21 +456,26 @@
             await self.zc.async_wait_for_start()
         self._async_send_ready_queries_schedule_next()
 
     def _cancel_send_timer(self) -> None:
         """Cancel the next send."""
         if self._next_send_timer:
             self._next_send_timer.cancel()
+            self._next_send_timer = None
 
     def reschedule_type(self, type_: str, now: float, next_time: float) -> None:
         """Reschedule a type to be refreshed in the future."""
         if self.query_scheduler.reschedule_type(type_, next_time):
+            # We need to send the queries before rescheduling the next one
+            # otherwise we may be scheduling a query to go out in the next
+            # iteration of the event loop which should be sent now.
+            if now >= next_time:
+                self._async_send_ready_queries(now)
             self._cancel_send_timer()
             self._async_schedule_next(now)
-        self._async_send_ready_queries(now)
 
     def _async_send_ready_queries(self, now: float) -> None:
         """Send any ready queries."""
         outs = self._generate_ready_queries(self._first_request, now)
         if outs:
             self._first_request = False
             for out in outs:
```

### Comparing `zeroconf-0.61.0/src/zeroconf/_services/info.py` & `zeroconf-0.62.0/src/zeroconf/_services/info.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/src/zeroconf/_services/registry.py` & `zeroconf-0.62.0/src/zeroconf/_services/registry.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/src/zeroconf/_services/types.py` & `zeroconf-0.62.0/src/zeroconf/_services/types.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/src/zeroconf/_updates.py` & `zeroconf-0.62.0/src/zeroconf/_updates.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/src/zeroconf/_utils/__init__.py` & `zeroconf-0.62.0/src/zeroconf/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/src/zeroconf/_utils/asyncio.py` & `zeroconf-0.62.0/src/zeroconf/_utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/src/zeroconf/_utils/name.py` & `zeroconf-0.62.0/src/zeroconf/_utils/name.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/src/zeroconf/_utils/net.py` & `zeroconf-0.62.0/src/zeroconf/_utils/net.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/src/zeroconf/_utils/time.py` & `zeroconf-0.62.0/src/zeroconf/_utils/time.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/src/zeroconf/asyncio.py` & `zeroconf-0.62.0/src/zeroconf/asyncio.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/src/zeroconf/const.py` & `zeroconf-0.62.0/src/zeroconf/const.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/tests/__init__.py` & `zeroconf-0.62.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/tests/conftest.py` & `zeroconf-0.62.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/tests/services/__init__.py` & `zeroconf-0.62.0/tests/services/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/tests/services/test_browser.py` & `zeroconf-0.62.0/tests/services/test_browser.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/tests/services/test_info.py` & `zeroconf-0.62.0/tests/services/test_info.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/tests/services/test_registry.py` & `zeroconf-0.62.0/tests/services/test_registry.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/tests/services/test_types.py` & `zeroconf-0.62.0/tests/services/test_types.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/tests/test_asyncio.py` & `zeroconf-0.62.0/tests/test_asyncio.py`

 * *Files 3% similar despite different names*

```diff
@@ -992,14 +992,17 @@
             sleep_count = 0
             test_iterations = 50
 
             while nbr_answers < test_iterations:
                 # Increase simulated time shift by 1/4 of the TTL in seconds
                 time_offset += expected_ttl / 4
                 now = _new_current_time_millis()
+                # Force the next query to be sent since we are testing
+                # to see if the query contains answers and not the scheduler
+                browser.query_scheduler._next_time[type_] = now + (1000 * expected_ttl)
                 browser.reschedule_type(type_, now, now)
                 sleep_count += 1
                 await asyncio.wait_for(got_query.wait(), 1)
                 got_query.clear()
                 # Prevent the test running indefinitely in an error condition
                 assert sleep_count < test_iterations * 4
             assert not unexpected_ttl.is_set()
@@ -1240,7 +1243,71 @@
     await browser.async_cancel()
     await aiozc.async_close()
 
     assert callbacks == [
         ('add', '_http._tcp.local.', 'ShellyPro4PM-94B97EC07650._http._tcp.local.'),
         ('update', '_http._tcp.local.', 'ShellyPro4PM-94B97EC07650._http._tcp.local.'),
     ]
+
+
+@pytest.mark.asyncio
+async def test_service_browser_does_not_try_to_send_if_not_ready():
+    """Test that the service browser does not try to send if not ready when rescheduling a type."""
+    service_added = asyncio.Event()
+    type_ = "_http._tcp.local."
+    registration_name = "nosend.%s" % type_
+
+    def on_service_state_change(zeroconf, service_type, state_change, name):
+        if name == registration_name:
+            if state_change is ServiceStateChange.Added:
+                service_added.set()
+
+    aiozc = AsyncZeroconf(interfaces=['127.0.0.1'])
+    zeroconf_browser = aiozc.zeroconf
+    await zeroconf_browser.async_wait_for_start()
+
+    expected_ttl = const._DNS_HOST_TTL
+    time_offset = 0.0
+
+    def _new_current_time_millis():
+        """Current system time in milliseconds"""
+        return (time.monotonic() * 1000) + (time_offset * 1000)
+
+    assert len(zeroconf_browser.engine.protocols) == 2
+
+    aio_zeroconf_registrar = AsyncZeroconf(interfaces=['127.0.0.1'])
+    zeroconf_registrar = aio_zeroconf_registrar.zeroconf
+    await aio_zeroconf_registrar.zeroconf.async_wait_for_start()
+    assert len(zeroconf_registrar.engine.protocols) == 2
+    with patch("zeroconf._services.browser.current_time_millis", _new_current_time_millis):
+        service_added = asyncio.Event()
+        browser = AsyncServiceBrowser(zeroconf_browser, type_, [on_service_state_change])
+        desc = {'path': '/~paulsm/'}
+        info = ServiceInfo(
+            type_, registration_name, 80, 0, 0, desc, "ash-2.local.", addresses=[socket.inet_aton("10.0.1.2")]
+        )
+        task = await aio_zeroconf_registrar.async_register_service(info)
+        await task
+
+        try:
+            await asyncio.wait_for(service_added.wait(), 1)
+            time_offset = 1000 * expected_ttl  # set the time to the end of the ttl
+            now = _new_current_time_millis()
+            browser.query_scheduler._next_time[type_] = now + (1000 * expected_ttl)
+            # Make sure the query schedule is to a time in the future
+            # so we will reschedule
+            with patch.object(
+                browser, "_async_send_ready_queries"
+            ) as _async_send_ready_queries, patch.object(
+                browser, "_async_send_ready_queries_schedule_next"
+            ) as _async_send_ready_queries_schedule_next:
+                # Reschedule the type to be sent in 1ms in the future
+                # to make sure the query is not sent
+                browser.reschedule_type(type_, now, now + 1)
+                assert not _async_send_ready_queries.called
+                await asyncio.sleep(0.01)
+                # Make sure it does happen after the sleep
+                assert _async_send_ready_queries_schedule_next.called
+        finally:
+            await aio_zeroconf_registrar.async_close()
+            await browser.async_cancel()
+            await aiozc.async_close()
```

### Comparing `zeroconf-0.61.0/tests/test_cache.py` & `zeroconf-0.62.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/tests/test_core.py` & `zeroconf-0.62.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/tests/test_dns.py` & `zeroconf-0.62.0/tests/test_dns.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/tests/test_exceptions.py` & `zeroconf-0.62.0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/tests/test_handlers.py` & `zeroconf-0.62.0/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/tests/test_history.py` & `zeroconf-0.62.0/tests/test_history.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/tests/test_init.py` & `zeroconf-0.62.0/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/tests/test_logger.py` & `zeroconf-0.62.0/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/tests/test_protocol.py` & `zeroconf-0.62.0/tests/test_protocol.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/tests/test_services.py` & `zeroconf-0.62.0/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/tests/test_updates.py` & `zeroconf-0.62.0/tests/test_updates.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/tests/utils/__init__.py` & `zeroconf-0.62.0/tests/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/tests/utils/test_asyncio.py` & `zeroconf-0.62.0/tests/utils/test_asyncio.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/tests/utils/test_name.py` & `zeroconf-0.62.0/tests/utils/test_name.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/tests/utils/test_net.py` & `zeroconf-0.62.0/tests/utils/test_net.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.61.0/setup.py` & `zeroconf-0.62.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ['ifaddr>=0.1.7']
 
 extras_require = \
 {':python_version < "3.11"': ['async-timeout>=3.0.0']}
 
 setup_kwargs = {
     'name': 'zeroconf',
-    'version': '0.61.0',
+    'version': '0.62.0',
     'description': 'A pure python implementation of multicast DNS service discovery',
     'long_description': 'python-zeroconf\n===============\n\n.. image:: https://github.com/python-zeroconf/python-zeroconf/workflows/CI/badge.svg\n   :target: https://github.com/python-zeroconf/python-zeroconf?query=workflow%3ACI+branch%3Amaster\n\n.. image:: https://img.shields.io/pypi/v/zeroconf.svg\n    :target: https://pypi.python.org/pypi/zeroconf\n\n.. image:: https://codecov.io/gh/python-zeroconf/python-zeroconf/branch/master/graph/badge.svg\n   :target: https://codecov.io/gh/python-zeroconf/python-zeroconf\n\n`Documentation <https://python-zeroconf.readthedocs.io/en/latest/>`_.\n\nThis is fork of pyzeroconf, Multicast DNS Service Discovery for Python,\noriginally by Paul Scott-Murphy (https://github.com/paulsm/pyzeroconf),\nmodified by William McBrine (https://github.com/wmcbrine/pyzeroconf).\n\nThe original William McBrine\'s fork note::\n\n    This fork is used in all of my TiVo-related projects: HME for Python\n    (and therefore HME/VLC), Network Remote, Remote Proxy, and pyTivo.\n    Before this, I was tracking the changes for zeroconf.py in three\n    separate repos. I figured I should have an authoritative source.\n\n    Although I make changes based on my experience with TiVos, I expect that\n    they\'re generally applicable. This version also includes patches found\n    on the now-defunct (?) Launchpad repo of pyzeroconf, and elsewhere\n    around the net -- not always well-documented, sorry.\n\nCompatible with:\n\n* Bonjour\n* Avahi\n\nCompared to some other Zeroconf/Bonjour/Avahi Python packages, python-zeroconf:\n\n* isn\'t tied to Bonjour or Avahi\n* doesn\'t use D-Bus\n* doesn\'t force you to use particular event loop or Twisted (asyncio is used under the hood but not required)\n* is pip-installable\n* has PyPI distribution\n* has an optional cython extension for performance (pure python is supported as well)\n\nPython compatibility\n--------------------\n\n* CPython 3.7+\n* PyPy3.7 7.3+\n\nVersioning\n----------\n\nThis project uses semantic versioning.\n\nStatus\n------\n\nThis project is actively maintained.\n\nTraffic Reduction\n-----------------\n\nBefore version 0.32, most traffic reduction techniques described in https://datatracker.ietf.org/doc/html/rfc6762#section-7\nwhere not implemented which could lead to excessive network traffic.  It is highly recommended that version 0.32 or later\nis used if this is a concern.\n\nIPv6 support\n------------\n\nIPv6 support is relatively new and currently limited, specifically:\n\n* `InterfaceChoice.All` is an alias for `InterfaceChoice.Default` on non-POSIX\n  systems.\n* Dual-stack IPv6 sockets are used, which may not be supported everywhere (some\n  BSD variants do not have them).\n* Listening on localhost (`::1`) does not work. Help with understanding why is\n  appreciated.\n\nHow to get python-zeroconf?\n===========================\n\n* PyPI page https://pypi.org/project/zeroconf/\n* GitHub project https://github.com/python-zeroconf/python-zeroconf\n\nThe easiest way to install python-zeroconf is using pip::\n\n    pip install zeroconf\n\n\n\nHow do I use it?\n================\n\nHere\'s an example of browsing for a service:\n\n.. code-block:: python\n\n    from zeroconf import ServiceBrowser, ServiceListener, Zeroconf\n\n\n    class MyListener(ServiceListener):\n\n        def update_service(self, zc: Zeroconf, type_: str, name: str) -> None:\n            print(f"Service {name} updated")\n\n        def remove_service(self, zc: Zeroconf, type_: str, name: str) -> None:\n            print(f"Service {name} removed")\n\n        def add_service(self, zc: Zeroconf, type_: str, name: str) -> None:\n            info = zc.get_service_info(type_, name)\n            print(f"Service {name} added, service info: {info}")\n\n\n    zeroconf = Zeroconf()\n    listener = MyListener()\n    browser = ServiceBrowser(zeroconf, "_http._tcp.local.", listener)\n    try:\n        input("Press enter to exit...\\n\\n")\n    finally:\n        zeroconf.close()\n\n.. note::\n\n    Discovery and service registration use *all* available network interfaces by default.\n    If you want to customize that you need to specify ``interfaces`` argument when\n    constructing ``Zeroconf`` object (see the code for details).\n\nIf you don\'t know the name of the service you need to browse for, try:\n\n.. code-block:: python\n\n    from zeroconf import ZeroconfServiceTypes\n    print(\'\\n\'.join(ZeroconfServiceTypes.find()))\n\nSee examples directory for more.\n\nChangelog\n=========\n\n`Changelog <CHANGELOG.md>`_\n\nLicense\n=======\n\nLGPL, see COPYING file for details.\n',
     'author': 'Paul Scott-Murphy',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/python-zeroconf/python-zeroconf',
```

### Comparing `zeroconf-0.61.0/PKG-INFO` & `zeroconf-0.62.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeroconf
-Version: 0.61.0
+Version: 0.62.0
 Summary: A pure python implementation of multicast DNS service discovery
 Home-page: https://github.com/python-zeroconf/python-zeroconf
 License: LGPL
 Author: Paul Scott-Murphy
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

