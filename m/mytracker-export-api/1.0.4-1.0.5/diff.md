# Comparing `tmp/mytracker_export_api-1.0.4.tar.gz` & `tmp/mytracker_export_api-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mytracker_export_api-1.0.4.tar", last modified: Thu May  4 13:26:51 2023, max compression
+gzip compressed data, was "mytracker_export_api-1.0.5.tar", last modified: Thu May  4 15:34:56 2023, max compression
```

## Comparing `mytracker_export_api-1.0.4.tar` & `mytracker_export_api-1.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 a.novopolsky   (503) staff       (20)        0 2023-05-04 13:26:51.961665 mytracker_export_api-1.0.4/
--rw-r--r--   0 a.novopolsky   (503) staff       (20)     1835 2022-06-29 14:57:53.000000 mytracker_export_api-1.0.4/.gitignore
--rw-r--r--   0 a.novopolsky   (503) staff       (20)     1063 2022-06-29 14:57:53.000000 mytracker_export_api-1.0.4/LICENSE
--rw-r--r--   0 a.novopolsky   (503) staff       (20)     1341 2023-05-04 13:26:51.961084 mytracker_export_api-1.0.4/PKG-INFO
--rw-r--r--   0 a.novopolsky   (503) staff       (20)      857 2022-07-01 13:49:40.000000 mytracker_export_api-1.0.4/README.md
-drwxr-xr-x   0 a.novopolsky   (503) staff       (20)        0 2023-05-04 13:26:51.951412 mytracker_export_api-1.0.4/examples/
--rw-r--r--   0 a.novopolsky   (503) staff       (20)     6778 2022-07-01 11:29:52.000000 mytracker_export_api-1.0.4/examples/raw_data.ipynb
--rw-r--r--   0 a.novopolsky   (503) staff       (20)     5503 2023-04-26 15:54:56.000000 mytracker_export_api-1.0.4/examples/report.ipynb
--rw-r--r--   0 a.novopolsky   (503) staff       (20)     1863 2022-06-29 15:28:06.000000 mytracker_export_api-1.0.4/examples/segment.ipynb
-drwxr-xr-x   0 a.novopolsky   (503) staff       (20)        0 2023-05-04 13:26:51.954400 mytracker_export_api-1.0.4/mytracker_export_api/
--rw-r--r--   0 a.novopolsky   (503) staff       (20)       72 2022-06-29 14:57:53.000000 mytracker_export_api-1.0.4/mytracker_export_api/__init__.py
--rw-r--r--   0 a.novopolsky   (503) staff       (20)       42 2022-06-29 14:57:53.000000 mytracker_export_api-1.0.4/mytracker_export_api/exceptions.py
--rw-r--r--   0 a.novopolsky   (503) staff       (20)    15826 2023-05-04 13:16:12.000000 mytracker_export_api-1.0.4/mytracker_export_api/mytracker.py
-drwxr-xr-x   0 a.novopolsky   (503) staff       (20)        0 2023-05-04 13:26:51.960313 mytracker_export_api-1.0.4/mytracker_export_api.egg-info/
--rw-r--r--   0 a.novopolsky   (503) staff       (20)     1341 2023-05-04 13:26:51.000000 mytracker_export_api-1.0.4/mytracker_export_api.egg-info/PKG-INFO
--rw-r--r--   0 a.novopolsky   (503) staff       (20)      487 2023-05-04 13:26:51.000000 mytracker_export_api-1.0.4/mytracker_export_api.egg-info/SOURCES.txt
--rw-r--r--   0 a.novopolsky   (503) staff       (20)        1 2023-05-04 13:26:51.000000 mytracker_export_api-1.0.4/mytracker_export_api.egg-info/dependency_links.txt
--rw-r--r--   0 a.novopolsky   (503) staff       (20)        1 2023-05-04 13:26:51.000000 mytracker_export_api-1.0.4/mytracker_export_api.egg-info/not-zip-safe
--rw-r--r--   0 a.novopolsky   (503) staff       (20)       47 2023-05-04 13:26:51.000000 mytracker_export_api-1.0.4/mytracker_export_api.egg-info/requires.txt
--rw-r--r--   0 a.novopolsky   (503) staff       (20)       21 2023-05-04 13:26:51.000000 mytracker_export_api-1.0.4/mytracker_export_api.egg-info/top_level.txt
--rw-r--r--   0 a.novopolsky   (503) staff       (20)       47 2023-05-04 12:53:06.000000 mytracker_export_api-1.0.4/requirements.txt
--rw-r--r--   0 a.novopolsky   (503) staff       (20)       38 2023-05-04 13:26:51.961943 mytracker_export_api-1.0.4/setup.cfg
--rw-r--r--   0 a.novopolsky   (503) staff       (20)      703 2023-05-04 13:26:22.000000 mytracker_export_api-1.0.4/setup.py
+drwxr-xr-x   0 a.novopolsky   (503) staff       (20)        0 2023-05-04 15:34:56.767727 mytracker_export_api-1.0.5/
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)     1835 2022-06-29 14:57:53.000000 mytracker_export_api-1.0.5/.gitignore
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)     1063 2022-06-29 14:57:53.000000 mytracker_export_api-1.0.5/LICENSE
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)     1341 2023-05-04 15:34:56.767152 mytracker_export_api-1.0.5/PKG-INFO
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)      857 2022-07-01 13:49:40.000000 mytracker_export_api-1.0.5/README.md
+drwxr-xr-x   0 a.novopolsky   (503) staff       (20)        0 2023-05-04 15:34:56.751537 mytracker_export_api-1.0.5/examples/
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)     6778 2022-07-01 11:29:52.000000 mytracker_export_api-1.0.5/examples/raw_data.ipynb
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)     5503 2023-04-26 15:54:56.000000 mytracker_export_api-1.0.5/examples/report.ipynb
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)     1863 2022-06-29 15:28:06.000000 mytracker_export_api-1.0.5/examples/segment.ipynb
+drwxr-xr-x   0 a.novopolsky   (503) staff       (20)        0 2023-05-04 15:34:56.756768 mytracker_export_api-1.0.5/mytracker_export_api/
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)       72 2022-06-29 14:57:53.000000 mytracker_export_api-1.0.5/mytracker_export_api/__init__.py
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)       42 2022-06-29 14:57:53.000000 mytracker_export_api-1.0.5/mytracker_export_api/exceptions.py
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)    15826 2023-05-04 14:53:24.000000 mytracker_export_api-1.0.5/mytracker_export_api/mytracker.py
+drwxr-xr-x   0 a.novopolsky   (503) staff       (20)        0 2023-05-04 15:34:56.766245 mytracker_export_api-1.0.5/mytracker_export_api.egg-info/
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)     1341 2023-05-04 15:34:56.000000 mytracker_export_api-1.0.5/mytracker_export_api.egg-info/PKG-INFO
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)      487 2023-05-04 15:34:56.000000 mytracker_export_api-1.0.5/mytracker_export_api.egg-info/SOURCES.txt
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)        1 2023-05-04 15:34:56.000000 mytracker_export_api-1.0.5/mytracker_export_api.egg-info/dependency_links.txt
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)        1 2023-05-04 15:34:56.000000 mytracker_export_api-1.0.5/mytracker_export_api.egg-info/not-zip-safe
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)       50 2023-05-04 15:34:56.000000 mytracker_export_api-1.0.5/mytracker_export_api.egg-info/requires.txt
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)       21 2023-05-04 15:34:56.000000 mytracker_export_api-1.0.5/mytracker_export_api.egg-info/top_level.txt
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)       50 2023-05-04 15:34:30.000000 mytracker_export_api-1.0.5/requirements.txt
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)       38 2023-05-04 15:34:56.767927 mytracker_export_api-1.0.5/setup.cfg
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)      703 2023-05-04 15:34:23.000000 mytracker_export_api-1.0.5/setup.py
```

### Comparing `mytracker_export_api-1.0.4/.gitignore` & `mytracker_export_api-1.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `mytracker_export_api-1.0.4/LICENSE` & `mytracker_export_api-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mytracker_export_api-1.0.4/PKG-INFO` & `mytracker_export_api-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mytracker_export_api
-Version: 1.0.4
+Version: 1.0.5
 Summary: Python wrapper for MyTracker Export API.
 Home-page: UNKNOWN
 Author: Artyom Novopolsky
 Author-email: a.novopolsky@corp.mail.ru
 License: UNKNOWN
 Project-URL: Documentation, https://tracker.my.com/docs/api/export-api/about
 Project-URL: Source, https://github.com/tracker-my-com/mytracker-export-api-python
```

### Comparing `mytracker_export_api-1.0.4/README.md` & `mytracker_export_api-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `mytracker_export_api-1.0.4/examples/raw_data.ipynb` & `mytracker_export_api-1.0.5/examples/raw_data.ipynb`

 * *Files identical despite different names*

### Comparing `mytracker_export_api-1.0.4/examples/report.ipynb` & `mytracker_export_api-1.0.5/examples/report.ipynb`

 * *Files identical despite different names*

### Comparing `mytracker_export_api-1.0.4/examples/segment.ipynb` & `mytracker_export_api-1.0.5/examples/segment.ipynb`

 * *Files identical despite different names*

### Comparing `mytracker_export_api-1.0.4/mytracker_export_api/mytracker.py` & `mytracker_export_api-1.0.5/mytracker_export_api/mytracker.py`

 * *Files identical despite different names*

### Comparing `mytracker_export_api-1.0.4/mytracker_export_api.egg-info/PKG-INFO` & `mytracker_export_api-1.0.5/mytracker_export_api.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mytracker-export-api
-Version: 1.0.4
+Version: 1.0.5
 Summary: Python wrapper for MyTracker Export API.
 Home-page: UNKNOWN
 Author: Artyom Novopolsky
 Author-email: a.novopolsky@corp.mail.ru
 License: UNKNOWN
 Project-URL: Documentation, https://tracker.my.com/docs/api/export-api/about
 Project-URL: Source, https://github.com/tracker-my-com/mytracker-export-api-python
```

### Comparing `mytracker_export_api-1.0.4/setup.py` & `mytracker_export_api-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='mytracker_export_api',
-    version='1.0.4',
+    version='1.0.5',
     description='Python wrapper for MyTracker Export API.',
     packages=['mytracker_export_api'],
     author='Artyom Novopolsky',
     author_email='a.novopolsky@corp.mail.ru',
     install_requires=open('requirements.txt').read().splitlines(),
     python_requires='>=3.6.1',
     long_description=open('README.md').read(),
```

