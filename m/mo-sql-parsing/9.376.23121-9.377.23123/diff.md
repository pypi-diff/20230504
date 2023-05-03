# Comparing `tmp/mo_sql_parsing-9.376.23121-py2.py3-none-any.whl.zip` & `tmp/mo_sql_parsing-9.377.23123-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 38165 bytes, number of entries: 13
+Zip file size: 38258 bytes, number of entries: 13
 -rw-rw-rw-  2.0 fat     2597 b- defN 22-Dec-18 22:41 mo_sql_parsing/__init__.py
 -rw-rw-rw-  2.0 fat    22229 b- defN 23-Mar-26 12:53 mo_sql_parsing/formatting.py
--rw-rw-rw-  2.0 fat    10299 b- defN 23-Apr-14 10:13 mo_sql_parsing/keywords.py
+-rw-rw-rw-  2.0 fat    10666 b- defN 23-May-03 23:07 mo_sql_parsing/keywords.py
 -rw-rw-rw-  2.0 fat    33442 b- defN 23-May-01 12:37 mo_sql_parsing/sql_parser.py
 -rw-rw-rw-  2.0 fat     7321 b- defN 23-Mar-26 12:53 mo_sql_parsing/types.py
 -rw-rw-rw-  2.0 fat    22945 b- defN 23-Apr-14 10:14 mo_sql_parsing/utils.py
 -rw-rw-rw-  2.0 fat     2987 b- defN 23-Mar-26 12:53 mo_sql_parsing/windows.py
--rw-rw-rw-  2.0 fat    15922 b- defN 23-May-01 12:37 mo_sql_parsing-9.376.23121.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     9345 b- defN 23-May-01 12:37 mo_sql_parsing-9.376.23121.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-May-01 12:37 mo_sql_parsing-9.376.23121.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 23-May-01 12:37 mo_sql_parsing-9.376.23121.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat        2 b- defN 23-May-01 12:37 mo_sql_parsing-9.376.23121.dist-info/zip-safe
-?rw-rw-r--  2.0 fat     1134 b- defN 23-May-01 12:37 mo_sql_parsing-9.376.23121.dist-info/RECORD
-13 files, 128348 bytes uncompressed, 36259 bytes compressed:  71.7%
+-rw-rw-rw-  2.0 fat    15922 b- defN 23-May-03 23:07 mo_sql_parsing-9.377.23123.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     9345 b- defN 23-May-03 23:07 mo_sql_parsing-9.377.23123.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-May-03 23:07 mo_sql_parsing-9.377.23123.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 23-May-03 23:07 mo_sql_parsing-9.377.23123.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 23-May-03 23:07 mo_sql_parsing-9.377.23123.dist-info/zip-safe
+?rw-rw-r--  2.0 fat     1134 b- defN 23-May-03 23:07 mo_sql_parsing-9.377.23123.dist-info/RECORD
+13 files, 128715 bytes uncompressed, 36352 bytes compressed:  71.8%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: mo_sql_parsing/utils.py
 Comment: 
 
 Filename: mo_sql_parsing/windows.py
 Comment: 
 
-Filename: mo_sql_parsing-9.376.23121.dist-info/LICENSE
+Filename: mo_sql_parsing-9.377.23123.dist-info/LICENSE
 Comment: 
 
-Filename: mo_sql_parsing-9.376.23121.dist-info/METADATA
+Filename: mo_sql_parsing-9.377.23123.dist-info/METADATA
 Comment: 
 
-Filename: mo_sql_parsing-9.376.23121.dist-info/WHEEL
+Filename: mo_sql_parsing-9.377.23123.dist-info/WHEEL
 Comment: 
 
-Filename: mo_sql_parsing-9.376.23121.dist-info/top_level.txt
+Filename: mo_sql_parsing-9.377.23123.dist-info/top_level.txt
 Comment: 
 
-Filename: mo_sql_parsing-9.376.23121.dist-info/zip-safe
+Filename: mo_sql_parsing-9.377.23123.dist-info/zip-safe
 Comment: 
 
-Filename: mo_sql_parsing-9.376.23121.dist-info/RECORD
+Filename: mo_sql_parsing-9.377.23123.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mo_sql_parsing/keywords.py

```diff
@@ -373,56 +373,71 @@
     "msecs": "millisecond",
     "msec": "millisecond",
     "ms": "millisecond",
     "seconds": "second",
     "second": "second",
     "secs": "second",
     "sec": "second",
-    "s": "second",
     "minutes": "minute",
     "minute": "minute",
     "mins": "minute",
     "min": "minute",
     "hours": "hour",
     "hour": "hour",
     "hrs": "hour",
     "hr": "hour",
-    "h": "hour",
-    "days": "day",
-    "dayofyear": "doy",
+    "day_of_week": "dow",
     "dayofweek": "dow",
-    "day": "day",
-    "date": "date",
-    "d": "day",
     "dow": "dow",
+    "day_of_month": "dom",
+    "dayofmonth": "dom",
+    "dom": "dow",
+    "day_of_year": "doy",
+    "dayofyear": "doy",
+    "doy": "doy",
+    "date": "date",
+    "days": "day",
+    "day": "day",
     "weekday": "dow",
     "weeks": "week",
     "week": "week",
-    "w": "week",
     "isoweek": "isoweek",
     "months": "month",
     "month": "month",
     "mons": "month",
     "mon": "month",
-    "m": "minute",
-    "M": "month",
     "quarters": "quarter",
     "quarter": "quarter",
+    "year_of_week": "yow",
+    "yearofweek": "yow",
     "years": "year",
     "year": "year",
-    "y": "year",
+    "yow": "yow",
+    "isodow": "isodow",
     "isoyear": "isoyear",
     "decades": "decade",
     "decade": "decade",
     "decs": "decade",
     "dec": "decade",
     "centuries": "century",
     "century": "century",
     "cents": "century",
     "cent": "century",
-    "c": "century",
     "millennia": "millennium",
     "millennium": "millennium",
     "mils": "millennium",
     "mil": "millennium",
     "epoch": "epoch",
+    "julian": "julian",
+    "timezone_minute": "timezone_minute",
+    "timezone_hour": "timezone_hour",
+    "timezone": "timezone",
+    "s": "second",
+    "m": "minute",
+    "h": "hour",
+    "d": "day",
+    "w": "week",
+    "M": "month",
+    "y": "year",
+    "c": "century",
+
 }
```

## Comparing `mo_sql_parsing-9.376.23121.dist-info/LICENSE` & `mo_sql_parsing-9.377.23123.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mo_sql_parsing-9.376.23121.dist-info/METADATA` & `mo_sql_parsing-9.377.23123.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-sql-parsing
-Version: 9.376.23121
+Version: 9.377.23123
 Summary: More SQL Parsing! Parse SQL into JSON parse tree
 Home-page: https://github.com/klahnakoski/mo-sql-parsing
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Software Development :: Libraries
```

