# Comparing `tmp/pydicts-0.4.0.tar.gz` & `tmp/pydicts-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydicts-0.4.0.tar", max compression
+gzip compressed data, was "pydicts-0.5.0.tar", max compression
```

## Comparing `pydicts-0.4.0.tar` & `pydicts-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
--rw-r--r--   0        0        0    35149 2023-04-10 16:27:20.112887 pydicts-0.4.0/LICENSE
--rw-r--r--   0        0        0     3384 2023-04-19 18:05:13.360372 pydicts-0.4.0/README.md
--rw-r--r--   0        0        0      144 2023-04-19 18:03:52.588369 pydicts-0.4.0/pydicts/__init__.py
--rw-r--r--   0        0        0     2814 2023-04-11 05:44:25.702913 pydicts-0.4.0/pydicts/classes.py
--rw-r--r--   0        0        0      424 2023-04-19 18:07:00.714375 pydicts-0.4.0/pydicts/locale/en/LC_MESSAGES/pydicts.mo
--rw-r--r--   0        0        0      738 2022-04-25 13:52:57.304754 pydicts-0.4.0/pydicts/locale/en.po
--rw-r--r--   0        0        0      513 2023-04-19 18:07:00.711375 pydicts-0.4.0/pydicts/locale/es/LC_MESSAGES/pydicts.mo
--rw-r--r--   0        0        0     2755 2023-04-19 17:40:24.132024 pydicts-0.4.0/pydicts/locale/es.po
--rw-r--r--   0        0        0      633 2023-04-19 17:40:13.925023 pydicts-0.4.0/pydicts/locale/pydicts.pot
--rw-r--r--   0        0        0     5550 2023-04-19 17:47:51.996037 pydicts-0.4.0/pydicts/lod.py
--rw-r--r--   0        0        0     1052 2023-04-12 05:25:02.458349 pydicts-0.4.0/pydicts/lod_xyv.py
--rw-r--r--   0        0        0     8792 2023-04-15 22:54:44.487769 pydicts-0.4.0/pydicts/lod_ymv.py
--rw-r--r--   0        0        0        0 2023-04-10 16:27:20.112887 pydicts-0.4.0/pydicts/tests/__init__.py
--rw-r--r--   0        0        0     1064 2023-04-19 17:53:54.673048 pydicts-0.4.0/pydicts/tests/test_lod.py
--rw-r--r--   0        0        0      409 2023-04-12 05:32:28.379363 pydicts-0.4.0/pydicts/tests/test_lod_ymv.py
--rw-r--r--   0        0        0      797 2023-04-19 18:07:56.169377 pydicts-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3901 1970-01-01 00:00:00.000000 pydicts-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-10 16:27:20.112887 pydicts-0.5.0/LICENSE
+-rw-r--r--   0        0        0     3401 2023-05-04 17:12:16.245845 pydicts-0.5.0/README.md
+-rw-r--r--   0        0        0      143 2023-05-04 17:11:12.157843 pydicts-0.5.0/pydicts/__init__.py
+-rw-r--r--   0        0        0     2814 2023-04-11 05:44:25.702913 pydicts-0.5.0/pydicts/classes.py
+-rw-r--r--   0        0        0      424 2023-05-04 17:12:34.664846 pydicts-0.5.0/pydicts/locale/en/LC_MESSAGES/pydicts.mo
+-rw-r--r--   0        0        0      738 2022-04-25 13:52:57.304754 pydicts-0.5.0/pydicts/locale/en.po
+-rw-r--r--   0        0        0      513 2023-05-04 17:12:34.662845 pydicts-0.5.0/pydicts/locale/es/LC_MESSAGES/pydicts.mo
+-rw-r--r--   0        0        0     2755 2023-04-19 17:40:24.132024 pydicts-0.5.0/pydicts/locale/es.po
+-rw-r--r--   0        0        0      633 2023-04-19 17:40:13.925023 pydicts-0.5.0/pydicts/locale/pydicts.pot
+-rw-r--r--   0        0        0     5811 2023-05-03 15:58:54.826246 pydicts-0.5.0/pydicts/lod.py
+-rw-r--r--   0        0        0     1052 2023-04-12 05:25:02.458349 pydicts-0.5.0/pydicts/lod_xyv.py
+-rw-r--r--   0        0        0     8792 2023-04-15 22:54:44.487769 pydicts-0.5.0/pydicts/lod_ymv.py
+-rw-r--r--   0        0        0     3716 2023-05-04 17:10:10.584841 pydicts-0.5.0/pydicts/pylatex.py
+-rw-r--r--   0        0        0        0 2023-04-10 16:27:20.112887 pydicts-0.5.0/pydicts/tests/__init__.py
+-rw-r--r--   0        0        0     1064 2023-04-19 17:53:54.673048 pydicts-0.5.0/pydicts/tests/test_lod.py
+-rw-r--r--   0        0        0      409 2023-04-12 05:32:28.379363 pydicts-0.5.0/pydicts/tests/test_lod_ymv.py
+-rw-r--r--   0        0        0     1038 2023-05-04 17:14:37.488849 pydicts-0.5.0/pydicts/tests/test_pylatex.py
+-rw-r--r--   0        0        0      816 2023-05-04 17:10:46.554842 pydicts-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3918 1970-01-01 00:00:00.000000 pydicts-0.5.0/PKG-INFO
```

### Comparing `pydicts-0.4.0/LICENSE` & `pydicts-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydicts-0.4.0/README.md` & `pydicts-0.5.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -82,17 +82,15 @@
 ### lod_rename_key
 
 ### lod_remove_key
 
 Removes a key in all dictionaries in the list of dictionaries
 
 ```python
-from pydicts.lod import lod_print, lod_remove_key
-lod=[{"a":1, "b":4},{"a":2, "b":None}]
->>> from pydicts.lod import *
+>>> from pydicts.lod import lod_print, lod_remove_key
 >>> lod=[{"a":1, "b":4},{"a":2, "b":None}]
 >>> lod_print(lod)
 +-----+-----+
 |   a |   b |
 |-----+-----|
 |   1 |   4 |
 |   2 |     |
@@ -143,14 +141,17 @@
 ### lod_ymv_filling
 
 ## Testing
 poetry run pytest
 
 ## CHANGELOG
 
+### 0.5.0 (2023-05-04)
+- Added support to latex tables from list of dictionaries
+
 ### 0.4.0 (2023-04-19)
 - Added poetry support
 - Added poethepoet support
 - Added lod_remove_key
 
 ### 0.3.0 (2023-04-16)
 - Added lod_ymv_transposition_with_porcentages
```

### Comparing `pydicts-0.4.0/pydicts/classes.py` & `pydicts-0.5.0/pydicts/classes.py`

 * *Files identical despite different names*

### Comparing `pydicts-0.4.0/pydicts/locale/en.po` & `pydicts-0.5.0/pydicts/locale/en.po`

 * *Files identical despite different names*

### Comparing `pydicts-0.4.0/pydicts/locale/es/LC_MESSAGES/pydicts.mo` & `pydicts-0.5.0/pydicts/locale/es/LC_MESSAGES/pydicts.mo`

 * *Files identical despite different names*

### Comparing `pydicts-0.4.0/pydicts/locale/es.po` & `pydicts-0.5.0/pydicts/locale/es.po`

 * *Files identical despite different names*

### Comparing `pydicts-0.4.0/pydicts/locale/pydicts.pot` & `pydicts-0.5.0/pydicts/locale/pydicts.pot`

 * *Files identical despite different names*

### Comparing `pydicts-0.4.0/pydicts/lod.py` & `pydicts-0.5.0/pydicts/lod.py`

 * *Files 4% similar despite different names*

```diff
@@ -213,7 +213,17 @@
 def lod_remove_key(lod, key):
     """
         Removes a key from all dictionaries in a list of dictionaries
     """
     for d in lod:
         del d[key]
     return lod
+    
+def lod_keys(lod_):
+    """
+        Return the keys of the list of dicts
+        Return None if length of lod is 0. 
+        Retuurn the keys of the first dictionary as a list
+    """
+    if len(lod_)>0:
+        return list(lod_[0].keys())
+    return None
```

### Comparing `pydicts-0.4.0/pydicts/lod_xyv.py` & `pydicts-0.5.0/pydicts/lod_xyv.py`

 * *Files identical despite different names*

### Comparing `pydicts-0.4.0/pydicts/lod_ymv.py` & `pydicts-0.5.0/pydicts/lod_ymv.py`

 * *Files identical despite different names*

### Comparing `pydicts-0.4.0/pydicts/tests/test_lod.py` & `pydicts-0.5.0/pydicts/tests/test_lod.py`

 * *Files identical despite different names*

### Comparing `pydicts-0.4.0/pyproject.toml` & `pydicts-0.5.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydicts"
-version = "0.4.0"
+version = "0.5.0"
 description = "Module to use dictionaries in various situations"
 authors = ["turulomio <turulomio@yahoo.es>"]
 license = "GPL-3.0"
 readme = "README.md"
 exclude = [
     "pydicts/devscripts.py"
 ]
@@ -12,14 +12,15 @@
 [tool.poetry.dependencies]
 python = "^3.10"
 tabulate = "^0.9.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.0"
 poethepoet = "^0.19.0"
+pylatex = "^1.4.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poe.tasks]
 release = { script = "pydicts.devscripts:release" }
```

### Comparing `pydicts-0.4.0/PKG-INFO` & `pydicts-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydicts
-Version: 0.4.0
+Version: 0.5.0
 Summary: Module to use dictionaries in various situations
 License: GPL-3.0
 Author: turulomio
 Author-email: turulomio@yahoo.es
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
@@ -97,17 +97,15 @@
 ### lod_rename_key
 
 ### lod_remove_key
 
 Removes a key in all dictionaries in the list of dictionaries
 
 ```python
-from pydicts.lod import lod_print, lod_remove_key
-lod=[{"a":1, "b":4},{"a":2, "b":None}]
->>> from pydicts.lod import *
+>>> from pydicts.lod import lod_print, lod_remove_key
 >>> lod=[{"a":1, "b":4},{"a":2, "b":None}]
 >>> lod_print(lod)
 +-----+-----+
 |   a |   b |
 |-----+-----|
 |   1 |   4 |
 |   2 |     |
@@ -158,14 +156,17 @@
 ### lod_ymv_filling
 
 ## Testing
 poetry run pytest
 
 ## CHANGELOG
 
+### 0.5.0 (2023-05-04)
+- Added support to latex tables from list of dictionaries
+
 ### 0.4.0 (2023-04-19)
 - Added poetry support
 - Added poethepoet support
 - Added lod_remove_key
 
 ### 0.3.0 (2023-04-16)
 - Added lod_ymv_transposition_with_porcentages
```

