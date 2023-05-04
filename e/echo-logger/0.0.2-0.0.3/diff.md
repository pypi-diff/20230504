# Comparing `tmp/echo_logger-0.0.2.tar.gz` & `tmp/echo_logger-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echo_logger-0.0.2.tar", last modified: Fri Apr 28 05:37:47 2023, max compression
+gzip compressed data, was "echo_logger-0.0.3.tar", last modified: Thu May  4 01:33:48 2023, max compression
```

## Comparing `echo_logger-0.0.2.tar` & `echo_logger-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 05:37:47.498410 echo_logger-0.0.2/
--rw-rw-rw-   0        0        0     1087 2023-04-28 05:16:22.000000 echo_logger-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      659 2023-04-28 05:37:47.498410 echo_logger-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      216 2023-04-28 05:18:15.000000 echo_logger-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-28 05:37:47.492413 echo_logger-0.0.2/echo_logger/
--rw-rw-rw-   0        0        0       90 2023-04-28 05:21:08.000000 echo_logger-0.0.2/echo_logger/__init__.py
--rw-rw-rw-   0        0        0     3847 2023-04-28 05:19:56.000000 echo_logger-0.0.2/echo_logger/echo_logger.py
-drwxrwxrwx   0        0        0        0 2023-04-28 05:37:47.497402 echo_logger-0.0.2/echo_logger.egg-info/
--rw-rw-rw-   0        0        0      659 2023-04-28 05:37:47.000000 echo_logger-0.0.2/echo_logger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-04-28 05:37:47.000000 echo_logger-0.0.2/echo_logger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 05:37:47.000000 echo_logger-0.0.2/echo_logger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-28 05:37:47.000000 echo_logger-0.0.2/echo_logger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-28 05:37:47.499401 echo_logger-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      663 2023-04-28 05:37:42.000000 echo_logger-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 01:33:48.434180 echo_logger-0.0.3/
+-rw-rw-rw-   0        0        0     1087 2023-04-28 05:16:22.000000 echo_logger-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      659 2023-05-04 01:33:48.433180 echo_logger-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-04-28 05:18:15.000000 echo_logger-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 01:33:48.376182 echo_logger-0.0.3/echo_logger/
+-rw-rw-rw-   0        0        0       90 2023-04-28 05:21:08.000000 echo_logger-0.0.3/echo_logger/__init__.py
+-rw-rw-rw-   0        0        0     4012 2023-05-04 01:32:32.000000 echo_logger-0.0.3/echo_logger/echo_logger.py
+drwxrwxrwx   0        0        0        0 2023-05-04 01:33:48.430180 echo_logger-0.0.3/echo_logger.egg-info/
+-rw-rw-rw-   0        0        0      659 2023-05-04 01:33:48.000000 echo_logger-0.0.3/echo_logger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-05-04 01:33:48.000000 echo_logger-0.0.3/echo_logger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 01:33:48.000000 echo_logger-0.0.3/echo_logger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-04 01:33:48.000000 echo_logger-0.0.3/echo_logger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 01:33:48.435381 echo_logger-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      663 2023-05-04 01:33:30.000000 echo_logger-0.0.3/setup.py
```

### Comparing `echo_logger-0.0.2/LICENSE` & `echo_logger-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `echo_logger-0.0.2/PKG-INFO` & `echo_logger-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echo_logger
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple logger for python, with color and time
 Home-page: https://github.com/void-echo/echo_logger/
 Author: Echo Void
 Author-email: void-echo@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `echo_logger-0.0.2/echo_logger/echo_logger.py` & `echo_logger-0.0.3/echo_logger/echo_logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 import time
 
-
+echo_logger_debug = True
 class _colors:
     RESET = "\033[0m"  # Text Reset
 
     # Regular Colors
     BLACK = "\033[0;30m"  # BLACK
     RED = "\033[0;31m"  # RED
     GREEN = "\033[0;32m"  # GREEN
@@ -73,28 +73,34 @@
     BLUE_BACKGROUND_BRIGHT = "\033[0;104m"  # BLUE
     PURPLE_BACKGROUND_BRIGHT = "\033[0;105m"  # PURPLE
     CYAN_BACKGROUND_BRIGHT = "\033[0;106m"  # CYAN
     WHITE_BACKGROUND_BRIGHT = "\033[0;107m"  # WHITE
 
 
 def print_info(*args, **kwargs):
+    if not echo_logger_debug:
+        return
     # print with green color: [INFO]
     with_time = kwargs.pop('with_time', False)
     pre_print_str = _colors.GREEN_BOLD + '[INFO]' + _colors.RESET if not with_time else _colors.GREEN_BOLD + '[INFO ' + time.strftime(
         '%Y-%m-%d %H:%M:%S', time.localtime(time.time())) + ']' + _colors.RESET
     print(pre_print_str, *args, **kwargs)
 
 
 def print_err(*args, **kwargs):
+    if not echo_logger_debug:
+        return
     # print with red color: [ERROR]
     with_time = kwargs.pop('with_time', False)
     pre_print_str = _colors.RED_BOLD + '[ERR ]' + _colors.RESET if not with_time else _colors.RED_BOLD + '[ERR  ' + time.strftime(
         '%Y-%m-%d %H:%M:%S', time.localtime(time.time())) + ']' + _colors.RESET
     print(pre_print_str, *args, **kwargs)
 
 
 def print_warn(*args, **kwargs):
+    if not echo_logger_debug:
+        return
     # print with yellow color: [WARNING]
     with_time = kwargs.pop('with_time', False)
     pre_print_str = _colors.YELLOW_BOLD + '[WARN]' + _colors.RESET if not with_time else _colors.YELLOW_BOLD + '[WARN ' + time.strftime(
         '%Y-%m-%d %H:%M:%S', time.localtime(time.time())) + ']' + _colors.RESET
     print(pre_print_str, *args, **kwargs)
```

### Comparing `echo_logger-0.0.2/echo_logger.egg-info/PKG-INFO` & `echo_logger-0.0.3/echo_logger.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echo-logger
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple logger for python, with color and time
 Home-page: https://github.com/void-echo/echo_logger/
 Author: Echo Void
 Author-email: void-echo@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `echo_logger-0.0.2/setup.py` & `echo_logger-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="echo_logger",
-    version="0.0.2",
+    version="0.0.3",
     author="Echo Void",
     author_email="void-echo@outlook.com",
     description="A simple logger for python, with color and time",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/void-echo/echo_logger/",
     packages=setuptools.find_packages(),
```

