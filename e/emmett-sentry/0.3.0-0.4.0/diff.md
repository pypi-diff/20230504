# Comparing `tmp/emmett_sentry-0.3.0.tar.gz` & `tmp/emmett_sentry-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emmett_sentry-0.3.0.tar", max compression
+gzip compressed data, was "emmett_sentry-0.4.0.tar", max compression
```

## Comparing `emmett_sentry-0.3.0.tar` & `emmett_sentry-0.4.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1486 2023-04-21 10:06:32.939689 emmett_sentry-0.3.0/LICENSE
--rw-r--r--   0        0        0     1393 2023-04-21 10:06:32.939689 emmett_sentry-0.3.0/README.md
--rw-r--r--   0        0        0       24 2023-04-21 10:06:32.939689 emmett_sentry-0.3.0/emmett_sentry/__init__.py
--rw-r--r--   0        0        0       22 2023-04-21 10:06:32.939689 emmett_sentry-0.3.0/emmett_sentry/__version__.py
--rw-r--r--   0        0        0     2354 2023-04-21 10:06:32.939689 emmett_sentry-0.3.0/emmett_sentry/ext.py
--rw-r--r--   0        0        0     7672 2023-04-21 10:06:32.939689 emmett_sentry-0.3.0/emmett_sentry/helpers.py
--rw-r--r--   0        0        0     1298 2023-04-21 10:06:32.939689 emmett_sentry-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2158 1970-01-01 00:00:00.000000 emmett_sentry-0.3.0/setup.py
--rw-r--r--   0        0        0     2864 1970-01-01 00:00:00.000000 emmett_sentry-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1486 2023-05-04 13:00:36.892799 emmett_sentry-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1475 2023-05-04 13:00:36.892799 emmett_sentry-0.4.0/README.md
+-rw-r--r--   0        0        0       24 2023-05-04 13:00:36.892799 emmett_sentry-0.4.0/emmett_sentry/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-04 13:00:36.892799 emmett_sentry-0.4.0/emmett_sentry/__version__.py
+-rw-r--r--   0        0        0     2469 2023-05-04 13:00:36.892799 emmett_sentry-0.4.0/emmett_sentry/ext.py
+-rw-r--r--   0        0        0     7878 2023-05-04 13:00:36.892799 emmett_sentry-0.4.0/emmett_sentry/helpers.py
+-rw-r--r--   0        0        0     1298 2023-05-04 13:00:36.892799 emmett_sentry-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2243 1970-01-01 00:00:00.000000 emmett_sentry-0.4.0/setup.py
+-rw-r--r--   0        0        0     2946 1970-01-01 00:00:00.000000 emmett_sentry-0.4.0/PKG-INFO
```

### Comparing `emmett_sentry-0.3.0/LICENSE` & `emmett_sentry-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `emmett_sentry-0.3.0/README.md` & `emmett_sentry-0.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 | environment | development | Application environment |
 | release | | Application release |
 | auto\_load | `True` | Automatically inject extension on routes |
 | enable\_tracing | `False` | Enable tracing on routes |
 | sample\_rate | 1 | Error sampling rate |
 | traces\_sample\_rate | | Traces sampling rate |
 | trace\_websockets | `False` | Enable tracing on websocket routes |
+| tracing\_exclude\_routes | | List of specific routes to exclude from tracing | 
 
 ## Usage
 
 The extension exposes two methods to manually track events:
 
 - exception
 - message
```

### Comparing `emmett_sentry-0.3.0/emmett_sentry/ext.py` & `emmett_sentry-0.4.0/emmett_sentry/ext.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,24 +28,26 @@
         dsn="",
         environment="development",
         release=None,
         auto_load=True,
         enable_tracing=False,
         sample_rate=1.0,
         traces_sample_rate=None,
-        trace_websockets=False
+        trace_websockets=False,
+        tracing_exclude_routes=[]
     )
     _initialized = False
     _errmsg = "You need to configure Sentry extension before using its methods"
 
     def on_load(self):
         self._scopes = {}
         self._before_send_callbacks = []
         if not self.config.dsn:
             return
+        self._tracing_excluded_routes = set(self.config.tracing_exclude_routes)
         sentry_sdk.init(
             dsn=self.config.dsn,
             environment=self.config.environment,
             release=self.config.release,
             sample_rate=self.config.sample_rate,
             traces_sample_rate=self.config.traces_sample_rate,
             before_send=self._before_send
```

### Comparing `emmett_sentry-0.3.0/emmett_sentry/helpers.py` & `emmett_sentry-0.4.0/emmett_sentry/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,41 +196,45 @@
                     except Exception as exc:
                         _capture_exception(hub, exc)
                         raise
     return wrap
 
 
 def _build_routing_rec_http(ext, rec_cls):
-    wrapper = (
-        _build_http_dispatcher_wrapper_txn if ext.config.enable_tracing else
-        _build_http_dispatcher_wrapper_err
-    )
-
     def _routing_rec_http(router, name, match, dispatch):
+        wrapper = (
+            _build_http_dispatcher_wrapper_txn if (
+                ext.config.enable_tracing and
+                name not in ext._tracing_excluded_routes
+            ) else _build_http_dispatcher_wrapper_err
+        )
+
         return rec_cls(
             name=name,
             match=match,
-            dispatch=wrapper(ext, dispatch)
+            dispatch=wrapper(ext, name, dispatch)
         )
 
     return _routing_rec_http
 
 
 def _build_routing_rec_ws(ext, rec_cls):
-    wrapper = (
-        _build_ws_dispatcher_wrapper_txn if (
-            ext.config.enable_tracing and ext.config.trace_websockets
-        ) else _build_ws_dispatcher_wrapper_err
-    )
-
     def _routing_rec_ws(router, name, match, dispatch, flow_recv, flow_send):
+        wrapper = (
+            _build_ws_dispatcher_wrapper_txn if (
+                ext.config.enable_tracing and
+                ext.config.trace_websockets and
+                name not in ext._tracing_excluded_routes
+            ) else _build_ws_dispatcher_wrapper_err
+        )
+
         return rec_cls(
             name=name,
             match=match,
-            dispatch=wrapper(ext, dispatch),
+            dispatch=wrapper(ext, name, dispatch),
             flow_recv=flow_recv,
             flow_send=flow_send
         )
 
     return _routing_rec_ws
```

### Comparing `emmett_sentry-0.3.0/pyproject.toml` & `emmett_sentry-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "emmett-sentry"
-version = "0.3.0"
+version = "0.4.0"
 description = "Sentry extension for Emmett framework"
 authors = ["Giovanni Barillari <g@baro.dev>"]
 license = "BSD-3-Clause"
 
 readme = "README.md"
 homepage = "https://github.com/emmett-framework/sentry"
 repository = "https://github.com/emmett-framework/sentry"
```

### Comparing `emmett_sentry-0.3.0/setup.py` & `emmett_sentry-0.4.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['emmett>=2.5.0,<3.0.0', 'sentry-sdk>=1.20.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'emmett-sentry',
-    'version': '0.3.0',
+    'version': '0.4.0',
     'description': 'Sentry extension for Emmett framework',
-    'long_description': '# Emmett-Sentry\n\nEmmett-Sentry is an [Emmett framework](https://emmett.sh) extension integrating [Sentry](https://sentry.io) monitoring platform.\n\n[![pip version](https://img.shields.io/pypi/v/emmett-sentry.svg?style=flat)](https://pypi.python.org/pypi/emmett-sentry) \n\n## Installation\n\nYou can install Emmett-Sentry using pip:\n\n    pip install emmett-sentry\n\nAnd add it to your Emmett application:\n\n```python\nfrom emmett_sentry import Sentry\n\nsentry = app.use_extension(Sentry)\n```\n\n## Configuration\n\nHere is the complete list of parameters of the extension configuration:\n\n| param | default | description |\n| --- | --- | --- |\n| dsn | | Sentry project\'s DSN |\n| environment | development | Application environment |\n| release | | Application release |\n| auto\\_load | `True` | Automatically inject extension on routes |\n| enable\\_tracing | `False` | Enable tracing on routes |\n| sample\\_rate | 1 | Error sampling rate |\n| traces\\_sample\\_rate | | Traces sampling rate |\n| trace\\_websockets | `False` | Enable tracing on websocket routes |\n\n## Usage\n\nThe extension exposes two methods to manually track events:\n\n- exception\n- message\n\nYou call these methods directly within your code:\n\n```python\n# track an error\ntry:\n    1 / 0\nexcept Exception:\n    sentry.exception()\n\n# track a message\nsentry.message("some event", level="info")\n```\n\n## License\n\nEmmett-Sentry is released under BSD license.\n',
+    'long_description': '# Emmett-Sentry\n\nEmmett-Sentry is an [Emmett framework](https://emmett.sh) extension integrating [Sentry](https://sentry.io) monitoring platform.\n\n[![pip version](https://img.shields.io/pypi/v/emmett-sentry.svg?style=flat)](https://pypi.python.org/pypi/emmett-sentry) \n\n## Installation\n\nYou can install Emmett-Sentry using pip:\n\n    pip install emmett-sentry\n\nAnd add it to your Emmett application:\n\n```python\nfrom emmett_sentry import Sentry\n\nsentry = app.use_extension(Sentry)\n```\n\n## Configuration\n\nHere is the complete list of parameters of the extension configuration:\n\n| param | default | description |\n| --- | --- | --- |\n| dsn | | Sentry project\'s DSN |\n| environment | development | Application environment |\n| release | | Application release |\n| auto\\_load | `True` | Automatically inject extension on routes |\n| enable\\_tracing | `False` | Enable tracing on routes |\n| sample\\_rate | 1 | Error sampling rate |\n| traces\\_sample\\_rate | | Traces sampling rate |\n| trace\\_websockets | `False` | Enable tracing on websocket routes |\n| tracing\\_exclude\\_routes | | List of specific routes to exclude from tracing | \n\n## Usage\n\nThe extension exposes two methods to manually track events:\n\n- exception\n- message\n\nYou call these methods directly within your code:\n\n```python\n# track an error\ntry:\n    1 / 0\nexcept Exception:\n    sentry.exception()\n\n# track a message\nsentry.message("some event", level="info")\n```\n\n## License\n\nEmmett-Sentry is released under BSD license.\n',
     'author': 'Giovanni Barillari',
     'author_email': 'g@baro.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/emmett-framework/sentry',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `emmett_sentry-0.3.0/PKG-INFO` & `emmett_sentry-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emmett-sentry
-Version: 0.3.0
+Version: 0.4.0
 Summary: Sentry extension for Emmett framework
 Home-page: https://github.com/emmett-framework/sentry
 License: BSD-3-Clause
 Keywords: sentry,logging,emmett
 Author: Giovanni Barillari
 Author-email: g@baro.dev
 Requires-Python: >=3.8,<4.0
@@ -62,14 +62,15 @@
 | environment | development | Application environment |
 | release | | Application release |
 | auto\_load | `True` | Automatically inject extension on routes |
 | enable\_tracing | `False` | Enable tracing on routes |
 | sample\_rate | 1 | Error sampling rate |
 | traces\_sample\_rate | | Traces sampling rate |
 | trace\_websockets | `False` | Enable tracing on websocket routes |
+| tracing\_exclude\_routes | | List of specific routes to exclude from tracing | 
 
 ## Usage
 
 The extension exposes two methods to manually track events:
 
 - exception
 - message
```

