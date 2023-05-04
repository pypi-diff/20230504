# Comparing `tmp/dknovautils-0.1.0.tar.gz` & `tmp/dknovautils-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dknovautils-0.1.0.tar", last modified: Mon May  1 03:49:03 2023, max compression
+gzip compressed data, was "dist/dknovautils-0.1.1.tar", last modified: Thu May  4 06:08:10 2023, max compression
```

## Comparing `dknovautils-0.1.0.tar` & `dknovautils-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-05-01 03:49:03.000000 dknovautils-0.1.0/
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-05-01 03:49:03.000000 dknovautils-0.1.0/dknovautils/
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     2902 2023-05-01 03:41:15.000000 dknovautils-0.1.0/dknovautils/commons.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     8009 2023-05-01 03:49:02.000000 dknovautils-0.1.0/dknovautils/dkat.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1510 2023-04-13 12:40:40.000000 dknovautils-0.1.0/dknovautils/dkfiles.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1149 2023-04-22 02:58:52.000000 dknovautils-0.1.0/dknovautils/dkipy.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      711 2023-05-01 03:49:02.000000 dknovautils-0.1.0/dknovautils/dk_imports.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      490 2023-04-13 12:40:48.000000 dknovautils-0.1.0/dknovautils/example.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      140 2023-04-13 15:12:06.000000 dknovautils-0.1.0/dknovautils/myadd.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      160 2023-04-13 15:11:54.000000 dknovautils-0.1.0/dknovautils/mysubtract.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      307 2023-04-21 15:52:41.000000 dknovautils-0.1.0/dknovautils/__init__.py
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-05-01 03:49:03.000000 dknovautils-0.1.0/dknovautils.egg-info/
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)        1 2023-05-01 03:49:02.000000 dknovautils-0.1.0/dknovautils.egg-info/dependency_links.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      880 2023-05-01 03:49:02.000000 dknovautils-0.1.0/dknovautils.egg-info/PKG-INFO
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)       12 2023-05-01 03:49:02.000000 dknovautils-0.1.0/dknovautils.egg-info/requires.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      407 2023-05-01 03:49:02.000000 dknovautils-0.1.0/dknovautils.egg-info/SOURCES.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)       12 2023-05-01 03:49:02.000000 dknovautils-0.1.0/dknovautils.egg-info/top_level.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      105 2023-03-09 04:32:08.000000 dknovautils-0.1.0/LICENSE
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      880 2023-05-01 03:49:03.000000 dknovautils-0.1.0/PKG-INFO
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      472 2023-03-09 06:46:27.000000 dknovautils-0.1.0/README.md
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)       38 2023-05-01 03:49:03.000000 dknovautils-0.1.0/setup.cfg
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1157 2023-05-01 03:49:02.000000 dknovautils-0.1.0/setup.py
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-05-04 06:08:10.000000 dknovautils-0.1.1/
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-05-04 06:08:10.000000 dknovautils-0.1.1/dknovautils/
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     2903 2023-05-02 15:06:54.000000 dknovautils-0.1.1/dknovautils/commons.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     7953 2023-05-04 06:08:06.000000 dknovautils-0.1.1/dknovautils/dkat.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      103 2023-05-04 04:54:01.000000 dknovautils-0.1.1/dknovautils/dkfiles.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1149 2023-04-22 02:58:52.000000 dknovautils-0.1.1/dknovautils/dkipy.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      711 2023-05-04 06:08:06.000000 dknovautils-0.1.1/dknovautils/dk_imports.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      490 2023-04-13 12:40:48.000000 dknovautils-0.1.1/dknovautils/example.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      140 2023-04-13 15:12:06.000000 dknovautils-0.1.1/dknovautils/myadd.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      160 2023-04-13 15:11:54.000000 dknovautils-0.1.1/dknovautils/mysubtract.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      307 2023-04-21 15:52:41.000000 dknovautils-0.1.1/dknovautils/__init__.py
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-05-04 06:08:10.000000 dknovautils-0.1.1/dknovautils.egg-info/
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)        1 2023-05-04 06:08:09.000000 dknovautils-0.1.1/dknovautils.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      880 2023-05-04 06:08:09.000000 dknovautils-0.1.1/dknovautils.egg-info/PKG-INFO
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)       12 2023-05-04 06:08:09.000000 dknovautils-0.1.1/dknovautils.egg-info/requires.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      407 2023-05-04 06:08:09.000000 dknovautils-0.1.1/dknovautils.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)       12 2023-05-04 06:08:09.000000 dknovautils-0.1.1/dknovautils.egg-info/top_level.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      105 2023-03-09 04:32:08.000000 dknovautils-0.1.1/LICENSE
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      880 2023-05-04 06:08:10.000000 dknovautils-0.1.1/PKG-INFO
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      472 2023-03-09 06:46:27.000000 dknovautils-0.1.1/README.md
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)       38 2023-05-04 06:08:10.000000 dknovautils-0.1.1/setup.cfg
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1157 2023-05-04 06:08:06.000000 dknovautils-0.1.1/setup.py
```

### Comparing `dknovautils-0.1.0/dknovautils/commons.py` & `dknovautils-0.1.1/dknovautils/commons.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 def dtprint(s: str):
     print(s)
 
 
 def iprint(obj):
-    iprint_info(obj)
+    iprint_debug(obj)
 
 
 def iprint_trace(obj):
     _iprint(obj, level=LLevel.Trace)
 
 
 def iprint_debug(obj):
```

### Comparing `dknovautils-0.1.0/dknovautils/dkat.py` & `dknovautils-0.1.1/dknovautils/dkat.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 import dknovautils
 from dknovautils.commons import *
 
 import beepy
 
 
-DkAppVer = '0.1.0'
+DkAppVer = '0.1.1'
 _unknown_err = '_unknown_err4035'
 
 
 class AT(object):
 
     _innerLoggerFun_ = None
 
@@ -64,19 +64,18 @@
     # _DATE_FORMAT_iso_simple = "%m/%d/%Y %H:%M:%S %p"
 
     STRFMT_ISO_COMPACT_SIMPLE = "%Y%m%dT%H%M%S"
     STRFMT_ISO_COMPACT_ALL_A = "%Y%m%dT%H%M%SS%fZ%Z"
     STRFMT_ISO_ALL_A = "%Y-%m-%dT%H:%M:%S.%f%Z"
     STRFMT_ISO_SEC_A = "%Y-%m-%dT%H:%M:%S"
 
-    STRFMT_LOGGER_MS_A = "%Y-%m-%d %H:%M:%S.%f"    
+    STRFMT_LOGGER_MS_A = "%Y-%m-%d %H:%M:%S.%f"
 
     _default_time_format = '%Y-%m-%d %H:%M:%S'
 
-
     _LOG_FORMAT_106 = '%(asctime)s.%(msecs)03d %(name)s %(threadName)s [%(levelname)s] %(message)s'
 
     '''
     
     dtstr = datetime.now().strftime("%Y%m%dT%H%M%S")
 
         
@@ -142,24 +141,24 @@
         beepy.beep(sound=tone)
 
     @staticmethod
     def beep2():
         #!wget -q -T 1 http://localhost:333/hello
         print('\7')
 
-    @staticmethod
-    def never(s=None):
-        AT.assert_(False,  s if s is not None else 'never come here')
+    @classmethod
+    def never(cls,s=None):
+        AT.assert_(False,  s if s is not None else 'should never come here')
 
     @staticmethod
     def checksys():
         assert sys.version_info >= (3, 11)
 
-    @staticmethod
-    def fepochMillis() -> int:
+    @classmethod
+    def fepochMillis(cls) -> int:
         millisec = int(AT.fepochSecs() * 1000)
         return millisec
 
     _last_epochsecs = 0.0
 
     @classmethod
     def fepochSecs(cls) -> float:
@@ -183,28 +182,28 @@
     # 20200101T120000
     dts = datetime.now().strftime("%Y%m%dT%H%M%S")
     print("date and time =", dts)
     
     
     '''
 
-    @staticmethod
-    def sdf_isocompact_format_datetime(dt=None, *, precise: str = 's'):
-        assert precise in ['d', 's','ms','a'], 'err5554 bad precise'
+    @classmethod
+    def sdf_isocompact_format_datetime(cls,dt=None, *, precise: str = 's'):
+        assert precise in ['d', 's', 'ms', 'a'], 'err5554 bad precise'
 
         if dt is not None:
             AT.unsupported()
 
         dt = AT._now_dt()
         dts = dt.strftime(AT.STRFMT_ISO_COMPACT_ALL_A)
 
         if precise == 'a':
             pass
         elif precise == 'ms':
-            dts = dts[:(8+0+1+6+4)]        
+            dts = dts[:(8+0+1+6+4)]
         elif precise == 's':
             dts = dts[:(8+0+1+6)]
         elif precise == 'd':
             dts = dts[:(8)]
         else:
             AT.never()
 
@@ -215,16 +214,16 @@
         pass
 
     @staticmethod
     def _now_dt():
         dt = datetime.now()
         return dt
 
-    @staticmethod
-    def sdf_logger_format_datetime(dt: int = None, *, precise: str = 's') -> str:
+    @classmethod
+    def sdf_logger_format_datetime(cls,dt: int = None, *, precise: str = 's') -> str:
         '''
 https://strftime.org/    
 https://docs.python.org/3/library/datetime.html#strftime-and-strptime-format-codes
 https://man7.org/linux/man-pages/man3/strftime.3.html
 
 2023-12-01T08:30:00.123456
 
@@ -234,27 +233,27 @@
 
 d date
 s seconds
 ms millis
 a all
 
         '''
-        assert precise in ['d', 's','ms','a'], 'err5554 bad precise'
+        assert precise in ['d', 's', 'ms', 'a'], 'err5554 bad precise'
 
         if dt is not None:
             dt = datetime.fromtimestamp(dt/1000, tz=None)
         else:
             dt = datetime.now()
 
         dts = dt.strftime(AT.STRFMT_ISO_ALL_A)
 
         if precise == 'a':
             pass
         elif precise == 'ms':
-            dts = dts[:(10+1+8+4)]        
+            dts = dts[:(10+1+8+4)]
         elif precise == 's':
             dts = dts[:(10+1+8)]
         elif precise == 'd':
             dts = dts[:(10)]
         else:
             AT.never()
 
@@ -278,30 +277,30 @@
 
     @staticmethod
     def mychdir(s):
         assert isinstance(s, str) and len(s) > 0
         iprint_debug(f'chdir: {s}')
         os.chdir(s)
 
-    @staticmethod
-    def never(s=None):
-        AT.assert_(False, f"should never come here {s}")
+    # @staticmethod
+    # def never(s=None):
+    #     AT.assert_(False, f"should never come here {s}")
 
     @staticmethod
     def astTrace(b: bool, s: str):
         '''在prod中完全不需要的'''
         AT.assert_(b, s)
 
     @staticmethod
-    def unsupported(s: str = None):
-        AT.assert_(False, s if s is not None else 'err8255 unsupported 不支持的功能')
+    def unsupported(s: str = 'feature'):
+        AT.assert_(False, f'err8255 unsupported "{s}"')
 
     @staticmethod
-    def unimplemented(s: str = None):
-        AT.assert_(False, s if s is not None else 'err4823 unimplemented 未实现的功能')
+    def unimplemented(s: str = 'feature'):
+        AT.assert_(False, f'err4173 unimplemented "{s}"')
 
     VERSION = DkAppVer
 
 
 class DkAstException(Exception):
     pass
```

### Comparing `dknovautils-0.1.0/dknovautils/dkipy.py` & `dknovautils-0.1.1/dknovautils/dkipy.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.1.0/dknovautils/dk_imports.py` & `dknovautils-0.1.1/dknovautils/dk_imports.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.1.0/dknovautils.egg-info/PKG-INFO` & `dknovautils-0.1.1/dknovautils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dknovautils
-Version: 0.1.0
+Version: 0.1.1
 Summary: This is the tools for dknova.
 Home-page: http://example.com
 Author: dknova
 Author-email: dknova@example.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dknovautils-0.1.0/PKG-INFO` & `dknovautils-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dknovautils
-Version: 0.1.0
+Version: 0.1.1
 Summary: This is the tools for dknova.
 Home-page: http://example.com
 Author: dknova
 Author-email: dknova@example.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dknovautils-0.1.0/setup.py` & `dknovautils-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import re
 import setuptools
 
 from distutils.core import setup
 from setuptools import find_packages
 
-DkAppVer = '0.1.0'
+DkAppVer = '0.1.1'
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="dknovautils",
     version=DkAppVer,
```

