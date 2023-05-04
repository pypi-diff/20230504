# Comparing `tmp/yetl-framework-0.0.9.tar.gz` & `tmp/yetl-framework-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yetl-framework-0.0.9.tar", last modified: Thu Aug 11 22:30:48 2022, max compression
+gzip compressed data, was "yetl-framework-1.0.0.tar", last modified: Thu May  4 12:16:49 2023, max compression
```

## Comparing `yetl-framework-0.0.9.tar` & `yetl-framework-1.0.0.tar`

### file list

```diff
@@ -1,53 +1,37 @@
-drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2022-08-11 22:30:48.229926 yetl-framework-0.0.9/
--rw-r--r--   0 shaunryan   (501) staff       (20)     1067 2022-07-24 07:32:49.000000 yetl-framework-0.0.9/LICENSE
--rw-r--r--   0 shaunryan   (501) staff       (20)     5212 2022-08-11 22:30:48.228646 yetl-framework-0.0.9/PKG-INFO
--rw-r--r--   0 shaunryan   (501) staff       (20)     3687 2022-08-11 22:27:07.000000 yetl-framework-0.0.9/README.md
--rw-r--r--   0 shaunryan   (501) staff       (20)       38 2022-08-11 22:30:48.230042 yetl-framework-0.0.9/setup.cfg
--rw-r--r--   0 shaunryan   (501) staff       (20)      913 2022-08-11 22:29:31.000000 yetl-framework-0.0.9/setup.py
-drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2022-08-11 22:30:48.205771 yetl-framework-0.0.9/test/
--rw-r--r--   0 shaunryan   (501) staff       (20)     1923 2022-07-24 07:32:49.000000 yetl-framework-0.0.9/test/test_pipeline.py
-drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2022-08-11 22:30:48.209254 yetl-framework-0.0.9/yetl_flow/
--rw-r--r--   0 shaunryan   (501) staff       (20)      649 2022-08-01 20:54:40.000000 yetl-framework-0.0.9/yetl_flow/__init__.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     1277 2022-07-30 09:06:19.000000 yetl-framework-0.0.9/yetl_flow/_config_provider.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     3785 2022-08-06 08:25:27.000000 yetl-framework-0.0.9/yetl_flow/_context.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     2767 2022-07-26 06:06:34.000000 yetl-framework-0.0.9/yetl_flow/_delta_lake.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     2885 2022-08-01 21:01:24.000000 yetl-framework-0.0.9/yetl_flow/_framework.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     1423 2022-07-31 09:40:59.000000 yetl-framework-0.0.9/yetl_flow/_logging_config.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     6489 2022-08-04 22:52:14.000000 yetl-framework-0.0.9/yetl_flow/_timeslice.py
-drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2022-08-11 22:30:48.211101 yetl-framework-0.0.9/yetl_flow/dataflow/
--rw-r--r--   0 shaunryan   (501) staff       (20)      104 2022-07-24 07:33:05.000000 yetl-framework-0.0.9/yetl_flow/dataflow/__init__.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     2790 2022-07-31 18:52:12.000000 yetl-framework-0.0.9/yetl_flow/dataflow/_dataflow.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     1752 2022-07-31 18:52:12.000000 yetl-framework-0.0.9/yetl_flow/dataflow/_i_dataflow.py
-drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2022-08-11 22:30:48.219225 yetl-framework-0.0.9/yetl_flow/dataset/
--rw-r--r--   0 shaunryan   (501) staff       (20)      706 2022-07-31 18:52:12.000000 yetl-framework-0.0.9/yetl_flow/dataset/__init__.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     1448 2022-07-31 10:20:58.000000 yetl-framework-0.0.9/yetl_flow/dataset/_builtin_functions.py
--rw-r--r--   0 shaunryan   (501) staff       (20)      701 2022-08-04 20:23:17.000000 yetl-framework-0.0.9/yetl_flow/dataset/_constants.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     1616 2022-07-24 07:33:05.000000 yetl-framework-0.0.9/yetl_flow/dataset/_dataset.py
--rw-r--r--   0 shaunryan   (501) staff       (20)      511 2022-07-31 18:43:23.000000 yetl-framework-0.0.9/yetl_flow/dataset/_destination.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     2244 2022-07-31 22:42:39.000000 yetl-framework-0.0.9/yetl_flow/dataset/_factory.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     8508 2022-08-11 21:42:22.000000 yetl-framework-0.0.9/yetl_flow/dataset/_reader.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     2402 2022-07-31 22:28:05.000000 yetl-framework-0.0.9/yetl_flow/dataset/_save.py
--rw-r--r--   0 shaunryan   (501) staff       (20)      682 2022-07-24 07:33:05.000000 yetl-framework-0.0.9/yetl_flow/dataset/_source.py
--rw-r--r--   0 shaunryan   (501) staff       (20)      238 2022-07-24 07:33:05.000000 yetl-framework-0.0.9/yetl_flow/dataset/_stream_reader.py
--rw-r--r--   0 shaunryan   (501) staff       (20)      253 2022-07-24 07:33:05.000000 yetl-framework-0.0.9/yetl_flow/dataset/_stream_writer.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     4452 2022-08-11 22:25:02.000000 yetl-framework-0.0.9/yetl_flow/dataset/_validation.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     7856 2022-07-31 16:43:20.000000 yetl-framework-0.0.9/yetl_flow/dataset/_writer.py
-drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2022-08-11 22:30:48.223307 yetl-framework-0.0.9/yetl_flow/file_system/
--rw-r--r--   0 shaunryan   (501) staff       (20)      344 2022-07-30 10:03:59.000000 yetl-framework-0.0.9/yetl_flow/file_system/__init__.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     1793 2022-07-30 10:21:05.000000 yetl-framework-0.0.9/yetl_flow/file_system/_dbfs_file_system.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     2286 2022-07-30 10:22:33.000000 yetl-framework-0.0.9/yetl_flow/file_system/_factory.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     3636 2022-07-30 10:21:05.000000 yetl-framework-0.0.9/yetl_flow/file_system/_file_system.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     1377 2022-07-30 10:21:05.000000 yetl-framework-0.0.9/yetl_flow/file_system/_ifile_system.py
-drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2022-08-11 22:30:48.225615 yetl-framework-0.0.9/yetl_flow/schema_repo/
--rw-r--r--   0 shaunryan   (501) staff       (20)      317 2022-07-24 07:33:05.000000 yetl-framework-0.0.9/yetl_flow/schema_repo/__init__.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     2192 2022-07-30 10:47:33.000000 yetl-framework-0.0.9/yetl_flow/schema_repo/_deltalake_sql_file.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     1770 2022-07-24 07:33:05.000000 yetl-framework-0.0.9/yetl_flow/schema_repo/_factory.py
--rw-r--r--   0 shaunryan   (501) staff       (20)      388 2022-07-24 07:33:05.000000 yetl-framework-0.0.9/yetl_flow/schema_repo/_ischema_repo.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     2751 2022-08-05 21:43:57.000000 yetl-framework-0.0.9/yetl_flow/schema_repo/_spark_file_schema_repo.py
-drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2022-08-11 22:30:48.228225 yetl-framework-0.0.9/yetl_framework.egg-info/
--rw-r--r--   0 shaunryan   (501) staff       (20)     5212 2022-08-11 22:30:48.000000 yetl-framework-0.0.9/yetl_framework.egg-info/PKG-INFO
--rw-r--r--   0 shaunryan   (501) staff       (20)     1351 2022-08-11 22:30:48.000000 yetl-framework-0.0.9/yetl_framework.egg-info/SOURCES.txt
--rw-r--r--   0 shaunryan   (501) staff       (20)        1 2022-08-11 22:30:48.000000 yetl-framework-0.0.9/yetl_framework.egg-info/dependency_links.txt
--rw-r--r--   0 shaunryan   (501) staff       (20)        1 2022-08-07 20:35:25.000000 yetl-framework-0.0.9/yetl_framework.egg-info/not-zip-safe
--rw-r--r--   0 shaunryan   (501) staff       (20)       33 2022-08-11 22:30:48.000000 yetl-framework-0.0.9/yetl_framework.egg-info/requires.txt
--rw-r--r--   0 shaunryan   (501) staff       (20)       10 2022-08-11 22:30:48.000000 yetl-framework-0.0.9/yetl_framework.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-04 12:16:49.997215 yetl-framework-1.0.0/
+-rw-r--r--   0 vsts      (1001) docker     (123)     4615 2023-05-04 12:16:49.997215 yetl-framework-1.0.0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     4118 2023-05-04 12:15:59.000000 yetl-framework-1.0.0/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-04 12:16:49.997215 yetl-framework-1.0.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1043 2023-05-04 12:15:59.000000 yetl-framework-1.0.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-04 12:16:49.993215 yetl-framework-1.0.0/yetl/
+-rw-r--r--   0 vsts      (1001) docker     (123)      455 2023-05-04 12:15:59.000000 yetl-framework-1.0.0/yetl/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3148 2023-05-04 12:15:59.000000 yetl-framework-1.0.0/yetl/_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1994 2023-05-04 12:15:59.000000 yetl-framework-1.0.0/yetl/_decorators.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-05-04 12:15:59.000000 yetl-framework-1.0.0/yetl/_logging_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-05-04 12:15:59.000000 yetl-framework-1.0.0/yetl/_project.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1399 2023-05-04 12:15:59.000000 yetl-framework-1.0.0/yetl/_spark_context.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      158 2023-05-04 12:15:59.000000 yetl-framework-1.0.0/yetl/_stage_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      305 2023-05-04 12:15:59.000000 yetl-framework-1.0.0/yetl/_table_mapping.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7311 2023-05-04 12:15:59.000000 yetl-framework-1.0.0/yetl/_tables.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5706 2023-05-04 12:15:59.000000 yetl-framework-1.0.0/yetl/_timeslice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4717 2023-05-04 12:15:59.000000 yetl-framework-1.0.0/yetl/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6667 2023-05-04 12:15:59.000000 yetl-framework-1.0.0/yetl/datallake.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-04 12:16:49.993215 yetl-framework-1.0.0/yetl/dataset/
+-rw-r--r--   0 vsts      (1001) docker     (123)      217 2023-05-04 12:15:59.000000 yetl-framework-1.0.0/yetl/dataset/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1203 2023-05-04 12:15:59.000000 yetl-framework-1.0.0/yetl/dataset/_dataset.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3242 2023-05-04 12:15:59.000000 yetl-framework-1.0.0/yetl/dataset/_deltalake.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3947 2023-05-04 12:15:59.000000 yetl-framework-1.0.0/yetl/dataset/_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5274 2023-05-04 12:15:59.000000 yetl-framework-1.0.0/yetl/dataset/_read.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      259 2023-05-04 12:15:59.000000 yetl-framework-1.0.0/yetl/dataset/_write.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      198 2023-05-04 12:15:59.000000 yetl-framework-1.0.0/yetl/dataset/dataset_type.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-04 12:16:49.993215 yetl-framework-1.0.0/yetl/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-05-04 12:15:59.000000 yetl-framework-1.0.0/yetl/workflow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-05-04 12:15:59.000000 yetl-framework-1.0.0/yetl/workflow/_multi_threaded.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-05-04 12:15:59.000000 yetl-framework-1.0.0/yetl/workflow/_notebook.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-04 12:16:49.993215 yetl-framework-1.0.0/yetl_framework.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     4615 2023-05-04 12:16:49.000000 yetl-framework-1.0.0/yetl_framework.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      734 2023-05-04 12:16:49.000000 yetl-framework-1.0.0/yetl_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-04 12:16:49.000000 yetl-framework-1.0.0/yetl_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-04 12:16:49.000000 yetl-framework-1.0.0/yetl_framework.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       23 2023-05-04 12:16:49.000000 yetl-framework-1.0.0/yetl_framework.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-05-04 12:16:49.000000 yetl-framework-1.0.0/yetl_framework.egg-info/top_level.txt
```

### Comparing `yetl-framework-0.0.9/yetl_flow/_timeslice.py` & `yetl-framework-1.0.0/yetl/_timeslice.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from datetime import datetime
 from typing import Literal, Union
-
+from pydantic import BaseModel, Field
+from typing import Any
 
 _WILDCARD = "*"
 Wildcard = Literal["*"]
 
 _UNSUPPORTED_FORMAT_CODES = [
     "%c",
     "%x",
@@ -20,58 +21,40 @@
     "%B",
     "%a",
     "%A",
     "%w",
 ]
 
 
-class Timeslice:
-    def __init__(
-        self,
-        year: Union[int, Wildcard],
-        month: Union[int, Wildcard] = None,
-        day: Union[int, Wildcard] = None,
-        hour: Union[int, Wildcard] = 0,
-        minute: Union[int, Wildcard] = 0,
-        second: Union[int, Wildcard] = 0,
-        microsecond: Union[int, Wildcard] = 0,
-    ) -> None:
-
-        self.year = self._wildcard_check(year)
-        self.month = self._wildcard_check(month)
-        self.day = self._wildcard_check(day)
-        self.hour = self._wildcard_check(hour)
-        self.minutue = self._wildcard_check(minute)
-        self.second = self._wildcard_check(second)
-        self.microsecond = self._wildcard_check(microsecond)
-
-    def _wildcard_check(self, value: Union[int, Wildcard]):
-        if isinstance(value, int):
-            return value
-        if isinstance(value, str) and value == _WILDCARD:
-            return value
-        else:
-            raise Exception(f"Timeslice parameters must be an int or '{_WILDCARD}'")
+class Timeslice(BaseModel):
+    def __init__(__pydantic_self__, **data: Any) -> None:
+        super().__init__(**data)
+
+    year: Union[int, Wildcard] = Field(...)
+    month: Union[int, Wildcard] = Field(default=_WILDCARD)
+    day: Union[int, Wildcard] = Field(default=_WILDCARD)
+    hour: Union[int, Wildcard] = Field(default=0)
+    minute: Union[int, Wildcard] = Field(default=0)
+    second: Union[int, Wildcard] = Field(default=0)
+    microsecond: Union[int, Wildcard] = Field(default=0)
 
     def strftime(self, format: str):
         """This will format and return the timeslice using python format codes. Only a subset of format codes are suppoered by design
-
         %d - Day of the month as a zero-padded decimal number.
         %m - Month as a zero-padded decimal number.
         %y - Year without century as a zero-padded decimal number.
         %Y - Year with century as a decimal number.
         %H - Hour (24-hour clock) as a zero-padded decimal number.
         %M - Minute as a zero-padded decimal number.
         %S - Second as a zero-padded decimal number.
         %f - Microsecond as a decimal number, zero-padded to 6 digits.
         %% - A literal '%' character.
         %j - Day of the year as a zero-padded decimal number.
         %U - Week number of the year (Sunday as the first day of the week) as a zero-padded decimal number. All days in a new year preceding the first Sunday are considered to be in week 0.
         %W - Week number of the year (Monday as the first day of the week) as a zero-padded decimal number. All days in a new year preceding the first Monday are considered to be in week 0.
-
         NOT SUPPORTED - %c - Locale’s appropriate date and time representation.
         NOT SUPPORTED - %x - Locale’s appropriate date representation.
         NOT SUPPORTED - %X - Locale’s appropriate time representation.
         NOT SUPPORTED - %G - ISO 8601 year with century representing the year that contains the greater part of the ISO week (%V).
         NOT SUPPORTED - %u - ISO 8601 weekday as a decimal number where 1 is Monday.
         NOT SUPPORTED - %V - ISO 8601 week as a decimal number with Monday as the first day of the week. Week 01 is the week containing Jan 4.
         NOT SUPPORTED - %z - UTC offset in the form ±HHMM[SS[.ffffff]] (empty string if the object is naive).
@@ -80,58 +63,46 @@
         NOT SUPPORTED - %p - Locale’s equivalent of either AM or PM.
         NOT SUPPORTED - %b - Month as locale’s abbreviated name.
         NOT SUPPORTED - %B - Month as locale’s full name.
         NOT SUPPORTED - %a - Weekday as locale’s abbreviated name.
         NOT SUPPORTED - %A - Weekday as locale’s full name.
         NOT SUPPORTED - %w - Weekday as a decimal number, where 0 is Sunday and 6 is Saturday.
         """
-        # format = "%Y%m%d"
-        unsupported_codes = []
-        for c in _UNSUPPORTED_FORMAT_CODES:
-            if c in format:
-                unsupported_codes.append(c)
+
+        unsupported_codes = [c for c in _UNSUPPORTED_FORMAT_CODES if c in format]
 
         if unsupported_codes:
             unsupported_codes = ",".join(unsupported_codes)
             raise Exception(
                 f"The format contains the following unsupported format codes: {unsupported_codes}"
             )
 
-        if not self.day and any(fmt_code in format for fmt_code in ["%d", "%j"]):
-            raise Exception(
-                f"Timeslice does not contain day (day=None) failed to format timeslice with FormatCode = [%d,%j]"
-            )
+        format, _year = self._format_wildcard(format, self.year, ["%y", "%Y"], 1900)
+        format, _month = self._format_wildcard(format, self.month, "%m", 1)
+        format, _day = self._format_wildcard(format, self.day, "%d", 1)
+
+        format, _hour = self._format_wildcard(format, self.hour, "%H")
+        format, _minutue = self._format_wildcard(format, self.minute, "%M")
+        format, _second = self._format_wildcard(format, self.second, "%S")
+        format, _microsecond = self._format_wildcard(format, self.microsecond, "%f")
 
-        if not self.month and "%m" in format:
-            raise Exception(
-                f"Timeslice does not contain month (month=None) failed to format timeslice with FormatCode = %m"
-            )
-
-        format, year = self._format_wildcard(format, self.year, ["%y", "%Y"], 1900)
-        format, month = self._format_wildcard(format, self.month, "%m", 1)
-        format, day = self._format_wildcard(format, self.day, "%d", 1)
-
-        format, hour = self._format_wildcard(format, self.hour, "%H")
-        format, minutue = self._format_wildcard(format, self.minutue, "%M")
-        format, second = self._format_wildcard(format, self.second, "%S")
-        format, microsecond = self._format_wildcard(format, self.microsecond, "%f")
-
-        timeslice = datetime(year, month, day, hour, minutue, second, microsecond)
+        timeslice = datetime(
+            _year, _month, _day, _hour, _minutue, _second, _microsecond
+        )
 
         formatted = timeslice.strftime(format)
         return formatted
 
     def _format_wildcard(
         self,
         format: str,
         datepart: Union[int, Wildcard],
         format_code: Union[list, str],
         default=0,
     ):
-
         if datepart == _WILDCARD:
             if isinstance(format_code, str):
                 format = format.replace(format_code, f"{_WILDCARD}")
             elif isinstance(format_code, list):
                 for f in format_code:
                     format = format.replace(f, f"{_WILDCARD}")
             datepart = default
@@ -141,30 +112,32 @@
     def __str__(self) -> str:
         return self.strftime("%Y-%m-%d %H:%M:%S.%f")
 
 
 class TimesliceNow(Timeslice):
     def __init__(self) -> None:
         now = datetime.now()
-        super().__init__(
-            now.year,
-            now.month,
-            now.day,
-            now.hour,
-            now.minute,
-            now.second,
-            now.microsecond,
-        )
+        args = {
+            "year": now.year,
+            "month": now.month,
+            "day": now.day,
+            "hour": now.hour,
+            "minute": now.minute,
+            "second": now.second,
+            "microsecond": now.microsecond,
+        }
+        super().__init__(**args)
 
 
 class TimesliceUtcNow(Timeslice):
     def __init__(self) -> None:
         now = datetime.utcnow()
-        super().__init__(
-            now.year,
-            now.month,
-            now.day,
-            now.hour,
-            now.minute,
-            now.second,
-            now.microsecond,
-        )
+        args = {
+            "year": now.year,
+            "month": now.month,
+            "day": now.day,
+            "hour": now.hour,
+            "minute": now.minute,
+            "second": now.second,
+            "microsecond": now.microsecond,
+        }
+        super().__init__(**args)
```

