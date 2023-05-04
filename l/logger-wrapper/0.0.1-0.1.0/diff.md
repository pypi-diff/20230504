# Comparing `tmp/logger_wrapper-0.0.1.tar.gz` & `tmp/logger_wrapper-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logger_wrapper-0.0.1.tar", last modified: Mon Apr  3 11:20:45 2023, max compression
+gzip compressed data, was "logger_wrapper-0.1.0.tar", last modified: Thu May  4 08:13:38 2023, max compression
```

## Comparing `logger_wrapper-0.0.1.tar` & `logger_wrapper-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 erol      (1000) erol      (1000)        0 2023-04-03 11:20:45.378496 logger_wrapper-0.0.1/
--rw-rw-r--   0 erol      (1000) erol      (1000)     2401 2023-04-03 11:20:45.378496 logger_wrapper-0.0.1/PKG-INFO
--rw-rw-r--   0 erol      (1000) erol      (1000)     1498 2023-04-03 11:11:04.000000 logger_wrapper-0.0.1/README.md
--rw-r--r--   0 erol      (1000) erol      (1000)      904 2023-04-03 11:10:18.000000 logger_wrapper-0.0.1/pyproject.toml
--rw-r--r--   0 erol      (1000) erol      (1000)      194 2023-04-03 11:20:45.382495 logger_wrapper-0.0.1/setup.cfg
--rw-r--r--   0 erol      (1000) erol      (1000)      253 2023-04-03 11:12:13.000000 logger_wrapper-0.0.1/setup.py
-drwxrwxr-x   0 erol      (1000) erol      (1000)        0 2023-04-03 11:20:45.378496 logger_wrapper-0.0.1/src/
-drwxrwxr-x   0 erol      (1000) erol      (1000)        0 2023-04-03 11:20:45.378496 logger_wrapper-0.0.1/src/logger_wrapper/
--rw-r--r--   0 erol      (1000) erol      (1000)     1424 2023-04-03 11:04:33.000000 logger_wrapper-0.0.1/src/logger_wrapper/__init__.py
--rw-r--r--   0 erol      (1000) erol      (1000)     9058 2023-04-03 11:07:26.000000 logger_wrapper-0.0.1/src/logger_wrapper/logger_wrapper.py
-drwxrwxr-x   0 erol      (1000) erol      (1000)        0 2023-04-03 11:20:45.378496 logger_wrapper-0.0.1/src/logger_wrapper.egg-info/
--rw-rw-r--   0 erol      (1000) erol      (1000)     2401 2023-04-03 11:20:45.000000 logger_wrapper-0.0.1/src/logger_wrapper.egg-info/PKG-INFO
--rw-rw-r--   0 erol      (1000) erol      (1000)      308 2023-04-03 11:20:45.000000 logger_wrapper-0.0.1/src/logger_wrapper.egg-info/SOURCES.txt
--rw-rw-r--   0 erol      (1000) erol      (1000)        1 2023-04-03 11:20:45.000000 logger_wrapper-0.0.1/src/logger_wrapper.egg-info/dependency_links.txt
--rw-rw-r--   0 erol      (1000) erol      (1000)       15 2023-04-03 11:20:45.000000 logger_wrapper-0.0.1/src/logger_wrapper.egg-info/top_level.txt
-drwxrwxr-x   0 erol      (1000) erol      (1000)        0 2023-04-03 11:20:45.378496 logger_wrapper-0.0.1/tests/
--rw-r--r--   0 erol      (1000) erol      (1000)     3554 2023-04-03 11:08:38.000000 logger_wrapper-0.0.1/tests/test_logger_wrapper.py
+drwxrwxr-x   0 erol      (1000) erol      (1000)        0 2023-05-04 08:13:38.474964 logger_wrapper-0.1.0/
+-rw-rw-r--   0 erol      (1000) erol      (1000)     8900 2023-05-04 08:13:38.474964 logger_wrapper-0.1.0/PKG-INFO
+-rw-rw-r--   0 erol      (1000) erol      (1000)     8012 2023-05-04 07:07:41.000000 logger_wrapper-0.1.0/README.md
+-rw-rw-r--   0 erol      (1000) erol      (1000)      894 2023-05-04 06:34:44.000000 logger_wrapper-0.1.0/pyproject.toml
+-rw-r--r--   0 erol      (1000) erol      (1000)      194 2023-05-04 08:13:38.474964 logger_wrapper-0.1.0/setup.cfg
+-rw-rw-r--   0 erol      (1000) erol      (1000)      248 2023-05-04 04:53:43.000000 logger_wrapper-0.1.0/setup.py
+drwxrwxr-x   0 erol      (1000) erol      (1000)        0 2023-05-04 08:13:38.474964 logger_wrapper-0.1.0/src/
+drwxrwxr-x   0 erol      (1000) erol      (1000)        0 2023-05-04 08:13:38.474964 logger_wrapper-0.1.0/src/logger_wrapper/
+-rw-rw-r--   0 erol      (1000) erol      (1000)     1605 2023-05-04 06:52:31.000000 logger_wrapper-0.1.0/src/logger_wrapper/__init__.py
+-rw-rw-r--   0 erol      (1000) erol      (1000)    17513 2023-05-04 07:42:15.000000 logger_wrapper-0.1.0/src/logger_wrapper/logger_wrapper.py
+-rw-rw-r--   0 erol      (1000) erol      (1000)     2200 2023-05-02 03:07:17.000000 logger_wrapper-0.1.0/src/logger_wrapper/scratch.py
+drwxrwxr-x   0 erol      (1000) erol      (1000)        0 2023-05-04 08:13:38.474964 logger_wrapper-0.1.0/src/logger_wrapper.egg-info/
+-rw-rw-r--   0 erol      (1000) erol      (1000)     8900 2023-05-04 08:13:38.000000 logger_wrapper-0.1.0/src/logger_wrapper.egg-info/PKG-INFO
+-rw-rw-r--   0 erol      (1000) erol      (1000)      338 2023-05-04 08:13:38.000000 logger_wrapper-0.1.0/src/logger_wrapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 erol      (1000) erol      (1000)        1 2023-05-04 08:13:38.000000 logger_wrapper-0.1.0/src/logger_wrapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 erol      (1000) erol      (1000)       15 2023-05-04 08:13:38.000000 logger_wrapper-0.1.0/src/logger_wrapper.egg-info/top_level.txt
+drwxrwxr-x   0 erol      (1000) erol      (1000)        0 2023-05-04 08:13:38.474964 logger_wrapper-0.1.0/tests/
+-rw-rw-r--   0 erol      (1000) erol      (1000)    12709 2023-05-04 07:59:11.000000 logger_wrapper-0.1.0/tests/test_logger_wrapper.py
```

### Comparing `logger_wrapper-0.0.1/pyproject.toml` & `logger_wrapper-0.1.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "logger_wrapper"
-version = "0.0.1"
+version = "0.1.0"
 authors = [
   { name="Erol Yesin", email="erol@sandboxzilla.net" },
 ]
-description = "The package wraps the built-in logger.  There are options to track the code location from where the log message was created."
+description = "The package wraps the built-in Logger package.  There are options to track from where the log message was created."
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.11"
 keywords=["logger", "logging", "syslog", "location", "formating"]
 classifiers = [
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',
-    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/sandboxzilla/logger-wrapper"
 "Bug Tracker" = "https://https://github.com/sandboxzilla/logger-wrapper/issues"
```

