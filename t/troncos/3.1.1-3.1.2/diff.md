# Comparing `tmp/troncos-3.1.1.tar.gz` & `tmp/troncos-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "troncos-3.1.1.tar", max compression
+gzip compressed data, was "troncos-3.1.2.tar", max compression
```

## Comparing `troncos-3.1.1.tar` & `troncos-3.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1077 2023-03-20 12:33:38.383234 troncos-3.1.1/LICENSE
--rw-r--r--   0        0        0    15620 2023-03-20 12:33:38.383234 troncos-3.1.1/README.md
--rw-r--r--   0        0        0     2258 2023-03-20 12:33:38.383234 troncos-3.1.1/pyproject.toml
--rw-r--r--   0        0        0      291 2023-03-20 12:33:38.383234 troncos-3.1.1/troncos/__init__.py
--rw-r--r--   0        0        0     1214 2023-03-20 12:33:38.387234 troncos-3.1.1/troncos/_ddlazy/__init__.py
--rw-r--r--   0        0        0        0 2023-03-20 12:33:38.387234 troncos-3.1.1/troncos/frameworks/__init__.py
--rw-r--r--   0        0        0        0 2023-03-20 12:33:38.387234 troncos-3.1.1/troncos/frameworks/asgi/__init__.py
--rw-r--r--   0        0        0     2595 2023-03-20 12:33:38.387234 troncos-3.1.1/troncos/frameworks/asgi/middleware.py
--rw-r--r--   0        0        0     3367 2023-03-20 12:33:38.387234 troncos-3.1.1/troncos/frameworks/asgi/utils.py
--rw-r--r--   0        0        0      993 2023-03-20 12:33:38.387234 troncos-3.1.1/troncos/frameworks/gunicorn/__init__.py
--rw-r--r--   0        0        0        0 2023-03-20 12:33:38.387234 troncos-3.1.1/troncos/frameworks/starlette/__init__.py
--rw-r--r--   0        0        0     4488 2023-03-20 12:33:38.387234 troncos-3.1.1/troncos/frameworks/starlette/uvicorn.py
--rw-r--r--   0        0        0        0 2023-03-20 12:33:38.387234 troncos-3.1.1/troncos/frameworks/structlog/__init__.py
--rw-r--r--   0        0        0     2044 2023-03-20 12:33:38.387234 troncos-3.1.1/troncos/frameworks/structlog/processors.py
--rw-r--r--   0        0        0     5589 2023-03-20 12:33:38.387234 troncos-3.1.1/troncos/frameworks/structlog/setup.py
--rw-r--r--   0        0        0     4922 2023-03-20 12:33:38.387234 troncos-3.1.1/troncos/logs/__init__.py
--rw-r--r--   0        0        0     3430 2023-03-20 12:33:38.387234 troncos-3.1.1/troncos/logs/filters.py
--rw-r--r--   0        0        0     9364 2023-03-20 12:33:38.387234 troncos-3.1.1/troncos/logs/formatters.py
--rw-r--r--   0        0        0     3090 2023-03-20 12:33:38.387234 troncos-3.1.1/troncos/profiling/__init__.py
--rw-r--r--   0        0        0        0 2023-03-20 12:33:38.387234 troncos-3.1.1/troncos/py.typed
--rw-r--r--   0        0        0    10468 2023-03-20 12:33:38.387234 troncos-3.1.1/troncos/traces/__init__.py
--rw-r--r--   0        0        0     6599 2023-03-20 12:33:38.387234 troncos-3.1.1/troncos/traces/dd_shim.py
--rw-r--r--   0        0        0     8351 2023-03-20 12:33:38.387234 troncos-3.1.1/troncos/traces/decorate.py
--rw-r--r--   0        0        0     1459 2023-03-20 12:33:38.387234 troncos-3.1.1/troncos/traces/propagation.py
--rw-r--r--   0        0        0    17312 1970-01-01 00:00:00.000000 troncos-3.1.1/setup.py
--rw-r--r--   0        0        0    16639 1970-01-01 00:00:00.000000 troncos-3.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-04 15:52:24.932265 troncos-3.1.2/LICENSE
+-rw-r--r--   0        0        0    15620 2023-05-04 15:52:24.932265 troncos-3.1.2/README.md
+-rw-r--r--   0        0        0     2258 2023-05-04 15:52:24.936265 troncos-3.1.2/pyproject.toml
+-rw-r--r--   0        0        0      291 2023-05-04 15:52:24.936265 troncos-3.1.2/troncos/__init__.py
+-rw-r--r--   0        0        0     1214 2023-05-04 15:52:24.936265 troncos-3.1.2/troncos/_ddlazy/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 15:52:24.936265 troncos-3.1.2/troncos/frameworks/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 15:52:24.936265 troncos-3.1.2/troncos/frameworks/asgi/__init__.py
+-rw-r--r--   0        0        0     2595 2023-05-04 15:52:24.936265 troncos-3.1.2/troncos/frameworks/asgi/middleware.py
+-rw-r--r--   0        0        0     3367 2023-05-04 15:52:24.936265 troncos-3.1.2/troncos/frameworks/asgi/utils.py
+-rw-r--r--   0        0        0      993 2023-05-04 15:52:24.936265 troncos-3.1.2/troncos/frameworks/gunicorn/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 15:52:24.936265 troncos-3.1.2/troncos/frameworks/starlette/__init__.py
+-rw-r--r--   0        0        0     4488 2023-05-04 15:52:24.936265 troncos-3.1.2/troncos/frameworks/starlette/uvicorn.py
+-rw-r--r--   0        0        0        0 2023-05-04 15:52:24.936265 troncos-3.1.2/troncos/frameworks/structlog/__init__.py
+-rw-r--r--   0        0        0     2044 2023-05-04 15:52:24.936265 troncos-3.1.2/troncos/frameworks/structlog/processors.py
+-rw-r--r--   0        0        0     5589 2023-05-04 15:52:24.936265 troncos-3.1.2/troncos/frameworks/structlog/setup.py
+-rw-r--r--   0        0        0     4922 2023-05-04 15:52:24.936265 troncos-3.1.2/troncos/logs/__init__.py
+-rw-r--r--   0        0        0     3430 2023-05-04 15:52:24.936265 troncos-3.1.2/troncos/logs/filters.py
+-rw-r--r--   0        0        0     9364 2023-05-04 15:52:24.936265 troncos-3.1.2/troncos/logs/formatters.py
+-rw-r--r--   0        0        0     3090 2023-05-04 15:52:24.936265 troncos-3.1.2/troncos/profiling/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 15:52:24.936265 troncos-3.1.2/troncos/py.typed
+-rw-r--r--   0        0        0    10468 2023-05-04 15:52:24.936265 troncos-3.1.2/troncos/traces/__init__.py
+-rw-r--r--   0        0        0     6745 2023-05-04 15:52:24.936265 troncos-3.1.2/troncos/traces/dd_shim.py
+-rw-r--r--   0        0        0     8351 2023-05-04 15:52:24.936265 troncos-3.1.2/troncos/traces/decorate.py
+-rw-r--r--   0        0        0     1459 2023-05-04 15:52:24.936265 troncos-3.1.2/troncos/traces/propagation.py
+-rw-r--r--   0        0        0    17312 1970-01-01 00:00:00.000000 troncos-3.1.2/setup.py
+-rw-r--r--   0        0        0    16639 1970-01-01 00:00:00.000000 troncos-3.1.2/PKG-INFO
```

### Comparing `troncos-3.1.1/LICENSE` & `troncos-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `troncos-3.1.1/README.md` & `troncos-3.1.2/README.md`

 * *Files identical despite different names*

### Comparing `troncos-3.1.1/pyproject.toml` & `troncos-3.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "troncos"
-version = "3.1.1"
+version = "3.1.2"
 description = "Collection of Python logging, tracing and profiling tools"
 authors = [
     "Guðmundur Björn Birkisson <gudmundur.birkisson@oda.com>",
     "Karl Fredrik Haugland <karlfredrik.haugland@oda.com>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `troncos-3.1.1/troncos/_ddlazy/__init__.py` & `troncos-3.1.2/troncos/_ddlazy/__init__.py`

 * *Files identical despite different names*

### Comparing `troncos-3.1.1/troncos/frameworks/asgi/middleware.py` & `troncos-3.1.2/troncos/frameworks/asgi/middleware.py`

 * *Files identical despite different names*

### Comparing `troncos-3.1.1/troncos/frameworks/asgi/utils.py` & `troncos-3.1.2/troncos/frameworks/asgi/utils.py`

 * *Files identical despite different names*

### Comparing `troncos-3.1.1/troncos/frameworks/gunicorn/__init__.py` & `troncos-3.1.2/troncos/frameworks/gunicorn/__init__.py`

 * *Files identical despite different names*

### Comparing `troncos-3.1.1/troncos/frameworks/starlette/uvicorn.py` & `troncos-3.1.2/troncos/frameworks/starlette/uvicorn.py`

 * *Files identical despite different names*

### Comparing `troncos-3.1.1/troncos/frameworks/structlog/processors.py` & `troncos-3.1.2/troncos/frameworks/structlog/processors.py`

 * *Files identical despite different names*

### Comparing `troncos-3.1.1/troncos/frameworks/structlog/setup.py` & `troncos-3.1.2/troncos/frameworks/structlog/setup.py`

 * *Files identical despite different names*

### Comparing `troncos-3.1.1/troncos/logs/__init__.py` & `troncos-3.1.2/troncos/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `troncos-3.1.1/troncos/logs/filters.py` & `troncos-3.1.2/troncos/logs/filters.py`

 * *Files identical despite different names*

### Comparing `troncos-3.1.1/troncos/logs/formatters.py` & `troncos-3.1.2/troncos/logs/formatters.py`

 * *Files identical despite different names*

### Comparing `troncos-3.1.1/troncos/profiling/__init__.py` & `troncos-3.1.2/troncos/profiling/__init__.py`

 * *Files identical despite different names*

### Comparing `troncos-3.1.1/troncos/traces/__init__.py` & `troncos-3.1.2/troncos/traces/__init__.py`

 * *Files identical despite different names*

### Comparing `troncos-3.1.1/troncos/traces/dd_shim.py` & `troncos-3.1.2/troncos/traces/dd_shim.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,28 +20,36 @@
 
 class _TranslatedSpan(Span):
     def __init__(
         self,
         dd_span: Any,
         base_resources: Attributes,
         default_resource: Resource,
+        dd_traces_exported: bool,
         ignore_attrs: list[str],
     ) -> None:
         super().__init__(
             dd_span.name,
             _internal_span_context(dd_span),
             parent=self._create_parent_context(dd_span),
             sampler=None,
             trace_config=None,
             resource=self._create_resource(dd_span, base_resources, default_resource),
             kind=self._create_span_kind(dd_span),
             instrumentation_scope=_instrumentation_scope,
         )
         self.start(dd_span.start_ns)
         self._apply_translation(dd_span, ignore_attrs)
+        if dd_traces_exported:
+            self.set_attributes(
+                {
+                    "dd_trace_id": str(dd_span.trace_id),
+                    "dd_span_id": str(dd_span.span_id),
+                }
+            )
         self.end(dd_span.start_ns + dd_span.duration_ns)
 
     @staticmethod
     def _create_parent_context(dd_span: Any) -> SpanContext | None:
         if dd_span.parent_id:
             if not dd_span._parent:
                 # External trace parent
@@ -165,20 +173,18 @@
     def on_span_start(self, dd_span: Any) -> None:
         pass
 
     def on_span_finish(self, dd_span: Any) -> None:
         span = _TranslatedSpan(
             dd_span,
             base_resources=self._base_resources,  # type: ignore[arg-type]
+            dd_traces_exported=self._dd_traces_exported,
             default_resource=self._default_resource,
             ignore_attrs=self._dd_span_ignore_attr,
         )
-        if self._dd_traces_exported:
-            span.set_attribute("dd_trace_id", str(dd_span.trace_id))
-            span.set_attribute("dd_span_id", str(dd_span.span_id))
         for p in self._otel_procs:
             p.on_end(span)
 
     def shutdown(self, timeout: int) -> None:
         if self._flush_on_shutdown:
             for p in self._otel_procs:
                 p.force_flush(timeout_millis=timeout)
```

### Comparing `troncos-3.1.1/troncos/traces/decorate.py` & `troncos-3.1.2/troncos/traces/decorate.py`

 * *Files identical despite different names*

### Comparing `troncos-3.1.1/troncos/traces/propagation.py` & `troncos-3.1.2/troncos/traces/propagation.py`

 * *Files identical despite different names*

### Comparing `troncos-3.1.1/setup.py` & `troncos-3.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 extras_require = \
 {'grpc': ['opentelemetry-exporter-otlp-proto-grpc==1.16.0'],
  'http': ['opentelemetry-exporter-otlp-proto-http==1.16.0'],
  'structlog': ['structlog>=22.3.0,<23.0.0']}
 
 setup_kwargs = {
     'name': 'troncos',
-    'version': '3.1.1',
+    'version': '3.1.2',
     'description': 'Collection of Python logging, tracing and profiling tools',
     'long_description': '<h1 align="center" style="border-bottom: 0">\n  🪵<br>\n  Troncos <br/>\n</h1>\n\n<p align="center">\n    <em>\n        Collection of Python logging, tracing and profiling tools\n    </em>\n    <br>\n    <a href="https://github.com/kolonialno/troncos/actions?workflow=CI">\n        <img src="https://github.com/kolonialno/troncos/actions/workflows/ci.yml/badge.svg" alt="CI status">\n    </a>\n    <a href="https://pypi.python.org/pypi/troncos">\n        <img src="https://img.shields.io/pypi/v/troncos.svg">\n    </a>\n    <img src="https://img.shields.io/pypi/pyversions/troncos">\n    <a href="https://github.com/kolonialno/troncos/blob/master/LICENSE">\n        <img src="https://img.shields.io/github/license/kolonialno/troncos.svg">\n    </a>\n</p>\n\n<!-- TOC -->\n  * [Etymology](#etymology)\n  * [Installation](#installation)\n  * [Setup](#setup)\n    * [Choosing a trace exporter](#choosing-a-trace-exporter)\n      * [gRPC](#grpc)\n      * [http](#http)\n    * [Import order](#import-order)\n    * [Plain setup](#plain-setup)\n    * [Starlette with uvicorn](#starlette-with-uvicorn)\n    * [Django](#django)\n  * [Logging](#logging)\n    * [Thoughts on logging](#thoughts-on-logging)\n    * [Log traces with Gunicorn](#log-traces-with-gunicorn)\n    * [Structlog](#structlog)\n  * [Tracing](#tracing)\n    * [Tracing your code](#tracing-your-code)\n      * [trace_function](#tracefunction)\n      * [trace_block](#traceblock)\n      * [trace_class](#traceclass)\n      * [trace_module](#tracemodule)\n      * [trace_ignore](#traceignore)\n    * [Trace Propagation](#trace-propagation)\n      * [Send context](#send-context)\n      * [Receive context](#receive-context)\n    * [Trace sampling](#trace-sampling)\n    * [Trace debugging](#trace-debugging)\n  * [Profiling](#profiling)\n    * [Setup endpoint](#setup-endpoint)\n    * [Enable scraping](#enable-scraping)\n  * [Development](#development)\n<!-- TOC -->\n\n## Etymology\n\n"Troncos" is the plural of the spanish word "Tronco", which translates to "trunk" or "log".\n\n## Installation\n\n```console\n# With pip\n$ pip install troncos\n\n# With poetry (grpc trace exporter)\n$ poetry add troncos -E grpc\n\n# With poetry (http trace exporter)\n$ poetry add troncos -E http\n```\n\n## Setup\n\n> **Note**: It is a good idea to use a `settings.py`-file (or similar) as an authoritative source of variables (service name, environment, whether tracing is enabled or not, log level, etc). In this README we mostly use `os.environ` for the sake of clarity.\n\n### Choosing a trace exporter\n\nTo export your traces, you have to pick either `grpc` or `http`. Using `grpc` gives you significant performance gains. If you are running a critical service with high load in production, we recommend using `grpc`.\n\n#### gRPC\n\n```toml\n[tool.poetry.dependencies]\ntroncos = {version="?", extras = ["grpc"]}\n```\n\n#### http\n\n```toml\n[tool.poetry.dependencies]\ntroncos = {version="?", extras = ["http"]}\n```\n\n> **Note**: You need to change the `TRACE_PORT` depending on your choice of protocol `http`/`grpc`.\n\n### Import order\n\nIt is very important that you do **NOT** import `ddtrace` anywhere before you have initialized troncos! Troncos should give you a warning if this is the case.\n\n### Plain setup\n\n```python\nfrom os import environ\n\nfrom troncos.logs import init_logging_basic\nfrom troncos.traces import init_tracing_basic, http_endpoint_from_env\nfrom troncos.profiling import init_profiling_basic\n\ninit_logging_basic(\n    level=environ.get("LOG_LEVEL", "INFO"),\n    formatter=environ.get("LOG_FORMATTER", "cli")  # Use "logfmt" or "json" in production\n)\ninit_tracing_basic(\n    endpoint=http_endpoint_from_env("TRACE_HOST", "TRACE_PORT", "/v1/traces"),\n    # endpoint_dd=http_endpoint_from_env("TRACE_DD_HOST", "TRACE_DD_PORT"),\n    service_name="my_service",\n    service_version=environ.get("VERSION", "unknown"),\n    service_env=environ.get("ENVIRONMENT", "localdev"),\n)\nprofiler = init_profiling_basic()\n\n# Import all your other stuff ...\n```\n\n### Starlette with uvicorn\n\n```python\nfrom os import environ\n\nfrom troncos.logs import init_logging_basic\nfrom troncos.traces import init_tracing_basic, http_endpoint_from_env\nfrom troncos.profiling import init_profiling_basic\n\ninit_logging_basic(\n    level=environ.get("LOG_LEVEL", "INFO"),\n    formatter=environ.get("LOG_FORMATTER", "cli")  # Use "logfmt" or "json" in production\n)\ninit_tracing_basic(\n    endpoint=http_endpoint_from_env("TRACE_HOST", "TRACE_PORT", "/v1/traces"),\n    # endpoint_dd=http_endpoint_from_env("TRACE_DD_HOST", "TRACE_DD_PORT"),\n    service_name="my_service",\n    service_version=environ.get("VERSION", "unknown"),\n    service_env=environ.get("ENVIRONMENT", "localdev"),\n)\nprofiler = init_profiling_basic()\n\n# Import all your other stuff ...\n\nfrom fastapi import FastAPI\nfrom troncos.frameworks.starlette.uvicorn import init_uvicorn_logging\n\napp = FastAPI(title="my_service")\ninit_uvicorn_logging(\n    app=app,\n    log_access_ignored_paths=["/health", "/metrics"],\n)\n```\n\n> **Note**: If you are running starlette but not calling `init_uvicorn_logging`, traces might not be logged.\n\n### Django\n\nAdd this logging and trace initialization to your `settings.py` file:\n\n```python\nimport environ\nfrom troncos.traces import init_tracing_basic\n\nenv = environ.Env()\n\nAPP_NAME = "my_service"\nVERSION = env.str("VERSION", default="unknown")\nENVIRONMENT = env.str("ENVIRONMENT", default="localhost")\n\n# ... All your settings here ...\n\n# Configure logging\n\nLOG_FORMATTER = env.str("LOG_FORMATTER", "logfmt")\nLOG_LEVEL = env.str("LOG_LEVEL", "INFO")\nLOGGING = {\n    "version": 1,\n    "disable_existing_loggers": True,\n    "filters": {\n        "trace_id": {"()": "troncos.logs.filters.TraceIdFilter"},\n    },\n    "formatters": {\n        "cli": {"()": "troncos.logs.formatters.PrettyFormatter"},\n        "json": {"()": "troncos.logs.formatters.JsonFormatter"},\n        "logfmt": {"()": "troncos.logs.formatters.LogfmtFormatter"},\n    },\n    "handlers": {\n        "console": {\n            "class": "logging.StreamHandler",\n            "formatter": LOG_FORMATTER,\n            "filters": ["trace_id"],\n        }\n    },\n    "loggers": {\n        APP_NAME: {"handlers": ["console"], "level": LOG_LEVEL},\n        "django": {"handlers": ["console"], "level": LOG_LEVEL},\n        "django.server": {\n            "handlers": ["console"],\n            "level": LOG_LEVEL,\n            "propagate": False,\n        },\n        "gunicorn.error": {\n            "handlers": ["console"],\n            "level": LOG_LEVEL,\n        },\n    },\n}\n\n# Configure tracing\n\nTRACING_ENABLED = env.bool("OPENTELEMETRY_TRACING_ENABLED", default=False)\nTRACING_HOST = env.str("OPENTELEMETRY_TRACING_HOST", default="localhost")\nTRACING_PORT = env.int("OPENTELEMETRY_TRACING_PORT", default=4318)\n\ninit_tracing_basic(\n    service_name=APP_NAME,\n    service_version=VERSION,\n    service_env=ENVIRONMENT,\n    endpoint=f"http://{TRACING_HOST}:{TRACING_PORT}/v1/traces"\n    if TRACING_ENABLED\n    else None,\n    # endpoint_dd=f"http://{TRACING_DD_HOST}:{TRACING_DD_PORT}"\n    # if TRACING_DD_ENABLED\n    # else None,\n)\n```\n\n> **Note**: This will not log traces of all incoming requests. See [log traces with Gunicorn](#log-traces-with-gunicorn) section on how to do that.\n\n## Logging\n\n### Thoughts on logging\n\nMore often then not, you want all loggers to propagate their records to the `root` logger and make the `root` logger handle everything. Depending on your project, this might require some additional configuration. Looking at the [python logging flow](https://docs.python.org/3/howto/logging.html#logging-flow) can help you understand how child loggers can propagate records to the `root` logger. Note that propagating to `root` is the default behaviour.\n\nThere is a nice helper function that will print all loggers in troncos called `print_loggers`:\n\n```python\nfrom troncos.logs import print_loggers\n\nprint_loggers(verbose=False)  # To visualize loggers\n```\n\nAfter calling the `init_logging_basic` function in a simple project you should see something like this printed `print_loggers`:\n\n```console\nLoggers:\n[ root                 ] logging.RootLogger LEVEL: 20 PROPAGATE: True\n  └ HANDLER logging.StreamHandler  LEVEL: 20\n    └ FILTER troncos.logs.filters.TraceIdFilter\n    └ FORMATTER troncos.logs.formatters.PrettyFormatter\n```\n\nSo in general, after the initial setup you can use any logger and that will propagate the log record to root:\n\n```python\nimport logging\n\nlogging.getLogger("my.random.logger").info("Root will handle this record")\n```\n\n### Log traces with Gunicorn\n\nCreate a `gunicorn/config.py` file in your project:\n\n```python\nimport time\n\ndef post_fork(server, worker):\n    pass\n\ndef pre_request(worker, req):\n    req._gunicorn_start_time = time.time()\n    worker.log.info("[begin] %s %s", req.method, req.path)\n    pass\n\ndef post_request(worker, req, environ, resp):\n    duration = time.time() - req._gunicorn_start_time\n    trace_id = next(iter([v for k, v in req.headers if k == "X-B3-TRACEID"]), None)\n    worker.log.info(\n        "[status=%s] %s %s duration=%s traceID=%s",\n        resp.status,\n        req.method,\n        req.path,\n        duration,\n        trace_id,\n    )\n```\n\nThen when running gunicorn, specify what config file to use:\n\n```console\ngunicorn myapp.wsgi:application --config python:myapp.gunicorn.config ...\n```\n\n### Structlog\n\nYou can substitute `init_logging_basic` with `init_logging_structlog` to setup structlog:\n\n```python\nfrom os import environ\nfrom troncos.frameworks.structlog.setup import init_logging_structlog\n\ninit_logging_structlog(\n    level=environ.get("LOG_LEVEL", "INFO"),\n    formatter=environ.get("LOG_FORMATTER", "cli"),  # Use "logfmt" in production\n)\n```\n\nAlternatively you can add trace injection into your own structlog setup:\n\n```python\nimport structlog\nfrom troncos.frameworks.structlog.processors import trace_injection_processor\n\nstructlog.configure(\n    processors=[\n       trace_injection_processor,\n    ],\n)\n```\n\n## Tracing\n\n### Tracing your code\n\nAfter initializing tracing in your project you can use different methods to trace your code.\n\n#### trace_function\n\nThis decorator adds tracing to a function. You can supply a tracer provider, if none is supplied, the global tracer provider will be used:\n\n```python\nfrom troncos.traces.decorate import trace_function\n\n@trace_function\ndef myfunc1():\n    return "This will be traced"\n\n@trace_function(service="my_custom_service")\ndef myfunc2():\n    return "This will be traced as my_custom_service"\n```\n\n#### trace_block\n\nTrace using a with statement. You can supply a tracer provider, if none is supplied, the global tracer provider will be used.\n\n```python\nfrom troncos.traces.decorate import trace_block\n\nwith trace_block(name="action", resource="thing", attributes={"some": "attribute"}):\n    print("... do an action to a thing...")\n```\n\n#### trace_class\n\nThis decorator adds a tracing decorator to every method of the decorated class. If you don\'t want some methods to be traced, you can add the [trace_ignore](#traceignore) decorator to them. You can supply a tracer provider, if none is supplied, the global tracer provider will be used:\n\n```python\nfrom troncos.traces.decorate import trace_class, trace_ignore\n\n@trace_class\nclass MyClass1:\n\n    def m1(self):\n        return "This will be traced"\n\n    @trace_ignore\n    def m2(self):\n        return "This will not traced"\n\n\n@trace_class(service="my_custom_service")\nclass MyClass2:\n\n    def m3(self):\n        return "This will be traced as my_custom_service"\n```\n\n#### trace_module\n\nThis function adds a tracing decorator to every function of the calling module. If you don\'t want some functions to be traced, you can add the [trace_ignore](#traceignore) decorator to them. You can supply a tracer provider, if none is supplied, the global tracer provider will be used:\n\n```python\nfrom troncos.traces.decorate import trace_ignore, trace_module\n\ndef my_function():\n    return "This func will be traced"\n\n@trace_ignore\ndef my_function():\n    return "This func will not be traced"\n\ntrace_module()\n```\n\n#### trace_ignore\n\nA decorator that will make [trace_class](#traceclass) and [trace_module](#tracemodule) ignore the decorated function/method.\n\n### Trace Propagation\n\n> **Warning**: Traces with IDs bigger than `64` bits are not propagated correctly because of limitations of [ddtrace](https://github.com/DataDog/dd-trace-py/blob/1e1de001d3fd694d3bcf0fff604a927ef891b19e/ddtrace/propagation/http.py#L102-L108). Default trace ID size for OTEL is `128` bits.\n\nIf you want to propagate your trace to the next service, you need to send/receive special headers with your request/message. If you are using plain `requests` that should be handled automatically by troncos. Here is how you do this manually:\n\n#### Send context\n\n```python\nfrom troncos.traces.propagation import get_propagation_value\n\n# Get header value\nvalue = get_propagation_value()\n\n# Send it somewhere\n```\n\nor\n\n```python\nfrom troncos.traces.propagation import add_context_to_dict\n\nsome_dict = {}\n\n# Add propagation headers to dict\nadd_context_to_dict(some_dict)\n\n# Send it somewhere\n```\n\n#### Receive context\n\nAgain, troncos should in most cases do this automatically for you, but here is how you do it manually:\n\n```python\nfrom troncos.traces.propagation import activate_context_from_dict\nfrom troncos.traces.decorate import trace_block\n\nsome_dict = {} \nactivate_context_from_dict(some_dict)\n\nwith trace_block("my_block"):\n    print("... do something ...")\n```\n\n### Trace sampling\n\nSet these variables to turn on trace sampling:\n\n```console\nOTEL_TRACES_SAMPLER=parentbased_traceidratio\nOTEL_TRACES_SAMPLER_ARG=0.05\nDD_TRACE_SAMPLE_RATE=0.05\n```\n\n### Trace debugging\n\nYou can enable trace debugging by setting the environmental variable `OTEL_TRACE_DEBUG=true`. That will print all spans to the console. If you would rather get the spans in a file you can also provide the variable `OTEL_TRACE_DEBUG_FILE=/tmp/traces`.\n\n## Profiling\n\n> **Warning**: Profiling while using Python 3.11 is [not yet fully supported](https://github.com/DataDog/dd-trace-py/issues/4149).\n\n### Setup endpoint\n\nSimply add a `/debug/pprof` endpoint that returns the profile:\n\n```python\nfrom fastapi import FastAPI\nfrom starlette.responses import Response\nfrom troncos.profiling import init_profiling_basic\n\nprofiler = init_profiling_basic()\n\napp = FastAPI(title="my_service")\n\n@app.get("/debug/pprof", response_model=str)\nasync def debug_pprof() -> Response:\n    content, headers = profiler()\n    return Response(content=content, headers=headers)\n```\n\nYou can verify that your setup works with the [pprof](https://github.com/google/pprof) cli:\n\n```console\n$ pprof -http :6060 "http://localhost:8080/debug/pprof"\n```\n\n> **Note**: You will get an empty string from `profiler()` until the first profile has been collected.\n\n### Enable scraping\n\nWhen you deploy your application, be sure to use the custom oda annotation for scraping:\n\n```yaml\nannotations:\n    phlare.oda.com/port: "8080"\n    phlare.oda.com/scrape: "true"\n```\n\n## Development\n\nWhen developing troncos you should be constantly aware of the fact that under no circumstances should you import `ddtrace` into your module. That would cause the tracer to initialize with default values that would not change when the user initializes the tracer.\n\nFor this reason, if you need to use any parts of `ddtrace` in your code, consider using the `_ddlazy` module, that gives you access lazily. If that does not satisfy your requirements you can always import `ddtrace` in your functions (not at the top of your module).\n\nYou can compare performance of your local version, to some older version of troncos using the [performance test setup](./perf).\n',
     'author': 'Guðmundur Björn Birkisson',
     'author_email': 'gudmundur.birkisson@oda.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/kolonialno/troncos',
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 'troncos._ddlazy', 'troncos.frameworks', 'troncos.frameworks.asgi',
 'troncos.frameworks.gunicorn', 'troncos.frameworks.starlette',
 'troncos.frameworks.structlog', 'troncos.logs', 'troncos.profiling',
 'troncos.traces'] package_data = \ {'': ['*']} install_requires = \
 ['ddtrace==1.8.0', 'opentelemetry-sdk==1.16.0'] extras_require = \ {'grpc':
 ['opentelemetry-exporter-otlp-proto-grpc==1.16.0'], 'http': ['opentelemetry-
 exporter-otlp-proto-http==1.16.0'], 'structlog': ['structlog>=22.3.0,<23.0.0']}
-setup_kwargs = { 'name': 'troncos', 'version': '3.1.1', 'description':
+setup_kwargs = { 'name': 'troncos', 'version': '3.1.2', 'description':
 'Collection of Python logging, tracing and profiling tools',
 'long_description': '
                                 ****** \n ðªµ
                                   \n Troncos
                                    \n ******
 \n\n
      \n \n Collection of Python logging, tracing and profiling tools\n\n
```

### Comparing `troncos-3.1.1/PKG-INFO` & `troncos-3.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: troncos
-Version: 3.1.1
+Version: 3.1.2
 Summary: Collection of Python logging, tracing and profiling tools
 Home-page: https://github.com/kolonialno/troncos
 License: MIT
 Keywords: logs,traces,opentelemetry
 Author: Guðmundur Björn Birkisson
 Author-email: gudmundur.birkisson@oda.com
 Requires-Python: >=3.10,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: troncos Version: 3.1.1 Summary: Collection of
+Metadata-Version: 2.1 Name: troncos Version: 3.1.2 Summary: Collection of
 Python logging, tracing and profiling tools Home-page: https://github.com/
 kolonialno/troncos License: MIT Keywords: logs,traces,opentelemetry Author:
 GuÃ°mundur BjÃ¶rn Birkisson Author-email: gudmundur.birkisson@oda.com Requires-
 Python: >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Provides-Extra: grpc Provides-Extra: http Provides-
 Extra: structlog Requires-Dist: ddtrace (==1.8.0) Requires-Dist: opentelemetry-
```

