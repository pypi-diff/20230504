# Comparing `tmp/DataProperty-0.8.1.tar.gz` & `tmp/DataProperty-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/DataProperty-0.8.1.tar", last modified: Wed Jul 27 13:26:17 2016, max compression
+gzip compressed data, was "dist/DataProperty-0.9.0.tar", last modified: Sat Sep 10 14:03:07 2016, max compression
```

## Comparing `DataProperty-0.8.1.tar` & `DataProperty-0.9.0.tar`

### file list

```diff
@@ -1,55 +1,54 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2016-07-27 13:26:17.000000 DataProperty-0.8.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2016-07-27 13:26:17.000000 DataProperty-0.8.1/DataProperty.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10540 2016-07-27 13:26:16.000000 DataProperty-0.8.1/DataProperty.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1210 2016-07-27 13:26:16.000000 DataProperty-0.8.1/DataProperty.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2016-07-27 13:26:16.000000 DataProperty-0.8.1/DataProperty.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       25 2016-07-27 13:26:16.000000 DataProperty-0.8.1/DataProperty.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2016-07-27 13:26:16.000000 DataProperty-0.8.1/DataProperty.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2016-07-27 13:26:17.000000 DataProperty-0.8.1/dataproperty/
-drwxr-xr-x   0 root         (0) root         (0)        0 2016-07-27 13:26:17.000000 DataProperty-0.8.1/dataproperty/converter/
--rwxrwxrwx   0 root         (0) root         (0)      391 2016-07-09 04:33:51.000000 DataProperty-0.8.1/dataproperty/converter/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     4367 2016-07-09 05:06:14.000000 DataProperty-0.8.1/dataproperty/converter/_core.py
--rwxrwxrwx   0 root         (0) root         (0)     1308 2016-07-09 03:56:55.000000 DataProperty-0.8.1/dataproperty/converter/_creator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2016-07-27 13:26:17.000000 DataProperty-0.8.1/dataproperty/type/
--rwxrwxrwx   0 root         (0) root         (0)      896 2016-07-09 12:32:18.000000 DataProperty-0.8.1/dataproperty/type/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     4883 2016-07-09 12:23:15.000000 DataProperty-0.8.1/dataproperty/type/_checker.py
--rwxrwxrwx   0 root         (0) root         (0)     1867 2016-07-09 12:22:43.000000 DataProperty-0.8.1/dataproperty/type/_checker_creator.py
--rwxrwxrwx   0 root         (0) root         (0)      634 2016-07-02 09:10:58.000000 DataProperty-0.8.1/dataproperty/type/_typecode.py
--rwxrwxrwx   0 root         (0) root         (0)     1065 2016-07-23 08:17:19.000000 DataProperty-0.8.1/dataproperty/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      656 2016-05-06 13:38:10.000000 DataProperty-0.8.1/dataproperty/_align.py
--rwxrwxrwx   0 root         (0) root         (0)      797 2016-07-09 12:31:49.000000 DataProperty-0.8.1/dataproperty/_align_getter.py
--rwxrwxrwx   0 root         (0) root         (0)     1687 2016-05-06 13:38:24.000000 DataProperty-0.8.1/dataproperty/_container.py
--rwxrwxrwx   0 root         (0) root         (0)    12825 2016-07-17 01:39:03.000000 DataProperty-0.8.1/dataproperty/_data_property.py
--rwxrwxrwx   0 root         (0) root         (0)      172 2016-06-04 05:30:16.000000 DataProperty-0.8.1/dataproperty/_error.py
--rwxrwxrwx   0 root         (0) root         (0)     3032 2016-07-09 12:28:51.000000 DataProperty-0.8.1/dataproperty/_factory.py
--rwxrwxrwx   0 root         (0) root         (0)     5009 2016-07-23 09:30:49.000000 DataProperty-0.8.1/dataproperty/_function.py
--rwxrwxrwx   0 root         (0) root         (0)      495 2016-07-09 13:16:38.000000 DataProperty-0.8.1/dataproperty/_interface.py
--rwxrwxrwx   0 root         (0) root         (0)     2691 2016-07-27 13:09:16.000000 DataProperty-0.8.1/dataproperty/_property_extractor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2016-07-27 13:26:17.000000 DataProperty-0.8.1/misc/
--rwxrwxrwx   0 root         (0) root         (0)     3930 2016-03-24 04:48:10.000000 DataProperty-0.8.1/misc/README.md
--rwxrwxrwx   0 root         (0) root         (0)      667 2016-03-20 12:35:01.000000 DataProperty-0.8.1/misc/README_HEADER.rst
--rwxrwxrwx   0 root         (0) root         (0)     1092 2016-02-26 06:26:06.000000 DataProperty-0.8.1/misc/readme_converter.py
--rwxrwxrwx   0 root         (0) root         (0)       47 2016-02-26 04:13:48.000000 DataProperty-0.8.1/misc/summary.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2016-07-27 13:26:17.000000 DataProperty-0.8.1/requirements/
--rwxrwxrwx   0 root         (0) root         (0)       17 2016-02-14 06:04:47.000000 DataProperty-0.8.1/requirements/docs_requirements.txt
--rwxrwxrwx   0 root         (0) root         (0)       25 2016-06-04 06:03:03.000000 DataProperty-0.8.1/requirements/requirements.txt
--rwxrwxrwx   0 root         (0) root         (0)       22 2016-07-03 00:53:22.000000 DataProperty-0.8.1/requirements/test_requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2016-07-27 13:26:17.000000 DataProperty-0.8.1/test/
--rwxrwxrwx   0 root         (0) root         (0)     1558 2016-05-15 12:24:42.000000 DataProperty-0.8.1/test/test_align_getter.py
--rwxrwxrwx   0 root         (0) root         (0)     8709 2016-07-03 08:36:32.000000 DataProperty-0.8.1/test/test_column_property.py
--rwxrwxrwx   0 root         (0) root         (0)     2875 2016-07-03 06:58:08.000000 DataProperty-0.8.1/test/test_container.py
--rwxrwxrwx   0 root         (0) root         (0)     5489 2016-07-09 04:04:01.000000 DataProperty-0.8.1/test/test_converter.py
--rwxrwxrwx   0 root         (0) root         (0)      839 2016-07-09 04:34:38.000000 DataProperty-0.8.1/test/test_converter_creator.py
--rwxrwxrwx   0 root         (0) root         (0)    11014 2016-07-23 09:57:33.000000 DataProperty-0.8.1/test/test_function.py
--rwxrwxrwx   0 root         (0) root         (0)    12901 2016-07-09 16:33:01.000000 DataProperty-0.8.1/test/test_property.py
--rwxrwxrwx   0 root         (0) root         (0)    10202 2016-07-17 02:33:51.000000 DataProperty-0.8.1/test/test_property_extractor.py
--rwxrwxrwx   0 root         (0) root         (0)     7525 2016-07-09 12:28:03.000000 DataProperty-0.8.1/test/test_type_checker.py
--rwxrwxrwx   0 root         (0) root         (0)     1015 2016-07-09 12:29:15.000000 DataProperty-0.8.1/test/test_type_checker_creator.py
--rwxrwxrwx   0 root         (0) root         (0)      491 2016-06-04 12:57:03.000000 DataProperty-0.8.1/test/test_typecode.py
--rwxrwxrwx   0 root         (0) root         (0)     1105 2016-02-19 14:57:59.000000 DataProperty-0.8.1/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      203 2016-02-26 12:26:02.000000 DataProperty-0.8.1/MANIFEST.in
--rwxrwxrwx   0 root         (0) root         (0)     7613 2016-07-25 13:52:01.000000 DataProperty-0.8.1/README.rst
--rwxrwxrwx   0 root         (0) root         (0)     2071 2016-07-27 13:14:27.000000 DataProperty-0.8.1/setup.py
--rwxrwxrwx   0 root         (0) root         (0)      109 2016-07-09 11:47:50.000000 DataProperty-0.8.1/tox.ini
--rw-r--r--   0 root         (0) root         (0)    10540 2016-07-27 13:26:17.000000 DataProperty-0.8.1/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      107 2016-07-27 13:26:17.000000 DataProperty-0.8.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2016-09-10 14:03:07.000000 DataProperty-0.9.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2016-09-10 14:03:07.000000 DataProperty-0.9.0/DataProperty.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10540 2016-09-10 14:03:06.000000 DataProperty-0.9.0/DataProperty.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1195 2016-09-10 14:03:06.000000 DataProperty-0.9.0/DataProperty.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2016-09-10 14:03:06.000000 DataProperty-0.9.0/DataProperty.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2016-09-10 14:03:06.000000 DataProperty-0.9.0/DataProperty.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2016-09-10 14:03:06.000000 DataProperty-0.9.0/DataProperty.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2016-09-10 14:03:07.000000 DataProperty-0.9.0/dataproperty/
+drwxr-xr-x   0 root         (0) root         (0)        0 2016-09-10 14:03:07.000000 DataProperty-0.9.0/dataproperty/converter/
+-rwxrwxrwx   0 root         (0) root         (0)      391 2016-07-09 04:33:51.000000 DataProperty-0.9.0/dataproperty/converter/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4388 2016-09-10 13:05:44.000000 DataProperty-0.9.0/dataproperty/converter/_core.py
+-rwxrwxrwx   0 root         (0) root         (0)     1307 2016-09-10 13:05:50.000000 DataProperty-0.9.0/dataproperty/converter/_creator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2016-09-10 14:03:07.000000 DataProperty-0.9.0/dataproperty/type/
+-rwxrwxrwx   0 root         (0) root         (0)      896 2016-07-09 12:32:18.000000 DataProperty-0.9.0/dataproperty/type/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5379 2016-09-10 13:45:18.000000 DataProperty-0.9.0/dataproperty/type/_checker.py
+-rwxrwxrwx   0 root         (0) root         (0)     1866 2016-09-10 13:06:00.000000 DataProperty-0.9.0/dataproperty/type/_checker_creator.py
+-rwxrwxrwx   0 root         (0) root         (0)      765 2016-09-10 13:13:51.000000 DataProperty-0.9.0/dataproperty/type/_typecode.py
+-rwxrwxrwx   0 root         (0) root         (0)     1065 2016-07-23 08:17:19.000000 DataProperty-0.9.0/dataproperty/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      656 2016-05-06 13:38:10.000000 DataProperty-0.9.0/dataproperty/_align.py
+-rwxrwxrwx   0 root         (0) root         (0)      797 2016-07-09 12:31:49.000000 DataProperty-0.9.0/dataproperty/_align_getter.py
+-rwxrwxrwx   0 root         (0) root         (0)     1687 2016-05-06 13:38:24.000000 DataProperty-0.9.0/dataproperty/_container.py
+-rwxrwxrwx   0 root         (0) root         (0)    12825 2016-07-17 01:39:03.000000 DataProperty-0.9.0/dataproperty/_data_property.py
+-rwxrwxrwx   0 root         (0) root         (0)      172 2016-06-04 05:30:16.000000 DataProperty-0.9.0/dataproperty/_error.py
+-rwxrwxrwx   0 root         (0) root         (0)     3030 2016-09-10 13:06:17.000000 DataProperty-0.9.0/dataproperty/_factory.py
+-rwxrwxrwx   0 root         (0) root         (0)     5009 2016-07-23 09:30:49.000000 DataProperty-0.9.0/dataproperty/_function.py
+-rwxrwxrwx   0 root         (0) root         (0)      492 2016-09-10 13:06:27.000000 DataProperty-0.9.0/dataproperty/_interface.py
+-rwxrwxrwx   0 root         (0) root         (0)     2691 2016-07-27 13:09:16.000000 DataProperty-0.9.0/dataproperty/_property_extractor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2016-09-10 14:03:07.000000 DataProperty-0.9.0/misc/
+-rwxrwxrwx   0 root         (0) root         (0)      667 2016-03-20 12:35:01.000000 DataProperty-0.9.0/misc/README_HEADER.rst
+-rwxrwxrwx   0 root         (0) root         (0)     1092 2016-02-26 06:26:06.000000 DataProperty-0.9.0/misc/readme_converter.py
+-rwxrwxrwx   0 root         (0) root         (0)       47 2016-02-26 04:13:48.000000 DataProperty-0.9.0/misc/summary.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2016-09-10 14:03:07.000000 DataProperty-0.9.0/requirements/
+-rwxrwxrwx   0 root         (0) root         (0)       36 2016-09-10 13:03:18.000000 DataProperty-0.9.0/requirements/docs_requirements.txt
+-rwxrwxrwx   0 root         (0) root         (0)       25 2016-06-04 06:03:03.000000 DataProperty-0.9.0/requirements/requirements.txt
+-rwxrwxrwx   0 root         (0) root         (0)       22 2016-07-03 00:53:22.000000 DataProperty-0.9.0/requirements/test_requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2016-09-10 14:03:07.000000 DataProperty-0.9.0/test/
+-rwxrwxrwx   0 root         (0) root         (0)     1558 2016-05-15 12:24:42.000000 DataProperty-0.9.0/test/test_align_getter.py
+-rwxrwxrwx   0 root         (0) root         (0)     8709 2016-07-03 08:36:32.000000 DataProperty-0.9.0/test/test_column_property.py
+-rwxrwxrwx   0 root         (0) root         (0)     2875 2016-07-03 06:58:08.000000 DataProperty-0.9.0/test/test_container.py
+-rwxrwxrwx   0 root         (0) root         (0)     5489 2016-07-09 04:04:01.000000 DataProperty-0.9.0/test/test_converter.py
+-rwxrwxrwx   0 root         (0) root         (0)      839 2016-07-09 04:34:38.000000 DataProperty-0.9.0/test/test_converter_creator.py
+-rwxrwxrwx   0 root         (0) root         (0)    11014 2016-07-23 09:57:33.000000 DataProperty-0.9.0/test/test_function.py
+-rwxrwxrwx   0 root         (0) root         (0)    12901 2016-07-09 16:33:01.000000 DataProperty-0.9.0/test/test_property.py
+-rwxrwxrwx   0 root         (0) root         (0)    10202 2016-07-17 02:33:51.000000 DataProperty-0.9.0/test/test_property_extractor.py
+-rwxrwxrwx   0 root         (0) root         (0)    10717 2016-09-10 13:51:31.000000 DataProperty-0.9.0/test/test_type_checker.py
+-rwxrwxrwx   0 root         (0) root         (0)     1015 2016-07-09 12:29:15.000000 DataProperty-0.9.0/test/test_type_checker_creator.py
+-rwxrwxrwx   0 root         (0) root         (0)      685 2016-09-10 13:14:40.000000 DataProperty-0.9.0/test/test_typecode.py
+-rwxrwxrwx   0 root         (0) root         (0)     1105 2016-02-19 14:57:59.000000 DataProperty-0.9.0/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      203 2016-02-26 12:26:02.000000 DataProperty-0.9.0/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)     7613 2016-07-25 13:52:01.000000 DataProperty-0.9.0/README.rst
+-rwxrwxrwx   0 root         (0) root         (0)      107 2016-09-10 14:03:07.000000 DataProperty-0.9.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2071 2016-09-10 13:39:24.000000 DataProperty-0.9.0/setup.py
+-rwxrwxrwx   0 root         (0) root         (0)      109 2016-07-09 11:47:50.000000 DataProperty-0.9.0/tox.ini
+-rw-r--r--   0 root         (0) root         (0)    10540 2016-09-10 14:03:07.000000 DataProperty-0.9.0/PKG-INFO
```

### Comparing `DataProperty-0.8.1/DataProperty.egg-info/PKG-INFO` & `DataProperty-0.9.0/DataProperty.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: DataProperty
-Version: 0.8.1
+Version: 0.9.0
 Summary: Python library for extract property from data.
 
 Home-page: https://github.com/thombashi/DataProperty
 Author: Tsuyoshi Hombashi
 Author-email: gogogo.vm@gmail.com
 License: MIT License
 Description: **DataProperty**
```

### Comparing `DataProperty-0.8.1/DataProperty.egg-info/SOURCES.txt` & `DataProperty-0.9.0/DataProperty.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 dataproperty/converter/__init__.py
 dataproperty/converter/_core.py
 dataproperty/converter/_creator.py
 dataproperty/type/__init__.py
 dataproperty/type/_checker.py
 dataproperty/type/_checker_creator.py
 dataproperty/type/_typecode.py
-misc/README.md
 misc/README_HEADER.rst
 misc/readme_converter.py
 misc/summary.txt
 requirements/docs_requirements.txt
 requirements/requirements.txt
 requirements/test_requirements.txt
 test/test_align_getter.py
```

### Comparing `DataProperty-0.8.1/dataproperty/converter/_core.py` & `DataProperty-0.9.0/dataproperty/converter/_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 # encoding: utf-8
 
 """
 .. codeauthor:: Tsuyoshi Hombashi <gogogo.vm@gmail.com>
 """
 
 from __future__ import absolute_import
+from __future__ import division
 import abc
 import re
 
 from .._error import TypeConversionError
 
 
 class ValueConverterInterface(object):
 
     @abc.abstractmethod
-    def convert(self):   # pragma: no cover
+    def convert(self):  # pragma: no cover
         pass
 
 
 class ValueConverter(ValueConverterInterface):
 
     @abc.abstractmethod
-    def convert(self):   # pragma: no cover
+    def convert(self):  # pragma: no cover
         pass
 
     def __init__(self, value):
         self._value = value
 
     def __repr__(self):
         return str(self.convert())
@@ -76,15 +77,15 @@
         except ValueError:
             raise TypeConversionError("failed to convert: " + str(self._value))
 
 
 class DateTimeConverter(ValueConverter):
 
     __DAYS_TO_SECONDS_COEF = 60 ** 2 * 24
-    __MICROSECONDS_TO_SECONDS_COEF = 1000.0 ** 2
+    __MICROSECONDS_TO_SECONDS_COEF = 1000 ** 2
     __COMMON_DST_TIMEZONE_TABLE = {
         -36000: "America/Adak",  # -1000
         -32400: "US/Alaska",  # -0900
         -28800: "US/Pacific",  # -0800
         -25200: "US/Mountain",  # -0700
         -21600: "US/Central",  # -0600
         -18000: "US/Eastern",  # -0500
@@ -135,15 +136,15 @@
 
         return int(
             (
                 dt.days *
                 self.__DAYS_TO_SECONDS_COEF +
                 float(dt.seconds)
             ) +
-            float(dt.microseconds / self.__MICROSECONDS_TO_SECONDS_COEF)
+            dt.microseconds / self.__MICROSECONDS_TO_SECONDS_COEF
         )
 
     def __get_dst_timezone_name(self, offset):
         return self.__COMMON_DST_TIMEZONE_TABLE[offset]
 
     def __validate_datetime_string(self):
         """
```

### Comparing `DataProperty-0.8.1/dataproperty/converter/_creator.py` & `DataProperty-0.9.0/dataproperty/converter/_creator.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from ._core import DateTimeConverter
 
 
 @six.add_metaclass(abc.ABCMeta)
 class ValueConverterCreatorInterface(object):
 
     @abc.abstractmethod
-    def create(self, value):   # pragma: no cover
+    def create(self, value):  # pragma: no cover
         pass
 
 
 class NopConverterCreator(ValueConverterCreatorInterface):
 
     def create(self, value):
         return NopConverter(value)
```

### Comparing `DataProperty-0.8.1/dataproperty/type/__init__.py` & `DataProperty-0.9.0/dataproperty/type/__init__.py`

 * *Files identical despite different names*

### Comparing `DataProperty-0.8.1/dataproperty/type/_checker.py` & `DataProperty-0.9.0/dataproperty/type/_checker.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,26 +21,30 @@
 from ._typecode import Typecode
 
 
 @six.add_metaclass(abc.ABCMeta)
 class TypeCheckerInterface(object):
 
     @abc.abstractproperty
-    def typecode(self):   # pragma: no cover
+    def typecode(self):  # pragma: no cover
         pass
 
     @abc.abstractmethod
-    def is_type(self):   # pragma: no cover
+    def is_type(self):  # pragma: no cover
+        pass
+
+    @abc.abstractmethod
+    def validate(self):  # pragma: no cover
         pass
 
 
 class TypeChecker(TypeCheckerInterface):
 
     @abc.abstractproperty
-    def _converter_creator(self):   # pragma: no cover
+    def _converter_creator(self):  # pragma: no cover
         pass
 
     def __init__(self, value, is_convert=True):
         self._value = value
         self._converted_value = None
         self._is_convert = is_convert
 
@@ -60,14 +64,29 @@
             return False
 
         if not self._is_valid_after_convert():
             return False
 
         return True
 
+    def validate(self, exception_type=TypeError, message=None):
+        """
+        :raises ValueError:
+            If the value is not matched the type to be expected.
+        """
+
+        if self.is_type():
+            return
+
+        if message is None:
+            message = "invalid value type: expected={:s}".format(
+                Typecode.get_typename(self.typecode))
+
+        raise exception_type(message)
+
     @abc.abstractmethod
     def _is_instance(self):
         pass
 
     def _is_exclude_instance(self):
         return False
```

### Comparing `DataProperty-0.8.1/dataproperty/type/_checker_creator.py` & `DataProperty-0.9.0/dataproperty/type/_checker_creator.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from ._checker import NanChecker
 
 
 @six.add_metaclass(abc.ABCMeta)
 class TypeCheckerCreatorInterface(object):
 
     @abc.abstractmethod
-    def create(self, value, is_convert):   # pragma: no cover
+    def create(self, value, is_convert):  # pragma: no cover
         pass
 
 
 class NoneTypeCheckerCreator(TypeCheckerCreatorInterface):
 
     def create(self, value, is_convert):
         return NoneTypeChecker(value, is_convert)
```

### Comparing `DataProperty-0.8.1/dataproperty/type/_typecode.py` & `DataProperty-0.9.0/dataproperty/type/_typecode.py`

 * *Files 26% similar despite different names*

```diff
@@ -26,8 +26,12 @@
         INFINITY: "INFINITY",
         NAN: "NAN",
         BOOL: "BOOL",
     }
 
     @classmethod
     def get_typename(cls, typecode):
-        return cls.__TYPENAME_TABLE.get(typecode)
+        type_name = cls.__TYPENAME_TABLE.get(typecode)
+        if type_name is None:
+            raise ValueError("unknown typecode: {}".format(typecode))
+
+        return type_name
```

### Comparing `DataProperty-0.8.1/dataproperty/__init__.py` & `DataProperty-0.9.0/dataproperty/__init__.py`

 * *Files identical despite different names*

### Comparing `DataProperty-0.8.1/dataproperty/_align.py` & `DataProperty-0.9.0/dataproperty/_align.py`

 * *Files identical despite different names*

### Comparing `DataProperty-0.8.1/dataproperty/_align_getter.py` & `DataProperty-0.9.0/dataproperty/_align_getter.py`

 * *Files identical despite different names*

### Comparing `DataProperty-0.8.1/dataproperty/_container.py` & `DataProperty-0.9.0/dataproperty/_container.py`

 * *Files identical despite different names*

### Comparing `DataProperty-0.8.1/dataproperty/_data_property.py` & `DataProperty-0.9.0/dataproperty/_data_property.py`

 * *Files identical despite different names*

### Comparing `DataProperty-0.8.1/dataproperty/_factory.py` & `DataProperty-0.9.0/dataproperty/_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,19 +28,19 @@
 @six.add_metaclass(abc.ABCMeta)
 class TypeConverterFactoryInterface(object):
     """
     Abstract factory class of type converter.
     """
 
     @abc.abstractproperty
-    def type_checker_factory(self):   # pragma: no cover
+    def type_checker_factory(self):  # pragma: no cover
         pass
 
     @abc.abstractproperty
-    def value_converter_factory(self):   # pragma: no cover
+    def value_converter_factory(self):  # pragma: no cover
         pass
 
 
 class NoneTypeFactory(TypeConverterFactoryInterface):
 
     @property
     def type_checker_factory(self):
```

### Comparing `DataProperty-0.8.1/dataproperty/_function.py` & `DataProperty-0.9.0/dataproperty/_function.py`

 * *Files identical despite different names*

### Comparing `DataProperty-0.8.1/dataproperty/_property_extractor.py` & `DataProperty-0.9.0/dataproperty/_property_extractor.py`

 * *Files identical despite different names*

### Comparing `DataProperty-0.8.1/misc/README_HEADER.rst` & `DataProperty-0.9.0/misc/README_HEADER.rst`

 * *Files identical despite different names*

### Comparing `DataProperty-0.8.1/misc/readme_converter.py` & `DataProperty-0.9.0/misc/readme_converter.py`

 * *Files identical despite different names*

### Comparing `DataProperty-0.8.1/test/test_align_getter.py` & `DataProperty-0.9.0/test/test_align_getter.py`

 * *Files identical despite different names*

### Comparing `DataProperty-0.8.1/test/test_column_property.py` & `DataProperty-0.9.0/test/test_column_property.py`

 * *Files identical despite different names*

### Comparing `DataProperty-0.8.1/test/test_container.py` & `DataProperty-0.9.0/test/test_container.py`

 * *Files identical despite different names*

### Comparing `DataProperty-0.8.1/test/test_converter.py` & `DataProperty-0.9.0/test/test_converter.py`

 * *Files identical despite different names*

### Comparing `DataProperty-0.8.1/test/test_converter_creator.py` & `DataProperty-0.9.0/test/test_converter_creator.py`

 * *Files identical despite different names*

### Comparing `DataProperty-0.8.1/test/test_function.py` & `DataProperty-0.9.0/test/test_function.py`

 * *Files identical despite different names*

### Comparing `DataProperty-0.8.1/test/test_property.py` & `DataProperty-0.9.0/test/test_property.py`

 * *Files identical despite different names*

### Comparing `DataProperty-0.8.1/test/test_property_extractor.py` & `DataProperty-0.9.0/test/test_property_extractor.py`

 * *Files identical despite different names*

### Comparing `DataProperty-0.8.1/test/test_type_checker.py` & `DataProperty-0.9.0/test/test_type_checker.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from decimal import Decimal
 
 
 nan = float("nan")
 inf = float("inf")
 
 
-class Test_NoneTypeChecker:
+class Test_NoneTypeChecker_is_type:
 
     @pytest.mark.parametrize(["value", "is_convert", "expected"], [
         [None, True, True],
         [None, False, True],
     ] + list(
         itertools.product(
             ["None", True, False, 0, six.MAXSIZE, inf, nan],
@@ -35,15 +35,45 @@
     )
     def test_normal_true(self, value, is_convert, expected):
         type_checker = tc.NoneTypeChecker(value, is_convert)
         assert type_checker.is_type() == expected
         assert type_checker.typecode == Typecode.NONE
 
 
-class Test_StringTypeChecker:
+class Test_NoneTypeChecker_validate:
+
+    @pytest.mark.parametrize(["value", "is_convert"], [
+        [None, True],
+        [None, False],
+    ])
+    def test_normal(self, value, is_convert):
+        type_checker = tc.NoneTypeChecker(value, is_convert)
+        type_checker.validate()
+
+    @pytest.mark.parametrize(
+        ["value", "is_convert", "exception_type", "expected"],
+        list(itertools.product(
+            ["None", True, False, 0, six.MAXSIZE, inf, nan],
+            [True, False],
+            [ValueError],
+            [ValueError]
+        )) + list(itertools.product(
+            ["None", True, False, 0, six.MAXSIZE, inf, nan],
+            [True, False],
+            [TypeError],
+            [TypeError]
+        ))
+    )
+    def test_exception(self, value, is_convert, exception_type, expected):
+        type_checker = tc.NoneTypeChecker(value, is_convert)
+        with pytest.raises(expected):
+            type_checker.validate(exception_type=exception_type)
+
+
+class Test_StringTypeChecker_is_type:
 
     @pytest.mark.parametrize(["value", "is_convert", "expected"], [
         [None, True, True],
         [None, False, False],
         [six.MAXSIZE, True, True],
         [six.MAXSIZE, False, False],
         [inf, True, True],
@@ -57,15 +87,45 @@
     )
     def test_normal_true(self, value, is_convert, expected):
         type_checker = tc.StringTypeChecker(value, is_convert)
         assert type_checker.is_type() == expected
         assert type_checker.typecode == Typecode.STRING
 
 
-class Test_IntegerTypeChecker:
+class Test_StringTypeChecker_validate:
+
+    @pytest.mark.parametrize(["value", "is_convert"],  [
+        [None, True],
+        [six.MAXSIZE, True],
+        [inf, True],
+    ] + list(
+        itertools.product(
+            ["None"],
+            [True, False],
+        ))
+    )
+    def test_normal(self, value, is_convert):
+        type_checker = tc.StringTypeChecker(value, is_convert)
+        type_checker.validate()
+
+    @pytest.mark.parametrize(
+        ["value", "is_convert", "exception_type", "expected"],
+        [
+            [None, False, ValueError, ValueError],
+            [six.MAXSIZE, False, TypeError, TypeError],
+            [inf, False, ValueError, ValueError],
+        ]
+    )
+    def test_exception(self, value, is_convert, exception_type, expected):
+        type_checker = tc.StringTypeChecker(value, is_convert)
+        with pytest.raises(expected):
+            type_checker.validate(exception_type=exception_type)
+
+
+class Test_IntegerTypeChecker_is_type:
 
     @pytest.mark.parametrize(["value", "is_convert"], [
         ["0", True],
         [" 1 ", True],
         [str(six.MAXSIZE), True], [str(-six.MAXSIZE), True],
         [Decimal("1"), True],
     ] + list(
@@ -95,15 +155,54 @@
             [True, False],
         ))
     )
     def test_normal_false(self, value, is_convert):
         assert not tc.IntegerTypeChecker(value, is_convert).is_type()
 
 
-class Test_FloatTypeChecker:
+class Test_IntegerTypeChecker_validate:
+
+    @pytest.mark.parametrize(["value", "is_convert"],  [
+        ["0", True],
+        [" 1 ", True],
+        [str(six.MAXSIZE), True], [str(-six.MAXSIZE), True],
+        [Decimal("1"), True],
+    ] + list(
+        itertools.product(
+            [0, six.MAXSIZE, -six.MAXSIZE],
+            [True, False],
+        ))
+    )
+    def test_normal(self, value, is_convert):
+        type_checker = tc.IntegerTypeChecker(value, is_convert)
+        type_checker.validate()
+
+    @pytest.mark.parametrize(["value", "is_convert"], [
+        ["0", False],
+        ["0xff", True], ["0xff", False],
+        [" 1 ", False],
+        [str(six.MAXSIZE), False], [str(-six.MAXSIZE), False],
+        [Decimal("1"), False],
+    ] + list(
+        itertools.product(
+            [
+                None, True, nan, inf, 0.5, "0.5", .999, ".999",
+                "", "test", "1a1", "11a", "a11",
+                1e-05, -1e-05, "1e-05", "-1e-05",
+            ],
+            [True, False],
+        ))
+    )
+    def test_exception(self, value, is_convert):
+        type_checker = tc.IntegerTypeChecker(value, is_convert)
+        with pytest.raises(TypeError):
+            type_checker.validate()
+
+
+class Test_FloatTypeChecker_is_type:
 
     @pytest.mark.parametrize(["value", "is_convert"], [
         [1, True],
         [-1, True],
         ["0.0", True],
         ["0.1", True], ["-0.1", True],
         ["1", True], ["-1", True],
@@ -138,15 +237,15 @@
             [True, False],
         ))
     )
     def test_normal_false(self, value, is_convert):
         assert not tc.FloatTypeChecker(value, is_convert).is_type()
 
 
-class Test_BoolTypeChecker:
+class Test_BoolTypeChecker_is_type:
 
     @pytest.mark.parametrize(["value", "is_convert"], [
         ["True", True],
         ["False", True],
         ["true", True],
         ["false", True],
     ] + list(
@@ -172,15 +271,15 @@
         ))
     )
     def test_normal_false(self, value, is_convert):
         type_checker = tc.BoolTypeChecker(value, is_convert)
         assert not type_checker.is_type()
 
 
-class Test_DateTimeTypeChecker:
+class Test_DateTimeTypeChecker_is_type:
 
     @pytest.mark.parametrize(["value", "is_convert"], [
         [
             datetime.datetime(
                 2017, 3, 22, 10, 0, tzinfo=tzoffset(None, 32400)),
             True,
         ],
@@ -207,15 +306,15 @@
         [None, False],
         [six.MAXSIZE, True], [six.MAXSIZE, False],
     ])
     def test_normal_false(self, value, is_convert):
         assert not tc.DateTimeTypeChecker(value, is_convert).is_type()
 
 
-class Test_InfinityChecker:
+class Test_InfinityChecker_is_type:
 
     @pytest.mark.parametrize(
         ["value", "is_convert", "expected"],
         list(itertools.product(
             [0.0, six.MAXSIZE, "0", nan],
             [True, False],
             [False]
@@ -232,15 +331,15 @@
     )
     def test_normal(self, value, is_convert, expected):
         type_checker = tc.InfinityChecker(value, is_convert)
         assert type_checker.is_type() == expected
         assert type_checker.typecode == Typecode.INFINITY
 
 
-class Test_NanChecker:
+class Test_NanChecker_is_type:
 
     @pytest.mark.parametrize(
         ["value", "is_convert", "expected"],
         list(itertools.product(
             [0.0, six.MAXSIZE, "0", inf],
             [True, False],
             [False]
```

### Comparing `DataProperty-0.8.1/test/test_type_checker_creator.py` & `DataProperty-0.9.0/test/test_type_checker_creator.py`

 * *Files identical despite different names*

### Comparing `DataProperty-0.8.1/LICENSE` & `DataProperty-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `DataProperty-0.8.1/README.rst` & `DataProperty-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `DataProperty-0.8.1/setup.py` & `DataProperty-0.9.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,39 +14,39 @@
 
 with open(os.path.join(REQUIREMENT_DIR, "requirements.txt")) as f:
     install_requires = [line.strip() for line in f if line.strip()]
 
 with open(os.path.join(REQUIREMENT_DIR, "test_requirements.txt")) as f:
     tests_require = [line.strip() for line in f if line.strip()]
 
-needs_pytest = set(['pytest', 'test', 'ptr']).intersection(sys.argv)
-pytest_runner = ['pytest-runner'] if needs_pytest else []
+needs_pytest = set(["pytest", "test", "ptr"]).intersection(sys.argv)
+pytest_runner = ["pytest-runner"] if needs_pytest else []
 
 author = "Tsuyoshi Hombashi"
 email = "gogogo.vm@gmail.com"
 project_name = "DataProperty"
 
 setuptools.setup(
     name=project_name,
-    version="0.8.1",
+    version="0.9.0",
     url="https://github.com/thombashi/" + project_name,
     bugtrack_url="https://github.com/thombashi/{:s}/issues".format(
         project_name),
 
     author=author,
     author_email=email,
     description=summary,
     include_package_data=True,
     install_requires=install_requires,
     keywords=["property"],
     license="MIT License",
     long_description=long_description,
     maintainer=author,
     maintainer_email=email,
-    packages=setuptools.find_packages(exclude=['test*']),
+    packages=setuptools.find_packages(exclude=["test*"]),
     setup_requires=[] + pytest_runner,
     tests_require=tests_require,
 
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
```

### Comparing `DataProperty-0.8.1/PKG-INFO` & `DataProperty-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: DataProperty
-Version: 0.8.1
+Version: 0.9.0
 Summary: Python library for extract property from data.
 
 Home-page: https://github.com/thombashi/DataProperty
 Author: Tsuyoshi Hombashi
 Author-email: gogogo.vm@gmail.com
 License: MIT License
 Description: **DataProperty**
```

