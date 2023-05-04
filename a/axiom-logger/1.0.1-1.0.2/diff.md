# Comparing `tmp/axiom_logger-1.0.1.tar.gz` & `tmp/axiom_logger-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "axiom_logger-1.0.1.tar", last modified: Wed May  3 16:30:46 2023, max compression
+gzip compressed data, was "axiom_logger-1.0.2.tar", last modified: Thu May  4 10:46:15 2023, max compression
```

## Comparing `axiom_logger-1.0.1.tar` & `axiom_logger-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 16:30:46.223649 axiom_logger-1.0.1/
--rw-rw-rw-   0        0        0     1084 2023-05-03 14:11:55.000000 axiom_logger-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     1552 2023-05-03 16:30:46.223649 axiom_logger-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1009 2023-05-03 16:30:26.000000 axiom_logger-1.0.1/README.md
--rw-rw-rw-   0        0        0      637 2023-05-03 16:30:26.000000 axiom_logger-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-03 16:30:46.223649 axiom_logger-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-03 16:30:46.208017 axiom_logger-1.0.1/src/
--rw-rw-rw-   0        0        0        0 2023-05-03 14:11:25.000000 axiom_logger-1.0.1/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 16:30:46.223649 axiom_logger-1.0.1/src/axiom_logger.egg-info/
--rw-rw-rw-   0        0        0     1552 2023-05-03 16:30:46.000000 axiom_logger-1.0.1/src/axiom_logger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      228 2023-05-03 16:30:46.000000 axiom_logger-1.0.1/src/axiom_logger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 16:30:46.000000 axiom_logger-1.0.1/src/axiom_logger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-05-03 16:30:46.000000 axiom_logger-1.0.1/src/axiom_logger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3768 2023-05-03 16:13:21.000000 axiom_logger-1.0.1/src/axiom_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:46:15.913614 axiom_logger-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-04 10:45:58.000000 axiom_logger-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-05-04 10:46:15.913614 axiom_logger-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-05-04 10:45:58.000000 axiom_logger-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-04 10:45:58.000000 axiom_logger-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 10:46:15.913614 axiom_logger-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:46:15.913614 axiom_logger-1.0.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:45:58.000000 axiom_logger-1.0.2/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:46:15.913614 axiom_logger-1.0.2/src/axiom_logger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-05-04 10:46:15.000000 axiom_logger-1.0.2/src/axiom_logger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-04 10:46:15.000000 axiom_logger-1.0.2/src/axiom_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 10:46:15.000000 axiom_logger-1.0.2/src/axiom_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 10:46:15.000000 axiom_logger-1.0.2/src/axiom_logger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-05-04 10:45:58.000000 axiom_logger-1.0.2/src/axiom_logger.py
```

### Comparing `axiom_logger-1.0.1/pyproject.toml` & `axiom_logger-1.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-[build-system]
-requires = ["setuptools>=61.0", "requests"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "axiom_logger"
-version = "1.0.1"
-authors = [
-  { name="Stefano Maddè", email="sm@spforniture.it" },
-]
-description = "Python logging handler for the Axiom service"
-readme = "README.md"
-requires-python = ">=3.7"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-
-[project.urls]
-"Homepage" = "https://github.com/stemadde/axiom_logger"
-"Bug Tracker" = "https://github.com/stemadde/axiom_logger/issues"
+[build-system]
+requires = ["setuptools>=61.0", "requests"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "axiom_logger"
+version = "1.0.2"
+authors = [
+  { name="Stefano Maddè", email="sm@spforniture.it" },
+]
+description = "Python logging handler for the Axiom service"
+readme = "README.md"
+requires-python = ">=3.7"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+
+[project.urls]
+"Homepage" = "https://github.com/stemadde/axiom_logger"
+"Bug Tracker" = "https://github.com/stemadde/axiom_logger/issues"
```

### Comparing `axiom_logger-1.0.1/src/axiom_logger.py` & `axiom_logger-1.0.2/src/axiom_logger.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,103 +1,117 @@
-import atexit
-import threading
-import time
-import requests
-from logging import LogRecord, Formatter, Handler
-from typing import Literal
-from requests.adapters import HTTPAdapter, Retry
-
-AXIOM_V1 = 'https://api.axiom.co/v1/datasets'
-_defaultFormatter = Formatter()
-
-
-class AxiomHandler(Handler):
-    def __init__(
-            self,
-            dataset: str,
-            api_token: str,
-            api_url=AXIOM_V1,
-            mode: Literal['elapsed_time', 'log_count'] = 'elapsed_time',
-            elapsed_time: int = 10,
-            log_count: int = 5,
-    ):
-        """
-        :param dataset: Name of the remote dataset to log to
-        :param api_token: API token used for authentication against the Axiom remote service
-        :param api_url: Override this value if you are using a different version of the Axiom API
-        :param mode: Defaults to "elapsed_time" which will send logs every elapsed_time seconds.
-        Can be changed to "log_count" which will send logs every log_count sent logs.
-        :param elapsed_time: Time in seconds to wait before sending logs. Only used if mode is "elapsed_time"
-        :param log_count: Count of logs to wait before sending logs. Only used if mode is "log_count"
-        """
-        # Assertion checks
-        assert api_token, 'api_token is required for AXIOM logging'
-        assert dataset, 'a dataset name is required for AXIOM logging'
-        if mode == 'elapsed_time' and not elapsed_time:
-            raise AssertionError('elapsed_time is required for mode elapsed_time')
-        if mode == 'log_count' and not log_count:
-            raise AssertionError('log_count is required for mode log_count')
-
-        # Sets up the handler
-        self.endpoint = f'{api_url}/{dataset}/ingest'
-        self.api_token = api_token
-        self.MAX_POOLSIZE = 100
-        self.session = session = requests.Session()
-        session.headers.update({
-            'Content-Type': 'application/json',
-            'Authorization': 'Bearer %s' % self.api_token
-        })
-        self.session.mount('https://', HTTPAdapter(
-            max_retries=Retry(
-                total=5,
-                backoff_factor=0.5,
-                status_forcelist=[403, 500]
-            ),
-            pool_connections=self.MAX_POOLSIZE,
-            pool_maxsize=self.MAX_POOLSIZE
-        ))
-
-        # Sets up the mode
-        self.record_pool = []
-        self.mode = mode
-        self.elapsed_time = elapsed_time
-        self.log_count = log_count
-        self.is_sending = False
-
-        if self.mode == 'elapsed_time':
-            self.timer = None
-
-        atexit.register(self.send)
-        super().__init__()
-
-    def emit(self, record: LogRecord) -> None:
-        while True:
-            if self.is_sending:
-                time.sleep(0.2)
-                continue
-            break
-
-        log_entry = self.axiom_format(record)
-        self.record_pool.append(log_entry)
-
-        if self.mode == 'log_count':
-            if len(self.record_pool) >= self.log_count:
-                self.send()
-        else:
-            if not self.timer or not self.timer.is_alive():
-                self.timer = threading.Timer(self.elapsed_time, self.send)
-                self.timer.start()
-
-    def axiom_format(self, record: LogRecord) -> dict:
-        return {
-            "_time": record.created,
-            "data": record.getMessage(),
-        }
-
-    def send(self) -> None:
-        if not self.record_pool:
-            return
-        self.is_sending = True
-        res = self.session.post(self.endpoint, json=self.record_pool)
-        if res.status_code == 200:
-            self.record_pool = []
-        self.is_sending = False
+import atexit
+import threading
+import time
+import warnings
+from datetime import datetime
+import requests
+from logging import LogRecord, Formatter, Handler
+from typing import Literal
+from requests.adapters import HTTPAdapter, Retry
+
+AXIOM_V1 = 'https://api.axiom.co/v1/datasets'
+_defaultFormatter = Formatter()
+
+
+class AxiomHandler(Handler):
+    def __init__(
+            self,
+            dataset: str,
+            api_token: str,
+            api_url=AXIOM_V1,
+            mode: Literal['elapsed_time', 'log_count'] = 'elapsed_time',
+            elapsed_time: float = 10,
+            log_count: int = 5
+    ):
+        """
+        :param dataset: Name of the remote dataset to log to
+        :param api_token: API token used for authentication against the Axiom remote service
+        :param api_url: Override this value if you are using a different version of the Axiom API
+        :param mode: Defaults to "elapsed_time" which will send logs every elapsed_time seconds.
+            Can be changed to "log_count" which will send logs every log_count sent logs.
+        :param elapsed_time: Time in seconds to wait before sending logs. Only used if mode is "elapsed_time"
+        :param log_count: Count of logs to wait before sending logs. Only used if mode is "log_count"
+        """
+        # Assertion checks
+        assert api_token, 'api_token is required for AXIOM logging'
+        assert dataset, 'a dataset name is required for AXIOM logging'
+        if mode == 'elapsed_time' and not elapsed_time:
+            raise AssertionError('elapsed_time is required for mode elapsed_time')
+        if mode == 'log_count' and not log_count:
+            raise AssertionError('log_count is required for mode log_count')
+
+        # Sets up the handler
+        self.endpoint = f'{api_url}/{dataset}/ingest'
+        self.api_token = api_token
+        self.MAX_POOLSIZE = 100
+        self.session = session = requests.Session()
+        session.headers.update({
+            'Content-Type': 'application/json',
+            'Authorization': 'Bearer %s' % self.api_token
+        })
+        self.session.mount('https://', HTTPAdapter(
+            max_retries=Retry(
+                total=5,
+                backoff_factor=0.5,
+                status_forcelist=[403, 500]
+            ),
+            pool_connections=self.MAX_POOLSIZE,
+            pool_maxsize=self.MAX_POOLSIZE
+        ))
+
+        # Sets up the mode
+        self.record_pool = []
+        self.mode = mode
+        self.elapsed_time = elapsed_time
+        self.log_count = log_count
+        self.is_sending = False
+
+        if self.mode == 'elapsed_time':
+            self.timer = None
+
+        atexit.register(self.send)
+        super().__init__()
+
+    def emit(self, record: LogRecord) -> None:
+        while True:
+            if self.is_sending:
+                time.sleep(0.2)
+                continue
+            break
+
+        log_entry = self.axiom_format(record)
+        self.record_pool.append(log_entry)
+
+        if self.mode == 'log_count':
+            if len(self.record_pool) >= self.log_count:
+                self.send()
+        else:
+            if not self.timer or not self.timer.is_alive():
+                self.timer = threading.Timer(self.elapsed_time, self.send)
+                self.timer.start()
+
+    def axiom_format(self, record: LogRecord) -> dict:
+        return {
+            "_time": record.created,
+            "data": record.getMessage(),
+        }
+
+    def send(self) -> None:
+        if not self.record_pool:
+            return
+        self.is_sending = True
+        res = self.session.post(self.endpoint, json=self.record_pool)
+        if not res.status_code == 200:
+            not_logged_records = '\n'.join(
+                f"{datetime.fromtimestamp(record['_time'])} -> {record['data']}" for record in self.record_pool
+            )
+            warnings.warn(
+                f'Failed to send logs to Axiom.\n'
+                f'Status code: {res.status_code}\n'
+                f'Response: {res.text}\n'
+                f'==== Begin of unsent records ===='
+                f'\n{not_logged_records}\n'
+                f'==== End of unsent records ====',
+                RuntimeWarning
+            )
+        self.record_pool = []
+        self.is_sending = False
```

