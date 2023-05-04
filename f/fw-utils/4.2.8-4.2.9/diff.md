# Comparing `tmp/fw_utils-4.2.8-py3-none-any.whl.zip` & `tmp/fw_utils-4.2.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 22038 bytes, number of entries: 14
+Zip file size: 22033 bytes, number of entries: 14
 -rw-r--r--  2.0 unx     1747 b- defN 80-Jan-01 00:00 fw_utils/__init__.py
 -rw-r--r--  2.0 unx     2914 b- defN 80-Jan-01 00:00 fw_utils/datetime.py
 -rw-r--r--  2.0 unx     3095 b- defN 80-Jan-01 00:00 fw_utils/dicts.py
 -rw-r--r--  2.0 unx     5436 b- defN 80-Jan-01 00:00 fw_utils/files.py
 -rw-r--r--  2.0 unx     8838 b- defN 80-Jan-01 00:00 fw_utils/filters.py
 -rw-r--r--  2.0 unx    10485 b- defN 80-Jan-01 00:00 fw_utils/formatters.py
 -rw-r--r--  2.0 unx    15077 b- defN 80-Jan-01 00:00 fw_utils/parsers.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 fw_utils/py.typed
 -rw-r--r--  2.0 unx     4382 b- defN 80-Jan-01 00:00 fw_utils/state.py
 -rw-r--r--  2.0 unx     3063 b- defN 80-Jan-01 00:00 fw_utils/testing.py
--rw-r--r--  2.0 unx     1078 b- defN 80-Jan-01 00:00 fw_utils-4.2.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     1928 b- defN 80-Jan-01 00:00 fw_utils-4.2.8.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_utils-4.2.8.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1054 b- defN 16-Jan-01 00:00 fw_utils-4.2.8.dist-info/RECORD
-14 files, 59185 bytes uncompressed, 20326 bytes compressed:  65.7%
+-rw-r--r--  2.0 unx     1078 b- defN 80-Jan-01 00:00 fw_utils-4.2.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1922 b- defN 80-Jan-01 00:00 fw_utils-4.2.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_utils-4.2.9.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1054 b- defN 16-Jan-01 00:00 fw_utils-4.2.9.dist-info/RECORD
+14 files, 59179 bytes uncompressed, 20321 bytes compressed:  65.7%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: fw_utils/state.py
 Comment: 
 
 Filename: fw_utils/testing.py
 Comment: 
 
-Filename: fw_utils-4.2.8.dist-info/LICENSE
+Filename: fw_utils-4.2.9.dist-info/LICENSE
 Comment: 
 
-Filename: fw_utils-4.2.8.dist-info/METADATA
+Filename: fw_utils-4.2.9.dist-info/METADATA
 Comment: 
 
-Filename: fw_utils-4.2.8.dist-info/WHEEL
+Filename: fw_utils-4.2.9.dist-info/WHEEL
 Comment: 
 
-Filename: fw_utils-4.2.8.dist-info/RECORD
+Filename: fw_utils-4.2.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `fw_utils-4.2.8.dist-info/LICENSE` & `fw_utils-4.2.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fw_utils-4.2.8.dist-info/METADATA` & `fw_utils-4.2.9.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fw-utils
-Version: 4.2.8
+Version: 4.2.9
 Summary: Common Flywheel helper utilities.
 Home-page: https://gitlab.com/flywheel-io/tools/lib/fw-utils
 License: MIT
 Keywords: Flywheel,helper,utility
 Author: Flywheel
 Author-email: support@flywheel.io
 Requires-Python: >=3.8,<4.0
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
-Requires-Dist: tzdata (>=2022,<2023)
+Requires-Dist: tzdata (>=2022)
 Requires-Dist: tzlocal (>=4.1,<5.0)
 Project-URL: Documentation, https://gitlab.com/flywheel-io/tools/lib/fw-utils
 Project-URL: Repository, https://gitlab.com/flywheel-io/tools/lib/fw-utils
 Description-Content-Type: text/markdown
 
 # fw-utils
```

## Comparing `fw_utils-4.2.8.dist-info/RECORD` & `fw_utils-4.2.9.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -4,11 +4,11 @@
 fw_utils/files.py,sha256=Jck1ZRDXkBxXeqMcKxeywPu-SzRnxQyw--WH8J8OEL8,5436
 fw_utils/filters.py,sha256=A96uXh0d0zvAxHhdDy5scaKFfxhiOVEMzztNy8kTDus,8838
 fw_utils/formatters.py,sha256=K4va7zrFj9KZDHEkzcbRlA28ZWDnOBCb8E4XFSXrM6Y,10485
 fw_utils/parsers.py,sha256=S0g7fQpudkNq8xz8BgCwgnoLnsqatFUq61PwhpSrNCA,15077
 fw_utils/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fw_utils/state.py,sha256=wsa1p60kVaoy-wLxMy5XjEmZO_A2CUjRLMgkrhgdVts,4382
 fw_utils/testing.py,sha256=e3qjGfECyiEk3BspMYTW85ZqRozxoDJjZTVu2qBdq3Y,3063
-fw_utils-4.2.8.dist-info/LICENSE,sha256=l6rSIY1z68PIZljFVsWf7vH6pbhZay7Yz2EKgbsR8q0,1078
-fw_utils-4.2.8.dist-info/METADATA,sha256=02X6ZXFEOiF0prio9At---N-OdDI1go3Z4cIBeUtJHI,1928
-fw_utils-4.2.8.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-fw_utils-4.2.8.dist-info/RECORD,,
+fw_utils-4.2.9.dist-info/LICENSE,sha256=l6rSIY1z68PIZljFVsWf7vH6pbhZay7Yz2EKgbsR8q0,1078
+fw_utils-4.2.9.dist-info/METADATA,sha256=4fj4LQlU-bnMZQRckhKUTwGD90rXFtLkEv41c6-3X38,1922
+fw_utils-4.2.9.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+fw_utils-4.2.9.dist-info/RECORD,,
```

