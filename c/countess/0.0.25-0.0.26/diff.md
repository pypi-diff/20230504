# Comparing `tmp/countess-0.0.25.tar.gz` & `tmp/countess-0.0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "countess-0.0.25.tar", last modified: Thu Apr 27 04:51:42 2023, max compression
+gzip compressed data, was "countess-0.0.26.tar", last modified: Thu May  4 00:11:45 2023, max compression
```

## Comparing `countess-0.0.25.tar` & `countess-0.0.26.tar`

### file list

```diff
@@ -1,48 +1,50 @@
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-27 04:51:42.905179 countess-0.0.25/
--rw-rw-r--   0 nick      (1000) nick      (1000)     1469 2022-12-12 02:15:43.000000 countess-0.0.25/LICENSE.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)       26 2023-04-27 04:47:23.000000 countess-0.0.25/MANIFEST.in
--rw-rw-r--   0 nick      (1000) nick      (1000)     3528 2023-04-27 04:51:42.905179 countess-0.0.25/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)     2877 2023-04-27 04:50:53.000000 countess-0.0.25/README.md
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-27 04:51:42.905179 countess-0.0.25/countess/
--rw-rw-r--   0 nick      (1000) nick      (1000)       43 2023-04-27 04:51:00.000000 countess-0.0.25/countess/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-27 04:51:42.905179 countess-0.0.25/countess/core/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:48:22.000000 countess-0.0.25/countess/core/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)      736 2023-04-21 06:08:37.000000 countess-0.0.25/countess/core/cmd.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     4271 2023-04-21 06:08:37.000000 countess-0.0.25/countess/core/config.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1910 2023-04-21 06:08:37.000000 countess-0.0.25/countess/core/logger.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    15736 2023-04-26 23:25:45.000000 countess-0.0.25/countess/core/parameters.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     5024 2023-04-21 06:08:37.000000 countess-0.0.25/countess/core/pipeline.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    13178 2023-04-26 23:25:45.000000 countess-0.0.25/countess/core/plugins.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-27 04:51:42.905179 countess-0.0.25/countess/gui/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-04-21 06:08:37.000000 countess-0.0.25/countess/gui/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    21779 2023-04-26 02:38:33.000000 countess-0.0.25/countess/gui/config.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     5947 2023-04-26 02:29:55.000000 countess-0.0.25/countess/gui/logger.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    33190 2023-04-26 23:25:45.000000 countess-0.0.25/countess/gui/main.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-27 04:51:42.905179 countess-0.0.25/countess/plugins/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-04-21 06:08:37.000000 countess-0.0.25/countess/plugins/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     5795 2023-04-26 02:38:33.000000 countess-0.0.25/countess/plugins/csv.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1194 2023-04-26 02:29:55.000000 countess-0.0.25/countess/plugins/expression.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2038 2023-04-26 03:33:35.000000 countess-0.0.25/countess/plugins/fastq.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     4145 2023-04-26 02:38:33.000000 countess-0.0.25/countess/plugins/group_by.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1744 2023-04-26 02:29:55.000000 countess-0.0.25/countess/plugins/hdf5.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     3051 2023-04-26 02:38:33.000000 countess-0.0.25/countess/plugins/join.py
--rw-rw-r--   0 nick      (1000) nick      (1000)      347 2023-04-26 02:29:55.000000 countess-0.0.25/countess/plugins/log_score.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     5520 2023-04-26 02:38:33.000000 countess-0.0.25/countess/plugins/pivot.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     6776 2023-04-26 23:25:45.000000 countess-0.0.25/countess/plugins/regex.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2200 2023-04-26 02:38:33.000000 countess-0.0.25/countess/plugins/variant.py
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:39:01.000000 countess-0.0.25/countess/py.typed
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-27 04:51:42.905179 countess-0.0.25/countess/utils/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-09-26 22:30:04.000000 countess-0.0.25/countess/utils/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     9717 2023-04-26 02:29:55.000000 countess-0.0.25/countess/utils/variant.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-27 04:51:42.905179 countess-0.0.25/countess.egg-info/
--rw-rw-r--   0 nick      (1000) nick      (1000)     3528 2023-04-27 04:51:42.000000 countess-0.0.25/countess.egg-info/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)      936 2023-04-27 04:51:42.000000 countess-0.0.25/countess.egg-info/SOURCES.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        1 2023-04-27 04:51:42.000000 countess-0.0.25/countess.egg-info/dependency_links.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)      784 2023-04-27 04:51:42.000000 countess-0.0.25/countess.egg-info/entry_points.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)      237 2023-04-27 04:51:42.000000 countess-0.0.25/countess.egg-info/requires.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        9 2023-04-27 04:51:42.000000 countess-0.0.25/countess.egg-info/top_level.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)     2414 2023-04-27 04:49:11.000000 countess-0.0.25/pyproject.toml
--rw-rw-r--   0 nick      (1000) nick      (1000)     1444 2023-04-27 04:51:42.909180 countess-0.0.25/setup.cfg
--rw-rw-r--   0 nick      (1000) nick      (1000)       39 2023-04-21 06:08:37.000000 countess-0.0.25/setup.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-27 04:51:42.905179 countess-0.0.25/tests/
--rw-rw-r--   0 nick      (1000) nick      (1000)      636 2023-04-21 06:08:37.000000 countess-0.0.25/tests/test_gui.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-04 00:11:45.341878 countess-0.0.26/
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1469 2022-12-12 02:15:43.000000 countess-0.0.26/LICENSE.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)       26 2023-04-27 04:47:23.000000 countess-0.0.26/MANIFEST.in
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3528 2023-05-04 00:11:45.341878 countess-0.0.26/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2877 2023-05-03 23:26:13.000000 countess-0.0.26/README.md
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-04 00:11:45.337878 countess-0.0.26/countess/
+-rw-rw-r--   0 nick      (1000) nick      (1000)       43 2023-05-03 23:26:09.000000 countess-0.0.26/countess/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-04 00:11:45.341878 countess-0.0.26/countess/core/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:48:22.000000 countess-0.0.26/countess/core/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)      736 2023-04-21 06:08:37.000000 countess-0.0.26/countess/core/cmd.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     4271 2023-04-21 06:08:37.000000 countess-0.0.26/countess/core/config.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1910 2023-04-21 06:08:37.000000 countess-0.0.26/countess/core/logger.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    16367 2023-05-03 23:19:50.000000 countess-0.0.26/countess/core/parameters.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     5024 2023-04-21 06:08:37.000000 countess-0.0.26/countess/core/pipeline.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    13178 2023-05-03 23:19:50.000000 countess-0.0.26/countess/core/plugins.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-04 00:11:45.341878 countess-0.0.26/countess/gui/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-04-21 06:08:37.000000 countess-0.0.26/countess/gui/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    21614 2023-05-03 23:23:10.000000 countess-0.0.26/countess/gui/config.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     5947 2023-04-26 02:29:55.000000 countess-0.0.26/countess/gui/logger.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    34627 2023-05-03 23:19:50.000000 countess-0.0.26/countess/gui/main.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-04 00:11:45.341878 countess-0.0.26/countess/plugins/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-04-21 06:08:37.000000 countess-0.0.26/countess/plugins/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     5795 2023-05-03 23:19:50.000000 countess-0.0.26/countess/plugins/csv.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3711 2023-05-03 23:19:50.000000 countess-0.0.26/countess/plugins/data_table.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1194 2023-04-26 02:29:55.000000 countess-0.0.26/countess/plugins/expression.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2017 2023-05-03 23:01:14.000000 countess-0.0.26/countess/plugins/fastq.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     4145 2023-05-03 23:19:50.000000 countess-0.0.26/countess/plugins/group_by.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1744 2023-04-26 02:29:55.000000 countess-0.0.26/countess/plugins/hdf5.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3051 2023-05-03 23:19:50.000000 countess-0.0.26/countess/plugins/join.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)      347 2023-04-26 02:29:55.000000 countess-0.0.26/countess/plugins/log_score.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2359 2023-05-03 23:15:48.000000 countess-0.0.26/countess/plugins/mutagenize.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     5520 2023-05-03 23:19:50.000000 countess-0.0.26/countess/plugins/pivot.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     6776 2023-05-03 23:19:50.000000 countess-0.0.26/countess/plugins/regex.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2200 2023-05-03 23:19:50.000000 countess-0.0.26/countess/plugins/variant.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:39:01.000000 countess-0.0.26/countess/py.typed
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-04 00:11:45.341878 countess-0.0.26/countess/utils/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-09-26 22:30:04.000000 countess-0.0.26/countess/utils/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     9717 2023-04-26 02:29:55.000000 countess-0.0.26/countess/utils/variant.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-04 00:11:45.337878 countess-0.0.26/countess.egg-info/
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3528 2023-05-04 00:11:45.000000 countess-0.0.26/countess.egg-info/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)      998 2023-05-04 00:11:45.000000 countess-0.0.26/countess.egg-info/SOURCES.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)        1 2023-05-04 00:11:45.000000 countess-0.0.26/countess.egg-info/dependency_links.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)      899 2023-05-04 00:11:45.000000 countess-0.0.26/countess.egg-info/entry_points.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)      239 2023-05-04 00:11:45.000000 countess-0.0.26/countess.egg-info/requires.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)        9 2023-05-04 00:11:45.000000 countess-0.0.26/countess.egg-info/top_level.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2595 2023-05-03 23:13:20.000000 countess-0.0.26/pyproject.toml
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1444 2023-05-04 00:11:45.341878 countess-0.0.26/setup.cfg
+-rw-rw-r--   0 nick      (1000) nick      (1000)       39 2023-04-21 06:08:37.000000 countess-0.0.26/setup.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-04 00:11:45.341878 countess-0.0.26/tests/
+-rw-rw-r--   0 nick      (1000) nick      (1000)      636 2023-04-21 06:08:37.000000 countess-0.0.26/tests/test_gui.py
```

### Comparing `countess-0.0.25/LICENSE.txt` & `countess-0.0.26/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `countess-0.0.25/PKG-INFO` & `countess-0.0.26/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: countess
-Version: 0.0.25
+Version: 0.0.26
 Summary: CountESS
 Author: CountESS Developers
 Author-email: Nick Moore <nick@zoic.org>, Alan Rubin <alan@rubin.id.au>
 Maintainer: Nick Moore
 Maintainer-email: Nick Moore <nick@zoic.org>
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -14,15 +14,15 @@
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: hdf
 License-File: LICENSE.txt
 
-# CountESS 0.0.25
+# CountESS 0.0.26
 
 This is CountESS, a modular, Python 3 reimplementation of Enrich2.
 
 ## License
 
 BSD 3-clause.  See [LICENSE.txt](LICENSE.txt)
```

### Comparing `countess-0.0.25/README.md` & `countess-0.0.26/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# CountESS 0.0.25
+# CountESS 0.0.26
 
 This is CountESS, a modular, Python 3 reimplementation of Enrich2.
 
 ## License
 
 BSD 3-clause.  See [LICENSE.txt](LICENSE.txt)
```

### Comparing `countess-0.0.25/countess/core/cmd.py` & `countess-0.0.26/countess/core/cmd.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.25/countess/core/config.py` & `countess-0.0.26/countess/core/config.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.25/countess/core/logger.py` & `countess-0.0.26/countess/core/logger.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.25/countess/core/parameters.py` & `countess-0.0.26/countess/core/parameters.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import hashlib
 import os.path
 import re
-from typing import Any, Iterable, Mapping, Optional
+from typing import Any, Iterable, Mapping, Optional, Type
 
 PARAM_DIGEST_HASH = "sha256"
 
 
 class BaseParam:
     """Represents the parameters which can be set on a plugin."""
 
@@ -81,19 +81,36 @@
         return bool(value)
 
 
 class IntegerParam(SimpleParam):
     var_type = int
     _value: int = 0
 
+    def clean_value(self, value):
+        if isinstance(value, str):
+            return super().clean_value("".join(re.split(r"\D+", value)))
+        else:
+            return super().clean_value(value)
+
 
 class FloatParam(SimpleParam):
     var_type = float
     _value: float = 0.0
 
+    def clean_value(self, value):
+        if isinstance(value, str):
+            try:
+                a, b = value.split(".", 1)
+                s = re.split(r"\D+", a) + ["."] + re.split(r"\D+", b)
+            except ValueError:
+                s = re.split(r"\D+", value)
+            return super().clean_value("".join(s))
+        else:
+            return super().clean_value(value)
+
 
 class StringParam(SimpleParam):
     var_type = str
     _value: str = ""
 
 
 class TextParam(StringParam):
@@ -234,19 +251,19 @@
             self._value = None
 
     def copy(self):
         return self.__class__(self.label, self.value, self.choices)
 
 
 class DataTypeChoiceParam(ChoiceParam):
-    DATA_TYPES: Mapping[str, Optional[tuple[type, Any]]] = {
-        "string": (str, None),
-        "number": (float, None),
-        "integer": (int, 0),
-        "boolean": (bool, None),
+    DATA_TYPES: Mapping[str, tuple[type, Any, Type[SimpleParam]]] = {
+        "string": (str, None, StringParam),
+        "number": (float, None, FloatParam),
+        "integer": (int, 0, IntegerParam),
+        "boolean": (bool, None, BooleanParam),
     }
 
     def __init__(
         self, label: str, value: Optional[str] = None, choices: Optional[Iterable[str]] = None
     ):
         if not choices:
             choices = list(self.DATA_TYPES.keys())
@@ -262,31 +279,26 @@
         if self.value is None:
             return None
         if value is None:
             return self.DATA_TYPES[self.value][1]
         else:
             return self.DATA_TYPES[self.value][0](value)
 
+    def get_parameter(self, label: str, value=None) -> BaseParam:
+        return self.DATA_TYPES[self.value][2](label, value)
+
 
 class DataTypeOrNoneChoiceParam(DataTypeChoiceParam):
     NONE_VALUE = "— NONE —"
 
-    DATA_TYPES = {
-        "string": (str, None),
-        "number": (float, None),
-        "integer": (int, 0),
-        "boolean": (bool, None),
-        NONE_VALUE: None,
-    }
-
     def __init__(
         self, label: str, value: Optional[str] = None, choices: Optional[Iterable[str]] = None
     ):
         if not choices:
-            choices = list(self.DATA_TYPES.keys())
+            choices = list(self.DATA_TYPES.keys()) + [self.NONE_VALUE]
         if value is None:
             value = self.NONE_VALUE
         super().__init__(label, value, choices)
 
     def get_selected_type(self):
         if self.value == self.NONE_VALUE:
             return None
@@ -537,15 +549,15 @@
     def get_parameters(self, key, base_dir="."):
         for k, p in self.params.items():
             yield from p.get_parameters(f"{key}.{k}", base_dir)
 
     def get_hash_value(self):
         digest = hashlib.new(PARAM_DIGEST_HASH)
         for k, p in self.params.items():
-            digest.update((k + "\0" + p.get_hash_value()).encode("utf-8"))
+            digest.update((str(k) + "\0" + p.get_hash_value()).encode("utf-8"))
         return digest.hexdigest()
 
     def set_column_choices(self, choices):
         for p in self.params.values():
             p.set_column_choices(choices)
```

### Comparing `countess-0.0.25/countess/core/pipeline.py` & `countess-0.0.26/countess/core/pipeline.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.25/countess/core/plugins.py` & `countess-0.0.26/countess/core/plugins.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.25/countess/gui/config.py` & `countess-0.0.26/countess/gui/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,14 @@
     ArrayParam,
     BaseParam,
     BooleanParam,
     ChoiceParam,
     FileArrayParam,
     FileParam,
     FileSaveParam,
-    FloatParam,
-    IntegerParam,
     MultiParam,
     SimpleParam,
     TabularMultiParam,
     TextParam,
 )
 from ..core.plugins import BasePlugin
 
@@ -52,14 +50,15 @@
         level=0,
     ):
         self.parameter = parameter
         self.callback = callback
         self.button = None
         self.level = level
         self.subwrapper_buttons: list[tk.Button] = []
+        self.column_labels: list[tk.Label] = []
 
         self.subwrappers: Mapping[BaseParam, ParameterWrapper] = {}
 
         self.var: Optional[tk.Variable] = None
         self.entry: Optional[tk.Widget] = None
         self.label: Optional[tk.Widget] = None
         self.row_labels: list[tk.Widget] = []
@@ -91,21 +90,15 @@
             self.entry = tk.Text(tk_parent, height=10)
             self.entry.insert("1.0", parameter.value)
             if parameter.read_only:
                 self.entry["state"] = "disabled"
             else:
                 self.entry.bind("<<Modified>>", self.widget_modified_callback)
         elif isinstance(parameter, SimpleParam):
-            if isinstance(parameter, FloatParam):
-                self.var = tk.DoubleVar(tk_parent, value=parameter.value)
-            elif isinstance(parameter, IntegerParam):
-                self.var = tk.IntVar(tk_parent, value=parameter.value)
-            else:
-                self.var = tk.StringVar(tk_parent, value=parameter.value)
-
+            self.var = tk.StringVar(tk_parent, value=parameter.value)
             self.entry = ttk.Entry(tk_parent, textvariable=self.var)
             if parameter.read_only:
                 self.entry.state(["readonly"])
 
         elif (
             isinstance(parameter, ArrayParam)
             and self.level == 0
@@ -136,20 +129,14 @@
                     width=2,
                     command=self.add_row_callback,
                 )
                 self.button.grid(row=0, column=1, padx=10)
 
             drc = self.delete_row_callback if not parameter.read_only else None
             if isinstance(parameter.param, MultiParam):
-                for n, pp in enumerate(parameter.param.values()):
-                    tk.Label(self.entry, text=pp.label).grid(
-                        row=0, column=n + 1, sticky=tk.EW, padx=10
-                    )
-                    self.entry.columnconfigure(n + 1, weight=1)
-
                 self.update_subwrappers_tabular(parameter.params, drc)
             else:
                 self.entry.columnconfigure(0, weight=0)
                 self.entry.columnconfigure(1, weight=0)
                 self.entry.columnconfigure(2, weight=1)
 
                 # XXX hack because the empty labelframe collapses
@@ -263,18 +250,24 @@
             self.subwrappers[p].set_row(n)
 
         self.cull_subwrappers(params)
 
     def update_subwrappers_tabular(self, params, delete_row_callback):
         while self.subwrapper_buttons:
             self.subwrapper_buttons.pop().destroy()
-
-        for rl in self.row_labels:
-            rl.destroy()
-        self.row_labels = []
+        while self.row_labels:
+            self.row_labels.pop().destroy()
+        while self.column_labels:
+            self.column_labels.pop().destroy()
+
+        for n, pp in enumerate(self.parameter.param.values()):
+            column_label = tk.Label(self.entry, text=pp.label)
+            self.column_labels.append(column_label)
+            column_label.grid(row=0, column=n + 1, sticky=tk.EW, padx=10)
+            self.entry.columnconfigure(n + 1, weight=1)
 
         for n, p in enumerate(params):
             row_label = tk.Label(self.entry, text=p.label)
             row_label.grid(row=n + 1, column=0, padx=10)
             self.row_labels.append(row_label)
 
             subparams = p.params.values()
```

### Comparing `countess-0.0.25/countess/gui/logger.py` & `countess-0.0.26/countess/gui/logger.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.25/countess/gui/main.py` & `countess-0.0.26/countess/gui/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,16 +97,16 @@
         self.after(100, self.__on_timeout)
 
     def __place(self, event=None):
         x, y, w, h = _geometry(self)
         x = x + (event.x if event else (w // 2))
         y = y + (event.y if event else (h // 2))
         return {
-            "relx": _limit( x / self.master.winfo_width(), 0.05, 0.95),
-            "rely": _limit( y / self.master.winfo_height(), 0.05, 0.95),
+            "relx": _limit(x / self.master.winfo_width(), 0.05, 0.95),
+            "rely": _limit(y / self.master.winfo_height(), 0.05, 0.95),
             "anchor": "c",
         }
 
     def __on_timeout(self):
         if self.__state == self.__state.DRAG_WAIT:
             self.__state = self.__state.DRAGGING
             self["cursor"] = TkCursors.ARROWS.value
@@ -405,15 +405,15 @@
         for connecting_line, _, _ in self.lines_lookup.values():
             self.canvas.itemconfig(connecting_line.line, fill="black")
 
     def new_node_position(self, x, y):
         flipped = self.canvas.winfo_height() > self.canvas.winfo_width()
         xp = _limit(x / self.canvas.winfo_width(), 0.05, 0.95)
         yp = _limit(y / self.canvas.winfo_height(), 0.05, 0.95)
-        return (yp, xp) if flipped else (xp,yp)
+        return (yp, xp) if flipped else (xp, yp)
 
     def on_canvas_button1(self, event):
         pass
 
     def on_canvas_button3(self, event):
         """Click to create a new node, if it is created on top of a line
         that line is broken and the node is included."""
@@ -421,15 +421,15 @@
         items = self.canvas.find_overlapping(event.x - 10, event.y - 10, event.x + 10, event.y + 10)
 
         # XXX creating a new node every time you click on the background
         # is proving quite annoying.  Lets see how it is to go without it.
         # (you can still create a new node by button-3-dragging from an
         # existing node, and if you really want a disconnected graph you can
         # delete the link to the new node!)
-        #if not items:
+        # if not items:
         #    return
 
         position = self.new_node_position(event.x, event.y)
         new_node = self.add_new_node(position)
 
         for item in items:
             _, child_node, parent_node = self.lines_lookup[item]
@@ -503,15 +503,15 @@
         return new_node
 
     def on_ghost_release(self, start_node, event):
         xl, yl, _wl, _hl = _geometry(event.widget)
         flipped = self.canvas.winfo_height() > self.canvas.winfo_width()
         other_node = self.find_node_at_position(event.x + xl, event.y + yl)
         if other_node is None:
-            position = self.new_node_position(event.x+xl,event.y+yl)
+            position = self.new_node_position(event.x + xl, event.y + yl)
             other_node = self.add_new_node(position)
         elif other_node == start_node:
             return
         elif start_node in other_node.parent_nodes:
             other_node.del_parent(start_node)
             return
         elif other_node in start_node.parent_nodes:
@@ -562,17 +562,20 @@
             label.destroy()
 
 
 class ConfiguratorWrapper:
     """Wraps up the PluginConfigurator or PluginChooserFrame, plus a
     DataFramePreview, to make up the larger part of the main window"""
 
+    config_canvas = None
     config_subframe = None
+    config_subframe_id = None
     preview_subframe = None
     config_change_task = None
+    notes_widget = None
 
     def __init__(self, frame, node, change_callback):
         self.frame = frame
         self.node = node
         self.change_callback = change_callback
 
         self.name_var = tk.StringVar(self.frame, value=node.name)
@@ -581,61 +584,95 @@
         )
         self.name_var.trace("w", self.name_changed_callback)
 
         self.label = tk.Label(self.frame, justify=tk.LEFT, wraplength=500)
         self.label.grid(sticky=tk.EW, row=1, padx=10, pady=5)
         self.label.bind("<Configure>", self.on_label_configure)
 
-        self.notes_widget = tk.Text(self.frame, height=5)
-        self.notes_widget.insert("1.0", node.notes or "")
-        self.notes_widget.bind("<<Modified>>", self.notes_modified_callback)
-
         self.logger_subframe = LoggerFrame(self.frame)
         self.logger = self.logger_subframe.get_logger(node.name)
 
         self.show_config_subframe()
         if self.node.plugin:
             if self.node.is_dirty:
                 self.config_change_callback()
             else:
                 self.show_preview_subframe()
 
     def show_config_subframe(self):
-        if self.config_subframe:
-            self.config_subframe.destroy()
+        if self.config_canvas:
+            self.config_canvas.destroy()
+        self.config_canvas = tk.Canvas(self.frame)
+        self.config_scrollbar = ttk.Scrollbar(
+            self.frame, orient=tk.VERTICAL, command=self.config_canvas.yview
+        )
+        self.config_canvas.configure(yscrollcommand=self.config_scrollbar.set, bd=0)
+        self.config_canvas.grid(row=3, sticky=tk.NSEW)
+        self.config_scrollbar.grid(row=3, column=1, sticky=tk.NS)
+
         self.node.prepare(self.logger)
+
         if self.node.plugin:
+            if self.node.notes:
+                self.show_notes_widget(self.node.notes)
+            else:
+                self.notes_widget = tk.Button(
+                    self.frame, text="add notes", command=self.on_add_notes
+                )
+                self.notes_widget.grid(row=2, columnspan=2, padx=10, pady=5)
+
             self.label["text"] = "%s %s — %s" % (
                 self.node.plugin.name,
                 self.node.plugin.version,
                 self.node.plugin.description,
             )
             if self.node.plugin.link:
                 tk.Button(
                     self.frame, text=UNICODE_INFO, fg="blue", command=self.on_info_button_press
                 ).grid(row=1, column=1, sticky=tk.SE, padx=10)
-            self.notes_widget.grid(row=2, columnspan=2, sticky=tk.EW, padx=10, pady=5)
             self.node.prepare(self.logger)
             self.node.plugin.update()
             self.configurator = PluginConfigurator(
-                self.frame, self.node.plugin, self.config_change_callback
+                self.config_canvas, self.node.plugin, self.config_change_callback
             )
             self.config_subframe = self.configurator.frame
         else:
             self.config_subframe = PluginChooserFrame(
                 self.frame, "Choose Plugin", self.choose_plugin
             )
-        self.config_subframe.grid(row=3, columnspan=2, sticky=tk.NSEW)
+        self.config_subframe_id = self.config_canvas.create_window(
+            (0, 0), window=self.config_subframe, anchor=tk.NW
+        )
+        self.config_subframe.bind(
+            "<Configure>",
+            lambda e: self.config_canvas.configure(scrollregion=self.config_canvas.bbox("all")),
+        )
+        self.config_canvas.bind("<Configure>", self.on_config_canvas_configure)
+
+    def on_config_canvas_configure(self, *_):
+        self.config_canvas.itemconfigure(
+            self.config_subframe_id, width=self.config_canvas.winfo_width()
+        )
 
     def on_label_configure(self, *_):
         self.label["wraplength"] = self.label.winfo_width() - 20
 
     def on_info_button_press(self, *_):
         webbrowser.open_new_tab(self.node.plugin.link)
 
+    def on_add_notes(self, *_):
+        self.notes_widget.destroy()
+        self.show_notes_widget()
+
+    def show_notes_widget(self, notes=""):
+        self.notes_widget = tk.Text(self.frame, height=5)
+        self.notes_widget.insert("1.0", notes)
+        self.notes_widget.bind("<<Modified>>", self.notes_modified_callback)
+        self.notes_widget.grid(row=2, columnspan=2, sticky=tk.EW, padx=10, pady=5)
+
     def show_preview_subframe(self):
         if self.preview_subframe:
             self.preview_subframe.destroy()
         if isinstance(self.node.result, pd.DataFrame):
             self.preview_subframe = DataFramePreview(self.frame, self.node.result).frame
         elif isinstance(self.node.result, str):
             self.preview_subframe = tk.Frame(self.frame)
@@ -663,15 +700,15 @@
 
     def name_changed_callback(self, *_):
         name = self.name_var.get()
         self.node.name = name
         self.change_callback(self.node)
 
     def notes_modified_callback(self, *_):
-        self.node.notes = self.notes_widget.get("1.0", tk.END)
+        self.node.notes = self.notes_widget.get("1.0", tk.END).strip()
         self.notes_widget.edit_modified(False)
 
     def config_change_callback(self, *_):
         self.node.mark_dirty()
         if self.config_change_task:
             self.frame.after_cancel(self.config_change_task)
         self.config_change_task = self.frame.after(500, self.config_change_task_callback)
```

### Comparing `countess-0.0.25/countess/plugins/csv.py` & `countess-0.0.26/countess/plugins/csv.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.25/countess/plugins/expression.py` & `countess-0.0.26/countess/plugins/expression.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.25/countess/plugins/fastq.py` & `countess-0.0.26/countess/plugins/fastq.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,13 +39,14 @@
 
     def combine_dfs(self, dfs):
         """first concatenate the count dataframes, then (optionally) group them by sequence"""
 
         combined_df = pd.concat(dfs)
 
         if len(combined_df) and self.parameters["group"].value:
-            combined_df = combined_df.groupby(by=["sequence", "filename"]).agg(
-                {"sequence": "first", "filename": "first", "header": "count"}
+            combined_df = (
+                combined_df.groupby(by=["sequence"])
+                .agg({"sequence": "first", "header": "count"})
+                .rename({"header": "count"}, axis=1)
             )
-            combined_df.rename({"header": "count"}, axis=1)
 
         return combined_df
```

### Comparing `countess-0.0.25/countess/plugins/group_by.py` & `countess-0.0.26/countess/plugins/group_by.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.25/countess/plugins/hdf5.py` & `countess-0.0.26/countess/plugins/hdf5.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.25/countess/plugins/join.py` & `countess-0.0.26/countess/plugins/join.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.25/countess/plugins/pivot.py` & `countess-0.0.26/countess/plugins/pivot.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.25/countess/plugins/regex.py` & `countess-0.0.26/countess/plugins/regex.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.25/countess/plugins/variant.py` & `countess-0.0.26/countess/plugins/variant.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.25/countess/utils/variant.py` & `countess-0.0.26/countess/utils/variant.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.25/countess.egg-info/PKG-INFO` & `countess-0.0.26/countess.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: countess
-Version: 0.0.25
+Version: 0.0.26
 Summary: CountESS
 Author: CountESS Developers
 Author-email: Nick Moore <nick@zoic.org>, Alan Rubin <alan@rubin.id.au>
 Maintainer: Nick Moore
 Maintainer-email: Nick Moore <nick@zoic.org>
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -14,15 +14,15 @@
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: hdf
 License-File: LICENSE.txt
 
-# CountESS 0.0.25
+# CountESS 0.0.26
 
 This is CountESS, a modular, Python 3 reimplementation of Enrich2.
 
 ## License
 
 BSD 3-clause.  See [LICENSE.txt](LICENSE.txt)
```

### Comparing `countess-0.0.25/countess.egg-info/SOURCES.txt` & `countess-0.0.26/countess.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -21,19 +21,21 @@
 countess/core/plugins.py
 countess/gui/__init__.py
 countess/gui/config.py
 countess/gui/logger.py
 countess/gui/main.py
 countess/plugins/__init__.py
 countess/plugins/csv.py
+countess/plugins/data_table.py
 countess/plugins/expression.py
 countess/plugins/fastq.py
 countess/plugins/group_by.py
 countess/plugins/hdf5.py
 countess/plugins/join.py
 countess/plugins/log_score.py
+countess/plugins/mutagenize.py
 countess/plugins/pivot.py
 countess/plugins/regex.py
 countess/plugins/variant.py
 countess/utils/__init__.py
 countess/utils/variant.py
 tests/test_gui.py
```

### Comparing `countess-0.0.25/countess.egg-info/entry_points.txt` & `countess-0.0.26/countess.egg-info/entry_points.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 [console_scripts]
 countess_cmd = countess.core.cmd:main
 
 [countess_plugins]
+data_table = countess.plugins.data_table:DataTablePlugin
 expression = countess.plugins.expression:ExpressionPlugin
 group_by = countess.plugins.group_by:GroupByPlugin
 group_by_expr = countess.plugins.group_by:GroupByExprPlugin
 join = countess.plugins.join:JoinPlugin
 load_csv = countess.plugins.csv:LoadCsvPlugin
 load_fastq = countess.plugins.fastq:LoadFastqPlugin
 load_hdf = countess.plugins.hdf5:LoadHdfPlugin
 log_score = countess.plugins.log_score:LogScorePlugin
+mutagenize = countess.plugins.mutagenize:MutagenizePlugin
 pivot = countess.plugins.pivot:PivotPlugin
 regex_reader = countess.plugins.regex:RegexReaderPlugin
 regex_tool = countess.plugins.regex:RegexToolPlugin
 save_csv = countess.plugins.csv:SaveCsvPlugin
 variants = countess.plugins.variant:VariantPlugin
 
 [gui_scripts]
```

### Comparing `countess-0.0.25/pyproject.toml` & `countess-0.0.26/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 dev = [
     'black<24',
     'build==0.10.0',
     'mypy~=1.0.1',
     'pylint~=2.16',
     'types-ttkthemes~=3.2',
     'twine==4.0.2',
-    'pandas-stubs~=1.4',
+    'pandas-stubs~=2.0.0',
     'pytest~=7.2',
 ]
 
 hdf = [
      'tables~=3.8.0',
 ]
 
@@ -54,14 +54,16 @@
 expression = "countess.plugins.expression:ExpressionPlugin"
 pivot = "countess.plugins.pivot:PivotPlugin"
 join = "countess.plugins.join:JoinPlugin"
 save_csv = "countess.plugins.csv:SaveCsvPlugin"
 regex_tool = "countess.plugins.regex:RegexToolPlugin"
 regex_reader = "countess.plugins.regex:RegexReaderPlugin"
 variants = "countess.plugins.variant:VariantPlugin"
+mutagenize = "countess.plugins.mutagenize:MutagenizePlugin"
+data_table = "countess.plugins.data_table:DataTablePlugin"
 
 [project.entry-points.gui_scripts]
 countess_gui = "countess.gui.main:main"
 
 [project.entry-points.console_scripts]
 countess_cmd = "countess.core.cmd:main"
 
@@ -80,11 +82,13 @@
     "invalid-name",
     "no-else-return",
     "too-many-ancestors",
     "too-many-arguments",
     "too-many-branches",
     "too-many-instance-attributes",
     "too-many-locals",
+    "too-many-public-methods",
+    "unidiomatic-typecheck",
 ]
 
 [tool.black]
 line-length = 100
```

### Comparing `countess-0.0.25/setup.cfg` & `countess-0.0.26/setup.cfg`

 * *Files identical despite different names*

### Comparing `countess-0.0.25/tests/test_gui.py` & `countess-0.0.26/tests/test_gui.py`

 * *Files identical despite different names*

