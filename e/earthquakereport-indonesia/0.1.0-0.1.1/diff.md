# Comparing `tmp/earthquakereport-indonesia-0.1.0.tar.gz` & `tmp/earthquakereport-indonesia-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "earthquakereport-indonesia-0.1.0.tar", last modified: Wed May  3 23:11:26 2023, max compression
+gzip compressed data, was "earthquakereport-indonesia-0.1.1.tar", last modified: Thu May  4 09:07:49 2023, max compression
```

## Comparing `earthquakereport-indonesia-0.1.0.tar` & `earthquakereport-indonesia-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 hasanrachmatullah   (501) staff       (20)        0 2023-05-03 23:11:26.172632 earthquakereport-indonesia-0.1.0/
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)    35149 2023-05-03 08:59:37.000000 earthquakereport-indonesia-0.1.0/LICENSE
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)     1020 2023-05-03 23:11:26.172189 earthquakereport-indonesia-0.1.0/PKG-INFO
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)      383 2023-05-03 22:48:28.000000 earthquakereport-indonesia-0.1.0/README.md
-drwxr-xr-x   0 hasanrachmatullah   (501) staff       (20)        0 2023-05-03 23:11:26.170418 earthquakereport-indonesia-0.1.0/earthquakereport_indonesia.egg-info/
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)     1020 2023-05-03 23:11:26.000000 earthquakereport-indonesia-0.1.0/earthquakereport_indonesia.egg-info/PKG-INFO
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)      250 2023-05-03 23:11:26.000000 earthquakereport-indonesia-0.1.0/earthquakereport_indonesia.egg-info/SOURCES.txt
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)        1 2023-05-03 23:11:26.000000 earthquakereport-indonesia-0.1.0/earthquakereport_indonesia.egg-info/dependency_links.txt
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)       12 2023-05-03 23:11:26.000000 earthquakereport-indonesia-0.1.0/earthquakereport_indonesia.egg-info/top_level.txt
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)       38 2023-05-03 23:11:26.172740 earthquakereport-indonesia-0.1.0/setup.cfg
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)     1018 2023-05-03 22:54:13.000000 earthquakereport-indonesia-0.1.0/setup.py
-drwxr-xr-x   0 hasanrachmatullah   (501) staff       (20)        0 2023-05-03 23:11:26.171197 earthquakereport-indonesia-0.1.0/updateGempa/
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)     2392 2023-05-03 23:03:44.000000 earthquakereport-indonesia-0.1.0/updateGempa/__init__.py
+drwxr-xr-x   0 hasanrachmatullah   (501) staff       (20)        0 2023-05-04 09:07:49.335781 earthquakereport-indonesia-0.1.1/
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)    35149 2023-05-03 08:59:37.000000 earthquakereport-indonesia-0.1.1/LICENSE
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)     1041 2023-05-04 09:07:49.335376 earthquakereport-indonesia-0.1.1/PKG-INFO
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)      404 2023-05-04 08:02:37.000000 earthquakereport-indonesia-0.1.1/README.md
+drwxr-xr-x   0 hasanrachmatullah   (501) staff       (20)        0 2023-05-04 09:07:49.334027 earthquakereport-indonesia-0.1.1/earthquakereport_indonesia.egg-info/
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)     1041 2023-05-04 09:07:49.000000 earthquakereport-indonesia-0.1.1/earthquakereport_indonesia.egg-info/PKG-INFO
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)      250 2023-05-04 09:07:49.000000 earthquakereport-indonesia-0.1.1/earthquakereport_indonesia.egg-info/SOURCES.txt
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)        1 2023-05-04 09:07:49.000000 earthquakereport-indonesia-0.1.1/earthquakereport_indonesia.egg-info/dependency_links.txt
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)       12 2023-05-04 09:07:49.000000 earthquakereport-indonesia-0.1.1/earthquakereport_indonesia.egg-info/top_level.txt
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)       38 2023-05-04 09:07:49.335958 earthquakereport-indonesia-0.1.1/setup.cfg
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)     1018 2023-05-04 08:19:19.000000 earthquakereport-indonesia-0.1.1/setup.py
+drwxr-xr-x   0 hasanrachmatullah   (501) staff       (20)        0 2023-05-04 09:07:49.334383 earthquakereport-indonesia-0.1.1/updateGempa/
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)     2392 2023-05-03 23:03:44.000000 earthquakereport-indonesia-0.1.1/updateGempa/__init__.py
```

### Comparing `earthquakereport-indonesia-0.1.0/LICENSE` & `earthquakereport-indonesia-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `earthquakereport-indonesia-0.1.0/PKG-INFO` & `earthquakereport-indonesia-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthquakereport-indonesia
-Version: 0.1.0
+Version: 0.1.1
 Summary: This package will provide the most update of Indonesian bureau of Forecast (BMKG)
 Home-page: https://github.com/ganirh0612/indonesiaEarthquakeReport
 Author: Hasan Gani
 Author-email: ganirh0612@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -16,7 +16,10 @@
 # Indonesia Earthquake Report
 This package will provide the most update of Indonesian bureau of Forecast (BMKG)
 
 ## How It Work?
 This package will scrape from [BMKG](https://www.bmkg.go.id) to get the latest earthquake reports in Indonesia.
 
 This package will use BeautifulSoup4 and Request, to then produce in the form of JSON that is ready to be used in web or mobile applications.
+
+# Author
+Hasan Gani
```

### Comparing `earthquakereport-indonesia-0.1.0/earthquakereport_indonesia.egg-info/PKG-INFO` & `earthquakereport-indonesia-0.1.1/earthquakereport_indonesia.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthquakereport-indonesia
-Version: 0.1.0
+Version: 0.1.1
 Summary: This package will provide the most update of Indonesian bureau of Forecast (BMKG)
 Home-page: https://github.com/ganirh0612/indonesiaEarthquakeReport
 Author: Hasan Gani
 Author-email: ganirh0612@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -16,7 +16,10 @@
 # Indonesia Earthquake Report
 This package will provide the most update of Indonesian bureau of Forecast (BMKG)
 
 ## How It Work?
 This package will scrape from [BMKG](https://www.bmkg.go.id) to get the latest earthquake reports in Indonesia.
 
 This package will use BeautifulSoup4 and Request, to then produce in the form of JSON that is ready to be used in web or mobile applications.
+
+# Author
+Hasan Gani
```

### Comparing `earthquakereport-indonesia-0.1.0/setup.py` & `earthquakereport-indonesia-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="earthquakereport-indonesia",
-    version="0.1.0",
+    version="0.1.1",
     author="Hasan Gani",
     author_email="ganirh0612@gmail.com",
     description="This package will provide the most update of Indonesian bureau of Forecast (BMKG)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ganirh0612/indonesiaEarthquakeReport",
     project_urls={
```

### Comparing `earthquakereport-indonesia-0.1.0/updateGempa/__init__.py` & `earthquakereport-indonesia-0.1.1/updateGempa/__init__.py`

 * *Files identical despite different names*

