# Comparing `tmp/PythonAvroSchemas-1.2.0.tar.gz` & `tmp/PythonAvroSchemas-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PythonAvroSchemas-1.2.0.tar", last modified: Sun Feb 12 11:19:42 2023, max compression
+gzip compressed data, was "PythonAvroSchemas-1.3.0.tar", last modified: Thu May  4 17:29:38 2023, max compression
```

## Comparing `PythonAvroSchemas-1.2.0.tar` & `PythonAvroSchemas-1.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-02-12 11:19:42.364091 PythonAvroSchemas-1.2.0/
--rw-rw-rw-   0        0        0     1079 2023-02-07 13:27:13.000000 PythonAvroSchemas-1.2.0/LICENSE.txt
--rw-rw-rw-   0        0        0      903 2023-02-12 11:19:42.365103 PythonAvroSchemas-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-02-07 13:27:13.000000 PythonAvroSchemas-1.2.0/README.md
--rw-rw-rw-   0        0        0      724 2023-02-12 11:19:42.369955 PythonAvroSchemas-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1721 2023-02-12 11:19:27.000000 PythonAvroSchemas-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-12 11:19:42.281087 PythonAvroSchemas-1.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-02-12 11:19:42.347788 PythonAvroSchemas-1.2.0/src/PythonAvroSchemas.egg-info/
--rw-rw-rw-   0        0        0      903 2023-02-12 11:19:42.000000 PythonAvroSchemas-1.2.0/src/PythonAvroSchemas.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2023-02-12 11:19:42.000000 PythonAvroSchemas-1.2.0/src/PythonAvroSchemas.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-12 11:19:42.000000 PythonAvroSchemas-1.2.0/src/PythonAvroSchemas.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-02-12 11:19:42.000000 PythonAvroSchemas-1.2.0/src/PythonAvroSchemas.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-12 11:19:42.361759 PythonAvroSchemas-1.2.0/src/Schemas/
--rw-rw-rw-   0        0        0      168 2023-02-12 11:17:28.000000 PythonAvroSchemas-1.2.0/src/Schemas/HelpEventCreated.py
--rw-rw-rw-   0        0        0       90 2023-02-12 11:17:28.000000 PythonAvroSchemas-1.2.0/src/Schemas/NotificationCreated.py
--rw-rw-rw-   0        0        0       73 2023-02-12 11:17:28.000000 PythonAvroSchemas-1.2.0/src/Schemas/UserCreatedEvent.py
--rw-rw-rw-   0        0        0        0 2023-02-07 13:27:13.000000 PythonAvroSchemas-1.2.0/src/Schemas/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 17:29:38.963829 PythonAvroSchemas-1.3.0/
+-rw-rw-rw-   0        0        0     1079 2023-02-07 13:27:13.000000 PythonAvroSchemas-1.3.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      758 2023-05-04 17:29:38.963829 PythonAvroSchemas-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-02-07 13:27:13.000000 PythonAvroSchemas-1.3.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-04 17:29:38.966152 PythonAvroSchemas-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1721 2023-05-04 17:28:32.000000 PythonAvroSchemas-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 17:29:38.898141 PythonAvroSchemas-1.3.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-04 17:29:38.950899 PythonAvroSchemas-1.3.0/src/PythonAvroSchemas.egg-info/
+-rw-rw-rw-   0        0        0      758 2023-05-04 17:29:38.000000 PythonAvroSchemas-1.3.0/src/PythonAvroSchemas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2023-05-04 17:29:38.000000 PythonAvroSchemas-1.3.0/src/PythonAvroSchemas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 17:29:38.000000 PythonAvroSchemas-1.3.0/src/PythonAvroSchemas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-04 17:29:38.000000 PythonAvroSchemas-1.3.0/src/PythonAvroSchemas.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 17:29:38.961305 PythonAvroSchemas-1.3.0/src/Schemas/
+-rw-rw-rw-   0        0        0      168 2023-05-04 17:27:40.000000 PythonAvroSchemas-1.3.0/src/Schemas/HelpEventCreated.py
+-rw-rw-rw-   0        0        0       90 2023-05-04 17:27:40.000000 PythonAvroSchemas-1.3.0/src/Schemas/NotificationCreated.py
+-rw-rw-rw-   0        0        0       55 2023-05-04 17:27:40.000000 PythonAvroSchemas-1.3.0/src/Schemas/UserCreatedEvent.py
+-rw-rw-rw-   0        0        0        0 2023-02-07 13:27:13.000000 PythonAvroSchemas-1.3.0/src/Schemas/__init__.py
```

### Comparing `PythonAvroSchemas-1.2.0/LICENSE.txt` & `PythonAvroSchemas-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PythonAvroSchemas-1.2.0/PKG-INFO` & `PythonAvroSchemas-1.3.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 Metadata-Version: 2.1
 Name: PythonAvroSchemas
-Version: 1.2.0
+Version: 1.3.0
 Summary: Library containing the python classes that represent avro schemas used in HelpSociety project
 Home-page: https://github.com/StevenSopilidis/PythonAvroSchemas
 Author: Steven Sopilidis
 Author-email: stefanossopilidis2003@gmail.com
 License: MIT
 Download-URL: https://github.com/StevenSopilidis/PythonAvroSchemas/archive/refs/tags/v1.0.0-alpha.tar.gz
-Project-URL: Bug Tracker, https://github.com/StevenSopilidis/PythonAvroSchemas
 Keywords: Avro Schemas
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 UNKNOWN
```

### Comparing `PythonAvroSchemas-1.2.0/setup.py` & `PythonAvroSchemas-1.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 from distutils.core import setup
 
 import setuptools
 setup(
   name = 'PythonAvroSchemas',         # How you named your package folder (MyLib)
   # packages = ['PythonAvroSchemas'],   # Chose the same as "name"
-  version = '1.2.0',      # Start with a small number and increase it with every change you make
+  version = '1.3.0',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Library containing the python classes that represent avro schemas used in HelpSociety project',   # Give a short description about your library
   author = 'Steven Sopilidis',                   # Type in your name
   author_email = 'stefanossopilidis2003@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/StevenSopilidis/PythonAvroSchemas',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/StevenSopilidis/PythonAvroSchemas/archive/refs/tags/v1.0.0-alpha.tar.gz',    # I explain this later on
   keywords = ['Avro Schemas'],   # Keywords that define your package best
```

### Comparing `PythonAvroSchemas-1.2.0/src/PythonAvroSchemas.egg-info/PKG-INFO` & `PythonAvroSchemas-1.3.0/src/PythonAvroSchemas.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 Metadata-Version: 2.1
 Name: PythonAvroSchemas
-Version: 1.2.0
+Version: 1.3.0
 Summary: Library containing the python classes that represent avro schemas used in HelpSociety project
 Home-page: https://github.com/StevenSopilidis/PythonAvroSchemas
 Author: Steven Sopilidis
 Author-email: stefanossopilidis2003@gmail.com
 License: MIT
 Download-URL: https://github.com/StevenSopilidis/PythonAvroSchemas/archive/refs/tags/v1.0.0-alpha.tar.gz
-Project-URL: Bug Tracker, https://github.com/StevenSopilidis/PythonAvroSchemas
 Keywords: Avro Schemas
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 UNKNOWN
```

