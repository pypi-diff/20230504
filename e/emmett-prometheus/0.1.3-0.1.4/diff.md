# Comparing `tmp/emmett_prometheus-0.1.3.tar.gz` & `tmp/emmett_prometheus-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emmett_prometheus-0.1.3.tar", max compression
+gzip compressed data, was "emmett_prometheus-0.1.4.tar", max compression
```

## Comparing `emmett_prometheus-0.1.3.tar` & `emmett_prometheus-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1486 2023-04-21 08:16:18.158111 emmett_prometheus-0.1.3/LICENSE
--rw-r--r--   0        0        0     1831 2023-04-21 08:16:18.158111 emmett_prometheus-0.1.3/README.md
--rw-r--r--   0        0        0       28 2023-04-21 08:16:18.158111 emmett_prometheus-0.1.3/emmett_prometheus/__init__.py
--rw-r--r--   0        0        0       22 2023-04-21 08:16:18.158111 emmett_prometheus-0.1.3/emmett_prometheus/__version__.py
--rw-r--r--   0        0        0     6380 2023-04-21 08:16:18.158111 emmett_prometheus-0.1.3/emmett_prometheus/ext.py
--rw-r--r--   0        0        0     1369 2023-04-21 08:16:18.158111 emmett_prometheus-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3379 1970-01-01 00:00:00.000000 emmett_prometheus-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1486 2023-05-04 12:45:12.605244 emmett_prometheus-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1831 2023-05-04 12:45:12.605244 emmett_prometheus-0.1.4/README.md
+-rw-r--r--   0        0        0       28 2023-05-04 12:45:12.605244 emmett_prometheus-0.1.4/emmett_prometheus/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-04 12:45:12.605244 emmett_prometheus-0.1.4/emmett_prometheus/__version__.py
+-rw-r--r--   0        0        0     6488 2023-05-04 12:45:12.605244 emmett_prometheus-0.1.4/emmett_prometheus/ext.py
+-rw-r--r--   0        0        0     1369 2023-05-04 12:45:12.605244 emmett_prometheus-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3379 1970-01-01 00:00:00.000000 emmett_prometheus-0.1.4/PKG-INFO
```

### Comparing `emmett_prometheus-0.1.3/LICENSE` & `emmett_prometheus-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `emmett_prometheus-0.1.3/README.md` & `emmett_prometheus-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `emmett_prometheus-0.1.3/emmett_prometheus/ext.py` & `emmett_prometheus-0.1.4/emmett_prometheus/ext.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,16 +70,18 @@
                 self.config.metrics_names["ws_send_counter"],
                 "Websockets sent messages counter",
                 labelnames=["websocket"]
             )
             self._pipe_ws = PrometheusWSPipe(self)
 
         if self.config.auto_load:
-            self.app.route(
+            self.appmod = self.app.module(__name__, "emmett_prometheus")
+            self.appmod.route(
                 self.config.metrics_route_path,
+                name="metrics",
                 methods='get',
                 hostname=self.config.metrics_route_hostname,
                 output='bytes'
             )(self._metrics_route)
 
     @listen_signal(Signals.before_route)
     def _inject_pipes(self, route, f):
```

### Comparing `emmett_prometheus-0.1.3/pyproject.toml` & `emmett_prometheus-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "emmett-prometheus"
-version = "0.1.3"
+version = "0.1.4"
 description = "Prometheus extension for Emmett framework"
 authors = ["Giovanni Barillari <g@baro.dev>"]
 license = "BSD-3-Clause"
 
 readme = "README.md"
 homepage = "https://github.com/emmett-framework/prometheus"
 repository = "https://github.com/emmett-framework/prometheus"
```

### Comparing `emmett_prometheus-0.1.3/PKG-INFO` & `emmett_prometheus-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emmett-prometheus
-Version: 0.1.3
+Version: 0.1.4
 Summary: Prometheus extension for Emmett framework
 Home-page: https://github.com/emmett-framework/prometheus
 License: BSD-3-Clause
 Keywords: prometheus,monitoring,emmett
 Author: Giovanni Barillari
 Author-email: g@baro.dev
 Requires-Python: >=3.8,<4.0
```

