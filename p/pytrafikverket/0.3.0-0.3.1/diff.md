# Comparing `tmp/pytrafikverket-0.3.0.tar.gz` & `tmp/pytrafikverket-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytrafikverket-0.3.0.tar", last modified: Wed May  3 20:20:24 2023, max compression
+gzip compressed data, was "pytrafikverket-0.3.1.tar", last modified: Thu May  4 16:19:48 2023, max compression
```

## Comparing `pytrafikverket-0.3.0.tar` & `pytrafikverket-0.3.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 gjo       (1000) gjo       (1000)        0 2023-05-03 20:20:24.230394 pytrafikverket-0.3.0/
--rw-r--r--   0 gjo       (1000) gjo       (1000)     1072 2023-04-07 12:58:54.000000 pytrafikverket-0.3.0/LICENSE
--rw-r--r--   0 gjo       (1000) gjo       (1000)     2675 2023-05-03 20:20:24.230394 pytrafikverket-0.3.0/PKG-INFO
--rw-r--r--   0 gjo       (1000) gjo       (1000)     2138 2023-05-03 19:02:53.000000 pytrafikverket-0.3.0/README.md
-drwxr-xr-x   0 gjo       (1000) gjo       (1000)        0 2023-05-03 20:20:24.230394 pytrafikverket-0.3.0/pytrafikverket/
--rw-r--r--   0 gjo       (1000) gjo       (1000)      632 2023-04-07 12:58:54.000000 pytrafikverket-0.3.0/pytrafikverket/__init__.py
--rw-r--r--   0 gjo       (1000) gjo       (1000)     6478 2023-05-03 18:52:58.000000 pytrafikverket-0.3.0/pytrafikverket/__main__.py
--rw-r--r--   0 gjo       (1000) gjo       (1000)     1327 2023-05-03 20:18:05.000000 pytrafikverket-0.3.0/pytrafikverket/exceptions.py
--rw-r--r--   0 gjo       (1000) gjo       (1000)        0 2023-05-03 18:52:58.000000 pytrafikverket-0.3.0/pytrafikverket/py.typed
--rw-r--r--   0 gjo       (1000) gjo       (1000)     8786 2023-05-03 20:18:05.000000 pytrafikverket-0.3.0/pytrafikverket/trafikverket.py
--rw-r--r--   0 gjo       (1000) gjo       (1000)     3717 2023-05-03 19:06:27.000000 pytrafikverket-0.3.0/pytrafikverket/trafikverket_camera.py
--rw-r--r--   0 gjo       (1000) gjo       (1000)     9937 2023-05-03 18:52:58.000000 pytrafikverket-0.3.0/pytrafikverket/trafikverket_ferry.py
--rw-r--r--   0 gjo       (1000) gjo       (1000)    12091 2023-05-03 20:07:04.000000 pytrafikverket-0.3.0/pytrafikverket/trafikverket_train.py
--rw-r--r--   0 gjo       (1000) gjo       (1000)     7315 2023-05-03 20:07:04.000000 pytrafikverket-0.3.0/pytrafikverket/trafikverket_weather.py
-drwxr-xr-x   0 gjo       (1000) gjo       (1000)        0 2023-05-03 20:20:24.230394 pytrafikverket-0.3.0/pytrafikverket.egg-info/
--rw-r--r--   0 gjo       (1000) gjo       (1000)     2675 2023-05-03 20:20:24.000000 pytrafikverket-0.3.0/pytrafikverket.egg-info/PKG-INFO
--rw-r--r--   0 gjo       (1000) gjo       (1000)      547 2023-05-03 20:20:24.000000 pytrafikverket-0.3.0/pytrafikverket.egg-info/SOURCES.txt
--rw-r--r--   0 gjo       (1000) gjo       (1000)        1 2023-05-03 20:20:24.000000 pytrafikverket-0.3.0/pytrafikverket.egg-info/dependency_links.txt
--rw-r--r--   0 gjo       (1000) gjo       (1000)       27 2023-05-03 20:20:24.000000 pytrafikverket-0.3.0/pytrafikverket.egg-info/requires.txt
--rw-r--r--   0 gjo       (1000) gjo       (1000)       15 2023-05-03 20:20:24.000000 pytrafikverket-0.3.0/pytrafikverket.egg-info/top_level.txt
--rw-r--r--   0 gjo       (1000) gjo       (1000)        1 2023-05-03 20:20:24.000000 pytrafikverket-0.3.0/pytrafikverket.egg-info/zip-safe
--rw-r--r--   0 gjo       (1000) gjo       (1000)      170 2023-05-03 20:20:24.230394 pytrafikverket-0.3.0/setup.cfg
--rw-r--r--   0 gjo       (1000) gjo       (1000)     1067 2023-05-03 20:18:05.000000 pytrafikverket-0.3.0/setup.py
+drwxr-xr-x   0 gjo       (1000) gjo       (1000)        0 2023-05-04 16:19:48.750889 pytrafikverket-0.3.1/
+-rw-r--r--   0 gjo       (1000) gjo       (1000)     1072 2023-04-07 12:58:54.000000 pytrafikverket-0.3.1/LICENSE
+-rw-r--r--   0 gjo       (1000) gjo       (1000)     2675 2023-05-04 16:19:48.750889 pytrafikverket-0.3.1/PKG-INFO
+-rw-r--r--   0 gjo       (1000) gjo       (1000)     2138 2023-05-03 19:02:53.000000 pytrafikverket-0.3.1/README.md
+drwxr-xr-x   0 gjo       (1000) gjo       (1000)        0 2023-05-04 16:19:48.740889 pytrafikverket-0.3.1/pytrafikverket/
+-rw-r--r--   0 gjo       (1000) gjo       (1000)      632 2023-04-07 12:58:54.000000 pytrafikverket-0.3.1/pytrafikverket/__init__.py
+-rw-r--r--   0 gjo       (1000) gjo       (1000)     6478 2023-05-03 18:52:58.000000 pytrafikverket-0.3.1/pytrafikverket/__main__.py
+-rw-r--r--   0 gjo       (1000) gjo       (1000)     1327 2023-05-03 20:18:05.000000 pytrafikverket-0.3.1/pytrafikverket/exceptions.py
+-rw-r--r--   0 gjo       (1000) gjo       (1000)        0 2023-05-03 18:52:58.000000 pytrafikverket-0.3.1/pytrafikverket/py.typed
+-rw-r--r--   0 gjo       (1000) gjo       (1000)     8786 2023-05-03 20:18:05.000000 pytrafikverket-0.3.1/pytrafikverket/trafikverket.py
+-rw-r--r--   0 gjo       (1000) gjo       (1000)     3717 2023-05-03 19:06:27.000000 pytrafikverket-0.3.1/pytrafikverket/trafikverket_camera.py
+-rw-r--r--   0 gjo       (1000) gjo       (1000)     9937 2023-05-03 18:52:58.000000 pytrafikverket-0.3.1/pytrafikverket/trafikverket_ferry.py
+-rw-r--r--   0 gjo       (1000) gjo       (1000)    12091 2023-05-03 20:07:04.000000 pytrafikverket-0.3.1/pytrafikverket/trafikverket_train.py
+-rw-r--r--   0 gjo       (1000) gjo       (1000)     7309 2023-05-04 16:19:35.000000 pytrafikverket-0.3.1/pytrafikverket/trafikverket_weather.py
+drwxr-xr-x   0 gjo       (1000) gjo       (1000)        0 2023-05-04 16:19:48.740889 pytrafikverket-0.3.1/pytrafikverket.egg-info/
+-rw-r--r--   0 gjo       (1000) gjo       (1000)     2675 2023-05-04 16:19:48.000000 pytrafikverket-0.3.1/pytrafikverket.egg-info/PKG-INFO
+-rw-r--r--   0 gjo       (1000) gjo       (1000)      547 2023-05-04 16:19:48.000000 pytrafikverket-0.3.1/pytrafikverket.egg-info/SOURCES.txt
+-rw-r--r--   0 gjo       (1000) gjo       (1000)        1 2023-05-04 16:19:48.000000 pytrafikverket-0.3.1/pytrafikverket.egg-info/dependency_links.txt
+-rw-r--r--   0 gjo       (1000) gjo       (1000)       27 2023-05-04 16:19:48.000000 pytrafikverket-0.3.1/pytrafikverket.egg-info/requires.txt
+-rw-r--r--   0 gjo       (1000) gjo       (1000)       15 2023-05-04 16:19:48.000000 pytrafikverket-0.3.1/pytrafikverket.egg-info/top_level.txt
+-rw-r--r--   0 gjo       (1000) gjo       (1000)        1 2023-05-03 20:20:24.000000 pytrafikverket-0.3.1/pytrafikverket.egg-info/zip-safe
+-rw-r--r--   0 gjo       (1000) gjo       (1000)      170 2023-05-04 16:19:48.750889 pytrafikverket-0.3.1/setup.cfg
+-rw-r--r--   0 gjo       (1000) gjo       (1000)     1067 2023-05-04 16:19:35.000000 pytrafikverket-0.3.1/setup.py
```

### Comparing `pytrafikverket-0.3.0/LICENSE` & `pytrafikverket-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytrafikverket-0.3.0/PKG-INFO` & `pytrafikverket-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrafikverket
-Version: 0.3.0
+Version: 0.3.1
 Summary: Retreive values from public API at the Swedish Transport Administration (Trafikverket).
 Home-page: https://github.com/endor-force/pytrafikverket
 Author: Peter Andersson, Jonas Karlsson
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pytrafikverket-0.3.0/README.md` & `pytrafikverket-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pytrafikverket-0.3.0/pytrafikverket/__init__.py` & `pytrafikverket-0.3.1/pytrafikverket/__init__.py`

 * *Files identical despite different names*

### Comparing `pytrafikverket-0.3.0/pytrafikverket/__main__.py` & `pytrafikverket-0.3.1/pytrafikverket/__main__.py`

 * *Files identical despite different names*

### Comparing `pytrafikverket-0.3.0/pytrafikverket/exceptions.py` & `pytrafikverket-0.3.1/pytrafikverket/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytrafikverket-0.3.0/pytrafikverket/trafikverket.py` & `pytrafikverket-0.3.1/pytrafikverket/trafikverket.py`

 * *Files identical despite different names*

### Comparing `pytrafikverket-0.3.0/pytrafikverket/trafikverket_camera.py` & `pytrafikverket-0.3.1/pytrafikverket/trafikverket_camera.py`

 * *Files identical despite different names*

### Comparing `pytrafikverket-0.3.0/pytrafikverket/trafikverket_ferry.py` & `pytrafikverket-0.3.1/pytrafikverket/trafikverket_ferry.py`

 * *Files identical despite different names*

### Comparing `pytrafikverket-0.3.0/pytrafikverket/trafikverket_train.py` & `pytrafikverket-0.3.1/pytrafikverket/trafikverket_train.py`

 * *Files identical despite different names*

### Comparing `pytrafikverket-0.3.0/pytrafikverket/trafikverket_weather.py` & `pytrafikverket-0.3.1/pytrafikverket/trafikverket_weather.py`

 * *Files 5% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         precipitationtype: str | None,
         precipitationtype_translated: str | None,
         winddirection: str | None,
         winddirectiontext: str | None,
         winddirectiontext_translated: str | None,
         windforce: float | None,
         windforcemax: float | None,
-        active: str | None,
+        active: bool,
         measure_time: datetime | None,
         precipitation_amount: float | None,
         precipitation_amountname: str | None,
         precipitation_amountname_translated: str | None,
         modified_time: datetime | None,
     ) -> None:
         """Initialize the class."""
@@ -133,15 +133,15 @@
         winddirectiontext_translated = None
         if winddirectiontext := node_helper.get_text("Measurement/Wind/DirectionText"):
             winddirectiontext_translated = WIND_DIRECTION_TRANSLATION.get(
                 winddirectiontext
             )
         windforce = node_helper.get_number("Measurement/Wind/Force")
         windforcemax = node_helper.get_number("Measurement/Wind/ForceMax")
-        active = node_helper.get_text("Active")
+        active = node_helper.get_bool("Active")
         measure_time = node_helper.get_datetime("Measurement/MeasureTime")
         precipitation_amount = node_helper.get_number(
             "Measurement/Precipitation/Amount"
         )
         precipitation_amountname_translated = None
         if precipitation_amountname := node_helper.get_text(
             "Measurement/Precipitation/AmountName"
```

### Comparing `pytrafikverket-0.3.0/pytrafikverket.egg-info/PKG-INFO` & `pytrafikverket-0.3.1/pytrafikverket.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrafikverket
-Version: 0.3.0
+Version: 0.3.1
 Summary: Retreive values from public API at the Swedish Transport Administration (Trafikverket).
 Home-page: https://github.com/endor-force/pytrafikverket
 Author: Peter Andersson, Jonas Karlsson
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pytrafikverket-0.3.0/pytrafikverket.egg-info/SOURCES.txt` & `pytrafikverket-0.3.1/pytrafikverket.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytrafikverket-0.3.0/setup.py` & `pytrafikverket-0.3.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="UTF-8") as fh:
     long_description = fh.read()
 
 setup(
     name="pytrafikverket",
-    version="0.3.0",
+    version="0.3.1",
     description="Retreive values from public API at the Swedish Transport Administration (Trafikverket).",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/endor-force/pytrafikverket",
     author="Peter Andersson, Jonas Karlsson",
     license="MIT",
     classifiers=[
```

