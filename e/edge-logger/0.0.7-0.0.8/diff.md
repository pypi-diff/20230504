# Comparing `tmp/edge_logger-0.0.7.tar.gz` & `tmp/edge_logger-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edge_logger-0.0.7.tar", max compression
+gzip compressed data, was "edge_logger-0.0.8.tar", max compression
```

## Comparing `edge_logger-0.0.7.tar` & `edge_logger-0.0.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-04-16 19:59:55.248252 edge_logger-0.0.7/LICENSE
--rw-r--r--   0        0        0        0 2023-04-17 03:01:06.502367 edge_logger-0.0.7/README.md
--rw-r--r--   0        0        0        0 2023-04-16 20:07:03.564649 edge_logger-0.0.7/edge_logger/__init__.py
--rw-r--r--   0        0        0     6536 2023-05-04 01:27:08.198457 edge_logger-0.0.7/edge_logger/edge_logger.py
--rw-r--r--   0        0        0      380 2023-05-04 01:56:24.556719 edge_logger-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      480 1970-01-01 00:00:00.000000 edge_logger-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-16 19:59:55.248252 edge_logger-0.0.8/LICENSE
+-rw-r--r--   0        0        0        0 2023-04-17 03:01:06.502367 edge_logger-0.0.8/README.md
+-rw-r--r--   0        0        0        0 2023-04-16 20:07:03.564649 edge_logger-0.0.8/edge_logger/__init__.py
+-rw-r--r--   0        0        0     6012 2023-05-04 02:30:39.656027 edge_logger-0.0.8/edge_logger/edge_logger.py
+-rw-r--r--   0        0        0      380 2023-05-04 02:30:39.651033 edge_logger-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      480 1970-01-01 00:00:00.000000 edge_logger-0.0.8/PKG-INFO
```

### Comparing `edge_logger-0.0.7/LICENSE` & `edge_logger-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `edge_logger-0.0.7/edge_logger/edge_logger.py` & `edge_logger-0.0.8/edge_logger/edge_logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,33 +90,21 @@
 
 class EdgeLogger(logging.Logger):
     """
     Subclass logging.Logger so we can extend makeRecord to add dynamic information on a per-log basis
     https://docs.python.org/3/library/logging.html#logging.Logger
     """
 
-    def __init__(self, name: str, stream=sys.stdout, console_handler=True, logger_level="INFO", console_level="DEBUG"):
+    def __init__(self, name: str):
 
         # root logger
         super().__init__(name)
 
         # Base logger level. Messages will be further filtered by each handler.
-        self.setLevel(logger_level)
-
-        if console_handler:
-            # create console handler and set level to info
-            ch = logging.StreamHandler(stream=stream)
-            ch.set_name("console_handler")
-
-            # Console handler log level will filter the messages that are actually sent to stdout.
-            ch.setLevel(console_level)
-            ch.setFormatter(JsonFormatter())
-
-            # add ch to logger
-            self.addHandler(ch)
+        self.setLevel("INFO")
 
     def add_console_handler(self, stream=sys.stdout, handler_level="INFO"):
         # create console handler and set level to info
         ch = logging.StreamHandler(stream=stream)
         ch.set_name("console_handler")
 
         # Console handler log level will filter the messages that are actually sent to stdout.
```

