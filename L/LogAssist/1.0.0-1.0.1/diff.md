# Comparing `tmp/LogAssist-1.0.0.tar.gz` & `tmp/LogAssist-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LogAssist-1.0.0.tar", last modified: Thu May  4 02:39:01 2023, max compression
+gzip compressed data, was "LogAssist-1.0.1.tar", last modified: Thu May  4 06:26:09 2023, max compression
```

## Comparing `LogAssist-1.0.0.tar` & `LogAssist-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 02:39:01.514789 LogAssist-1.0.0/
--rw-rw-rw-   0        0        0     1087 2023-05-04 01:09:05.000000 LogAssist-1.0.0/LICENSE
-drwxrwxrwx   0        0        0        0 2023-05-04 02:39:01.500539 LogAssist-1.0.0/LogAssist/
--rw-rw-rw-   0        0        0       23 2023-05-04 02:24:43.000000 LogAssist-1.0.0/LogAssist/__init__.py
--rw-rw-rw-   0        0        0     6416 2023-05-04 01:24:46.000000 LogAssist-1.0.0/LogAssist/log.py
-drwxrwxrwx   0        0        0        0 2023-05-04 02:39:01.509950 LogAssist-1.0.0/LogAssist.egg-info/
--rw-rw-rw-   0        0        0     2263 2023-05-04 02:39:01.000000 LogAssist-1.0.0/LogAssist.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2023-05-04 02:39:01.000000 LogAssist-1.0.0/LogAssist.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 02:39:01.000000 LogAssist-1.0.0/LogAssist.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-04 02:39:01.000000 LogAssist-1.0.0/LogAssist.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2263 2023-05-04 02:39:01.513687 LogAssist-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1645 2023-05-04 02:20:09.000000 LogAssist-1.0.0/README.md
--rw-rw-rw-   0        0        0      620 2023-05-04 02:28:46.000000 LogAssist-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-04 02:39:01.514789 LogAssist-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      874 2023-05-04 02:21:00.000000 LogAssist-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:26:09.866265 LogAssist-1.0.1/
+-rw-rw-rw-   0        0        0     1087 2023-05-04 01:09:05.000000 LogAssist-1.0.1/LICENSE
+drwxrwxrwx   0        0        0        0 2023-05-04 06:26:09.855616 LogAssist-1.0.1/LogAssist/
+-rw-rw-rw-   0        0        0       23 2023-05-04 06:26:01.000000 LogAssist-1.0.1/LogAssist/__init__.py
+-rw-rw-rw-   0        0        0     6416 2023-05-04 01:24:46.000000 LogAssist-1.0.1/LogAssist/log.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:26:09.863754 LogAssist-1.0.1/LogAssist.egg-info/
+-rw-rw-rw-   0        0        0     2353 2023-05-04 06:26:09.000000 LogAssist-1.0.1/LogAssist.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2023-05-04 06:26:09.000000 LogAssist-1.0.1/LogAssist.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 06:26:09.000000 LogAssist-1.0.1/LogAssist.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-04 06:26:09.000000 LogAssist-1.0.1/LogAssist.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2353 2023-05-04 06:26:09.866265 LogAssist-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1668 2023-05-04 02:43:50.000000 LogAssist-1.0.1/README.md
+-rw-rw-rw-   0        0        0      709 2023-05-04 06:25:50.000000 LogAssist-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-04 06:26:09.866265 LogAssist-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      874 2023-05-04 06:25:56.000000 LogAssist-1.0.1/setup.py
```

### Comparing `LogAssist-1.0.0/LICENSE` & `LogAssist-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `LogAssist-1.0.0/LogAssist/log.py` & `LogAssist-1.0.1/LogAssist/log.py`

 * *Files identical despite different names*

### Comparing `LogAssist-1.0.0/LogAssist.egg-info/PKG-INFO` & `LogAssist-1.0.1/LogAssist.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 Metadata-Version: 2.1
 Name: LogAssist
-Version: 1.0.0
+Version: 1.0.1
 Summary: A simple and customizable logging library for Python.
 Home-page: https://github.com/horrible-gh/LogAssist.git
 Author: horrible-gh
 Author-email: horrible <shinjpn1@gmail.com>
 Project-URL: Homepage, https://github.com/horrible-gh/Logger
 Project-URL: Bug Tracker, https://github.com/horrible-gh/Logger/issues
+Keywords: LogAssist,Log Assist,logassist,log assist,Logger,logger
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # LogAssist
 
 A simple and customizable logging library for Python.
 
 ## Installation
 
-Preparing for pypi
+```powershell
+pip install LogAssist
+```
 
 ## Features
 
 - Easy to use and configure
 - Supports multiple log levels (debug, info, warning, error)
 - Outputs log messages to both console and file
 - Allows for log file removal on initialization
```

### Comparing `LogAssist-1.0.0/PKG-INFO` & `LogAssist-1.0.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 Metadata-Version: 2.1
 Name: LogAssist
-Version: 1.0.0
+Version: 1.0.1
 Summary: A simple and customizable logging library for Python.
 Home-page: https://github.com/horrible-gh/LogAssist.git
 Author: horrible-gh
 Author-email: horrible <shinjpn1@gmail.com>
 Project-URL: Homepage, https://github.com/horrible-gh/Logger
 Project-URL: Bug Tracker, https://github.com/horrible-gh/Logger/issues
+Keywords: LogAssist,Log Assist,logassist,log assist,Logger,logger
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # LogAssist
 
 A simple and customizable logging library for Python.
 
 ## Installation
 
-Preparing for pypi
+```powershell
+pip install LogAssist
+```
 
 ## Features
 
 - Easy to use and configure
 - Supports multiple log levels (debug, info, warning, error)
 - Outputs log messages to both console and file
 - Allows for log file removal on initialization
```

### Comparing `LogAssist-1.0.0/README.md` & `LogAssist-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # LogAssist
 
 A simple and customizable logging library for Python.
 
 ## Installation
 
-Preparing for pypi
+```powershell
+pip install LogAssist
+```
 
 ## Features
 
 - Easy to use and configure
 - Supports multiple log levels (debug, info, warning, error)
 - Outputs log messages to both console and file
 - Allows for log file removal on initialization
```

### Comparing `LogAssist-1.0.0/pyproject.toml` & `LogAssist-1.0.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "LogAssist"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="horrible", email="shinjpn1@gmail.com" },
 ]
 description = "A simple and customizable logging library for Python."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+keywords=['LogAssist', 'Log Assist', 'logassist', 'log assist',  'Logger',  'logger']
+
 
 [project.urls]
 "Homepage" = "https://github.com/horrible-gh/Logger"
 "Bug Tracker" = "https://github.com/horrible-gh/Logger/issues"
```

### Comparing `LogAssist-1.0.0/setup.py` & `LogAssist-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='LogAssist',
-    version='1.0.0',
+    version='1.0.1',
     description='LogAssist package',
     author='horrible-gh',
     author_email='shinjpn1@gmail.com',
     url='https://github.com/horrible-gh/LogAssist.git',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
```

