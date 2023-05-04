# Comparing `tmp/Zeraora-0.2.5.tar.gz` & `tmp/Zeraora-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Zeraora-0.2.5.tar", last modified: Mon May  1 16:42:20 2023, max compression
+gzip compressed data, was "dist/Zeraora-0.2.6.tar", last modified: Thu May  4 07:44:53 2023, max compression
```

## Comparing `Zeraora-0.2.5.tar` & `Zeraora-0.2.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:42:20.000000 Zeraora-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-05-01 16:42:20.000000 Zeraora-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-05-01 16:42:09.000000 Zeraora-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:42:20.000000 Zeraora-0.2.5/Zeraora.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-05-01 16:42:19.000000 Zeraora-0.2.5/Zeraora.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-01 16:42:20.000000 Zeraora-0.2.5/Zeraora.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 16:42:19.000000 Zeraora-0.2.5/Zeraora.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-01 16:42:19.000000 Zeraora-0.2.5/Zeraora.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 16:42:20.000000 Zeraora-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-01 16:42:09.000000 Zeraora-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:42:20.000000 Zeraora-0.2.5/zeraora/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-01 16:42:09.000000 Zeraora-0.2.5/zeraora/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-01 16:42:09.000000 Zeraora-0.2.5/zeraora/charsets.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-01 16:42:09.000000 Zeraora-0.2.5/zeraora/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-01 16:42:09.000000 Zeraora-0.2.5/zeraora/divisions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:42:20.000000 Zeraora-0.2.5/zeraora/djangobase/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-01 16:42:09.000000 Zeraora-0.2.5/zeraora/djangobase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-05-01 16:42:09.000000 Zeraora-0.2.5/zeraora/djangobase/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-05-01 16:42:09.000000 Zeraora-0.2.5/zeraora/generators.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-01 16:42:09.000000 Zeraora-0.2.5/zeraora/math.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-01 16:42:09.000000 Zeraora-0.2.5/zeraora/shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-05-01 16:42:09.000000 Zeraora-0.2.5/zeraora/time.py
--rw-r--r--   0 runner    (1001) docker     (123)    13305 2023-05-01 16:42:09.000000 Zeraora-0.2.5/zeraora/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:44:53.000000 Zeraora-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-05-04 07:44:53.000000 Zeraora-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-05-04 07:44:43.000000 Zeraora-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:44:53.000000 Zeraora-0.2.6/Zeraora.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-05-04 07:44:53.000000 Zeraora-0.2.6/Zeraora.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-04 07:44:53.000000 Zeraora-0.2.6/Zeraora.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 07:44:53.000000 Zeraora-0.2.6/Zeraora.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 07:44:53.000000 Zeraora-0.2.6/Zeraora.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 07:44:53.000000 Zeraora-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-04 07:44:43.000000 Zeraora-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:44:53.000000 Zeraora-0.2.6/zeraora/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-04 07:44:43.000000 Zeraora-0.2.6/zeraora/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-04 07:44:43.000000 Zeraora-0.2.6/zeraora/charsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-04 07:44:43.000000 Zeraora-0.2.6/zeraora/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-04 07:44:43.000000 Zeraora-0.2.6/zeraora/divisions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:44:53.000000 Zeraora-0.2.6/zeraora/djangobase/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-04 07:44:43.000000 Zeraora-0.2.6/zeraora/djangobase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-05-04 07:44:43.000000 Zeraora-0.2.6/zeraora/djangobase/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-05-04 07:44:43.000000 Zeraora-0.2.6/zeraora/generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-04 07:44:43.000000 Zeraora-0.2.6/zeraora/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-04 07:44:43.000000 Zeraora-0.2.6/zeraora/shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-05-04 07:44:43.000000 Zeraora-0.2.6/zeraora/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13305 2023-05-04 07:44:43.000000 Zeraora-0.2.6/zeraora/typing.py
```

### Comparing `Zeraora-0.2.5/PKG-INFO` & `Zeraora-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Zeraora
-Version: 0.2.5
+Version: 0.2.6
 Summary: 一个包含原创工具类及快捷函数的工具库。A original utility Python package.
 Home-page: https://github.com/aixcyi/zeraora
 Author: aixcyi
 Author-email: 75880483+aixcyi@users.noreply.github.com
 License: MIT
 Project-URL: Source, https://github.com/aixcyi/zeraora
 Project-URL: Tracker, https://github.com/aixcyi/zeraora/issues
```

### Comparing `Zeraora-0.2.5/README.md` & `Zeraora-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `Zeraora-0.2.5/Zeraora.egg-info/PKG-INFO` & `Zeraora-0.2.6/Zeraora.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Zeraora
-Version: 0.2.5
+Version: 0.2.6
 Summary: 一个包含原创工具类及快捷函数的工具库。A original utility Python package.
 Home-page: https://github.com/aixcyi/zeraora
 Author: aixcyi
 Author-email: 75880483+aixcyi@users.noreply.github.com
 License: MIT
 Project-URL: Source, https://github.com/aixcyi/zeraora
 Project-URL: Tracker, https://github.com/aixcyi/zeraora/issues
```

### Comparing `Zeraora-0.2.5/setup.py` & `Zeraora-0.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.2.5/zeraora/__init__.py` & `Zeraora-0.2.6/zeraora/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,9 +31,9 @@
     ChoicesMeta,
     Choices,
     IntegerChoices,
     TextChoices,
 )
 
 __author__ = 'aixcyi'
-__version__ = (0, 2, 5)
-version = '0.2.5'
+__version__ = (0, 2, 6)
+version = '0.2.6'
```

### Comparing `Zeraora-0.2.5/zeraora/charsets.py` & `Zeraora-0.2.6/zeraora/charsets.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.2.5/zeraora/decorators.py` & `Zeraora-0.2.6/zeraora/decorators.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.2.5/zeraora/divisions.py` & `Zeraora-0.2.6/zeraora/divisions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 中国行政区划相关。
 """
 
-from zeraora import IntegerChoices
+from .typing import IntegerChoices
 
 
 class Province(IntegerChoices):
     """
     中国省级行政区。
     """
     BEIJING = 11, '北京市'
```

### Comparing `Zeraora-0.2.5/zeraora/djangobase/mixins.py` & `Zeraora-0.2.6/zeraora/djangobase/mixins.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.2.5/zeraora/generators.py` & `Zeraora-0.2.6/zeraora/generators.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.2.5/zeraora/time.py` & `Zeraora-0.2.6/zeraora/time.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.2.5/zeraora/typing.py` & `Zeraora-0.2.6/zeraora/typing.py`

 * *Files identical despite different names*

