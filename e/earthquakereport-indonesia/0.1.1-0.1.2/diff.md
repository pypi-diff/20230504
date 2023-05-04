# Comparing `tmp/earthquakereport-indonesia-0.1.1.tar.gz` & `tmp/earthquakereport-indonesia-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "earthquakereport-indonesia-0.1.1.tar", last modified: Thu May  4 09:07:49 2023, max compression
+gzip compressed data, was "earthquakereport-indonesia-0.1.2.tar", last modified: Thu May  4 09:26:12 2023, max compression
```

## Comparing `earthquakereport-indonesia-0.1.1.tar` & `earthquakereport-indonesia-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 hasanrachmatullah   (501) staff       (20)        0 2023-05-04 09:07:49.335781 earthquakereport-indonesia-0.1.1/
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)    35149 2023-05-03 08:59:37.000000 earthquakereport-indonesia-0.1.1/LICENSE
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)     1041 2023-05-04 09:07:49.335376 earthquakereport-indonesia-0.1.1/PKG-INFO
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)      404 2023-05-04 08:02:37.000000 earthquakereport-indonesia-0.1.1/README.md
-drwxr-xr-x   0 hasanrachmatullah   (501) staff       (20)        0 2023-05-04 09:07:49.334027 earthquakereport-indonesia-0.1.1/earthquakereport_indonesia.egg-info/
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)     1041 2023-05-04 09:07:49.000000 earthquakereport-indonesia-0.1.1/earthquakereport_indonesia.egg-info/PKG-INFO
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)      250 2023-05-04 09:07:49.000000 earthquakereport-indonesia-0.1.1/earthquakereport_indonesia.egg-info/SOURCES.txt
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)        1 2023-05-04 09:07:49.000000 earthquakereport-indonesia-0.1.1/earthquakereport_indonesia.egg-info/dependency_links.txt
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)       12 2023-05-04 09:07:49.000000 earthquakereport-indonesia-0.1.1/earthquakereport_indonesia.egg-info/top_level.txt
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)       38 2023-05-04 09:07:49.335958 earthquakereport-indonesia-0.1.1/setup.cfg
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)     1018 2023-05-04 08:19:19.000000 earthquakereport-indonesia-0.1.1/setup.py
-drwxr-xr-x   0 hasanrachmatullah   (501) staff       (20)        0 2023-05-04 09:07:49.334383 earthquakereport-indonesia-0.1.1/updateGempa/
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)     2392 2023-05-03 23:03:44.000000 earthquakereport-indonesia-0.1.1/updateGempa/__init__.py
+drwxr-xr-x   0 hasanrachmatullah   (501) staff       (20)        0 2023-05-04 09:26:12.165985 earthquakereport-indonesia-0.1.2/
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)    35149 2023-05-04 09:21:22.000000 earthquakereport-indonesia-0.1.2/LICENSE
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)     1233 2023-05-04 09:26:12.165684 earthquakereport-indonesia-0.1.2/PKG-INFO
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)      596 2023-05-04 09:24:44.000000 earthquakereport-indonesia-0.1.2/README.md
+drwxr-xr-x   0 hasanrachmatullah   (501) staff       (20)        0 2023-05-04 09:26:12.164465 earthquakereport-indonesia-0.1.2/earthquakereport_indonesia.egg-info/
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)     1233 2023-05-04 09:26:12.000000 earthquakereport-indonesia-0.1.2/earthquakereport_indonesia.egg-info/PKG-INFO
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)      250 2023-05-04 09:26:12.000000 earthquakereport-indonesia-0.1.2/earthquakereport_indonesia.egg-info/SOURCES.txt
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)        1 2023-05-04 09:26:12.000000 earthquakereport-indonesia-0.1.2/earthquakereport_indonesia.egg-info/dependency_links.txt
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)       12 2023-05-04 09:26:12.000000 earthquakereport-indonesia-0.1.2/earthquakereport_indonesia.egg-info/top_level.txt
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)       38 2023-05-04 09:26:12.166107 earthquakereport-indonesia-0.1.2/setup.cfg
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)     1018 2023-05-04 09:25:39.000000 earthquakereport-indonesia-0.1.2/setup.py
+drwxr-xr-x   0 hasanrachmatullah   (501) staff       (20)        0 2023-05-04 09:26:12.164967 earthquakereport-indonesia-0.1.2/updateGempa/
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)     2392 2023-05-04 09:21:22.000000 earthquakereport-indonesia-0.1.2/updateGempa/__init__.py
```

### Comparing `earthquakereport-indonesia-0.1.1/LICENSE` & `earthquakereport-indonesia-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `earthquakereport-indonesia-0.1.1/setup.py` & `earthquakereport-indonesia-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="earthquakereport-indonesia",
-    version="0.1.1",
+    version="0.1.2",
     author="Hasan Gani",
     author_email="ganirh0612@gmail.com",
     description="This package will provide the most update of Indonesian bureau of Forecast (BMKG)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ganirh0612/indonesiaEarthquakeReport",
     project_urls={
```

### Comparing `earthquakereport-indonesia-0.1.1/updateGempa/__init__.py` & `earthquakereport-indonesia-0.1.2/updateGempa/__init__.py`

 * *Files identical despite different names*

