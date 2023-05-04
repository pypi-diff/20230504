# Comparing `tmp/emmett_prometheus-0.1.4.tar.gz` & `tmp/emmett_prometheus-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emmett_prometheus-0.1.4.tar", max compression
+gzip compressed data, was "emmett_prometheus-0.1.5.tar", max compression
```

## Comparing `emmett_prometheus-0.1.4.tar` & `emmett_prometheus-0.1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1486 2023-05-04 12:45:12.605244 emmett_prometheus-0.1.4/LICENSE
--rw-r--r--   0        0        0     1831 2023-05-04 12:45:12.605244 emmett_prometheus-0.1.4/README.md
--rw-r--r--   0        0        0       28 2023-05-04 12:45:12.605244 emmett_prometheus-0.1.4/emmett_prometheus/__init__.py
--rw-r--r--   0        0        0       22 2023-05-04 12:45:12.605244 emmett_prometheus-0.1.4/emmett_prometheus/__version__.py
--rw-r--r--   0        0        0     6488 2023-05-04 12:45:12.605244 emmett_prometheus-0.1.4/emmett_prometheus/ext.py
--rw-r--r--   0        0        0     1369 2023-05-04 12:45:12.605244 emmett_prometheus-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3379 1970-01-01 00:00:00.000000 emmett_prometheus-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1486 2023-05-04 13:08:07.596982 emmett_prometheus-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1831 2023-05-04 13:08:07.596982 emmett_prometheus-0.1.5/README.md
+-rw-r--r--   0        0        0       28 2023-05-04 13:08:07.596982 emmett_prometheus-0.1.5/emmett_prometheus/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-04 13:08:07.596982 emmett_prometheus-0.1.5/emmett_prometheus/__version__.py
+-rw-r--r--   0        0        0     6534 2023-05-04 13:08:07.596982 emmett_prometheus-0.1.5/emmett_prometheus/ext.py
+-rw-r--r--   0        0        0     1369 2023-05-04 13:08:07.596982 emmett_prometheus-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3379 1970-01-01 00:00:00.000000 emmett_prometheus-0.1.5/PKG-INFO
```

### Comparing `emmett_prometheus-0.1.4/LICENSE` & `emmett_prometheus-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `emmett_prometheus-0.1.4/README.md` & `emmett_prometheus-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `emmett_prometheus-0.1.4/emmett_prometheus/ext.py` & `emmett_prometheus-0.1.5/emmett_prometheus/ext.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,20 +70,23 @@
                 self.config.metrics_names["ws_send_counter"],
                 "Websockets sent messages counter",
                 labelnames=["websocket"]
             )
             self._pipe_ws = PrometheusWSPipe(self)
 
         if self.config.auto_load:
-            self.appmod = self.app.module(__name__, "emmett_prometheus")
+            self.appmod = self.app.module(
+                __name__,
+                "emmett_prometheus",
+                hostname=self.config.metrics_route_hostname
+            )
             self.appmod.route(
                 self.config.metrics_route_path,
                 name="metrics",
                 methods='get',
-                hostname=self.config.metrics_route_hostname,
                 output='bytes'
             )(self._metrics_route)
 
     @listen_signal(Signals.before_route)
     def _inject_pipes(self, route, f):
         if not self.config.auto_load:
             return
```

### Comparing `emmett_prometheus-0.1.4/pyproject.toml` & `emmett_prometheus-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "emmett-prometheus"
-version = "0.1.4"
+version = "0.1.5"
 description = "Prometheus extension for Emmett framework"
 authors = ["Giovanni Barillari <g@baro.dev>"]
 license = "BSD-3-Clause"
 
 readme = "README.md"
 homepage = "https://github.com/emmett-framework/prometheus"
 repository = "https://github.com/emmett-framework/prometheus"
```

### Comparing `emmett_prometheus-0.1.4/PKG-INFO` & `emmett_prometheus-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emmett-prometheus
-Version: 0.1.4
+Version: 0.1.5
 Summary: Prometheus extension for Emmett framework
 Home-page: https://github.com/emmett-framework/prometheus
 License: BSD-3-Clause
 Keywords: prometheus,monitoring,emmett
 Author: Giovanni Barillari
 Author-email: g@baro.dev
 Requires-Python: >=3.8,<4.0
```

