# Comparing `tmp/opnieuw-1.2.1.tar.gz` & `tmp/opnieuw-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/opnieuw-1.2.1.tar", last modified: Wed May  3 14:27:41 2023, max compression
+gzip compressed data, was "dist/opnieuw-2.0.0.tar", last modified: Thu May  4 09:03:05 2023, max compression
```

## Comparing `opnieuw-1.2.1.tar` & `opnieuw-2.0.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 semaphore  (1001) semaphore  (1001)        0 2023-05-03 14:27:41.000000 opnieuw-1.2.1/
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     1508 2023-05-03 14:27:39.000000 opnieuw-1.2.1/LICENSE
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     4979 2023-05-03 14:27:41.000000 opnieuw-1.2.1/PKG-INFO
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     4569 2023-05-03 14:27:39.000000 opnieuw-1.2.1/README.md
-drwxrwxr-x   0 semaphore  (1001) semaphore  (1001)        0 2023-05-03 14:27:41.000000 opnieuw-1.2.1/opnieuw/
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)      281 2023-05-03 14:27:39.000000 opnieuw-1.2.1/opnieuw/__init__.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)      802 2023-05-03 14:27:39.000000 opnieuw-1.2.1/opnieuw/clock.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)      298 2023-05-03 14:27:39.000000 opnieuw-1.2.1/opnieuw/exceptions.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)        0 2023-05-03 14:27:39.000000 opnieuw-1.2.1/opnieuw/py.typed
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)    11018 2023-05-03 14:27:39.000000 opnieuw-1.2.1/opnieuw/retries.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)      668 2023-05-03 14:27:39.000000 opnieuw-1.2.1/opnieuw/test_util.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)      586 2023-05-03 14:27:39.000000 opnieuw-1.2.1/opnieuw/util.py
-drwxrwxr-x   0 semaphore  (1001) semaphore  (1001)        0 2023-05-03 14:27:41.000000 opnieuw-1.2.1/opnieuw.egg-info/
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     4979 2023-05-03 14:27:41.000000 opnieuw-1.2.1/opnieuw.egg-info/PKG-INFO
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)      399 2023-05-03 14:27:41.000000 opnieuw-1.2.1/opnieuw.egg-info/SOURCES.txt
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)        1 2023-05-03 14:27:41.000000 opnieuw-1.2.1/opnieuw.egg-info/dependency_links.txt
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)       54 2023-05-03 14:27:41.000000 opnieuw-1.2.1/opnieuw.egg-info/requires.txt
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)        8 2023-05-03 14:27:41.000000 opnieuw-1.2.1/opnieuw.egg-info/top_level.txt
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)       38 2023-05-03 14:27:41.000000 opnieuw-1.2.1/setup.cfg
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     1001 2023-05-03 14:27:39.000000 opnieuw-1.2.1/setup.py
-drwxrwxr-x   0 semaphore  (1001) semaphore  (1001)        0 2023-05-03 14:27:41.000000 opnieuw-1.2.1/tests/
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     8433 2023-05-03 14:27:39.000000 opnieuw-1.2.1/tests/test_context_local.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)      902 2023-05-03 14:27:39.000000 opnieuw-1.2.1/tests/test_exponential_multiplier.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     3316 2023-05-03 14:27:39.000000 opnieuw-1.2.1/tests/test_opnieuw.py
+drwxrwxr-x   0 semaphore  (1001) semaphore  (1001)        0 2023-05-04 09:03:05.000000 opnieuw-2.0.0/
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     1508 2023-05-04 09:03:05.000000 opnieuw-2.0.0/LICENSE
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     4979 2023-05-04 09:03:05.000000 opnieuw-2.0.0/PKG-INFO
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     4569 2023-05-04 09:03:05.000000 opnieuw-2.0.0/README.md
+drwxrwxr-x   0 semaphore  (1001) semaphore  (1001)        0 2023-05-04 09:03:05.000000 opnieuw-2.0.0/opnieuw/
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)      281 2023-05-04 09:03:05.000000 opnieuw-2.0.0/opnieuw/__init__.py
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)      803 2023-05-04 09:03:05.000000 opnieuw-2.0.0/opnieuw/clock.py
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)      298 2023-05-04 09:03:05.000000 opnieuw-2.0.0/opnieuw/exceptions.py
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)        0 2023-05-04 09:03:05.000000 opnieuw-2.0.0/opnieuw/py.typed
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)    11082 2023-05-04 09:03:05.000000 opnieuw-2.0.0/opnieuw/retries.py
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)      738 2023-05-04 09:03:05.000000 opnieuw-2.0.0/opnieuw/test_util.py
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)      656 2023-05-04 09:03:05.000000 opnieuw-2.0.0/opnieuw/util.py
+drwxrwxr-x   0 semaphore  (1001) semaphore  (1001)        0 2023-05-04 09:03:05.000000 opnieuw-2.0.0/opnieuw.egg-info/
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     4979 2023-05-04 09:03:05.000000 opnieuw-2.0.0/opnieuw.egg-info/PKG-INFO
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)      399 2023-05-04 09:03:05.000000 opnieuw-2.0.0/opnieuw.egg-info/SOURCES.txt
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)        1 2023-05-04 09:03:05.000000 opnieuw-2.0.0/opnieuw.egg-info/dependency_links.txt
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)       54 2023-05-04 09:03:05.000000 opnieuw-2.0.0/opnieuw.egg-info/requires.txt
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)        8 2023-05-04 09:03:05.000000 opnieuw-2.0.0/opnieuw.egg-info/top_level.txt
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)       38 2023-05-04 09:03:05.000000 opnieuw-2.0.0/setup.cfg
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     1001 2023-05-04 09:03:05.000000 opnieuw-2.0.0/setup.py
+drwxrwxr-x   0 semaphore  (1001) semaphore  (1001)        0 2023-05-04 09:03:05.000000 opnieuw-2.0.0/tests/
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     8440 2023-05-04 09:03:05.000000 opnieuw-2.0.0/tests/test_context_local.py
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)      902 2023-05-04 09:03:05.000000 opnieuw-2.0.0/tests/test_exponential_multiplier.py
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     3318 2023-05-04 09:03:05.000000 opnieuw-2.0.0/tests/test_opnieuw.py
```

### Comparing `opnieuw-1.2.1/LICENSE` & `opnieuw-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opnieuw-1.2.1/PKG-INFO` & `opnieuw-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opnieuw
-Version: 1.2.1
+Version: 2.0.0
 Summary: Retries for humans
 Home-page: https://github.com/channable/opnieuw
 Author: Channable
 Author-email: ruud@channable.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `opnieuw-1.2.1/README.md` & `opnieuw-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `opnieuw-1.2.1/opnieuw/clock.py` & `opnieuw-2.0.0/opnieuw/clock.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 class MonotonicClock(Clock):
     """Effectual clock for use in production."""
 
     def seconds_since_epoch(self) -> float:
         return time.monotonic()
 
 
-class TestClock(Clock):
+class DummyClock(Clock):
     """Fake clock for use in tests."""
 
     def __init__(self) -> None:
         self.time = 0.0
 
     def advance_to(self, t: float) -> None:
         assert t >= self.time, "Clock should not go backwards"
```

### Comparing `opnieuw-1.2.1/opnieuw/retries.py` & `opnieuw-2.0.0/opnieuw/retries.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import asyncio
 import functools
 import logging
 import random
 import sys
 import time
 from collections import defaultdict
-from collections.abc import Awaitable, Callable, Iterator
+from collections.abc import Callable, Coroutine, Iterator
 from contextlib import contextmanager
 from contextvars import ContextVar
 from typing import NamedTuple, TypeVar, Union
 
 if sys.version_info < (3, 10):
     from typing_extensions import ParamSpec
 else:
@@ -222,25 +222,23 @@
     Opnieuw is based on a retry algorithm off of:
         https://aws.amazon.com/blogs/architecture/exponential-backoff-and-jitter/
     """
 
     def decorator(f: Callable[P, R]) -> Callable[P, R]:
         @functools.wraps(f)
         def wrapper(*args: P.args, **kwargs: P.kwargs) -> R:
-
             last_exception = None
 
             retry_state = _get_retry_state_class(namespace)(
                 MonotonicClock(),
                 max_calls_total=max_calls_total,
                 retry_window_after_first_call_in_seconds=retry_window_after_first_call_in_seconds,
             )
 
             for retry_action in retry_state:
-
                 if isinstance(retry_action, DoCall):
                     try:
                         return f(*args, **kwargs)
 
                     except retry_on_exceptions as e:
                         last_exception = e
 
@@ -275,29 +273,31 @@
 
 def retry_async(
     *,
     retry_on_exceptions: type[Exception] | tuple[type[Exception], ...],
     max_calls_total: int = 3,
     retry_window_after_first_call_in_seconds: int = 60,
     namespace: str | None = None,
-) -> Callable[[Callable[P, Awaitable[R]]], Callable[P, Awaitable[R]]]:
-    def decorator(f: Callable[P, Awaitable[R]]) -> Callable[P, Awaitable[R]]:
+) -> Callable[
+    [Callable[P, Coroutine[None, None, R]]], Callable[P, Coroutine[None, None, R]]
+]:
+    def decorator(
+        f: Callable[P, Coroutine[None, None, R]]
+    ) -> Callable[P, Coroutine[None, None, R]]:
         @functools.wraps(f)
         async def wrapper(*args: P.args, **kwargs: P.kwargs) -> R:
-
             last_exception = None
 
             retry_state = _get_retry_state_class(namespace)(
                 MonotonicClock(),
                 max_calls_total=max_calls_total,
                 retry_window_after_first_call_in_seconds=retry_window_after_first_call_in_seconds,
             )
 
             for retry_action in retry_state:
-
                 if isinstance(retry_action, DoCall):
                     try:
                         return await f(*args, **kwargs)
 
                     except retry_on_exceptions as e:
                         last_exception = e
```

### Comparing `opnieuw-1.2.1/opnieuw/test_util.py` & `opnieuw-2.0.0/opnieuw/util.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-from typing import Iterator, Optional, ContextManager
+from __future__ import annotations
 
-from .retries import DoCall, RetryState, Action, replace_retry_state
+from collections.abc import Iterator
+from contextlib import AbstractContextManager
 
+from .retries import Action, DoCall, RetryState, replace_retry_state
 
-class WaitLessRetryState(RetryState):
+
+class NoRetryState(RetryState):
     def __iter__(self) -> Iterator[Action]:
-        for _ in range(self.max_calls_total):
-            yield DoCall()
+        yield DoCall()
 
 
-def retry_immediately(namespace: Optional[str] = None) -> ContextManager[None]:
+def no_retries(namespace: str | None = None) -> AbstractContextManager[None]:
     """
-    Returns a contextmanager that prevents waits between retries for all `retry` and
+    Returns a contextmanager that disables retries for all `retry` and
     `retry_async` decorators with the provided namespace. None means all decorators
-    without a provided namespace will not wait.
+    without a provided namespace will not retry.
     """
-    return replace_retry_state(WaitLessRetryState, namespace=namespace)
+    return replace_retry_state(NoRetryState, namespace=namespace)
```

### Comparing `opnieuw-1.2.1/opnieuw.egg-info/PKG-INFO` & `opnieuw-2.0.0/opnieuw.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opnieuw
-Version: 1.2.1
+Version: 2.0.0
 Summary: Retries for humans
 Home-page: https://github.com/channable/opnieuw
 Author: Channable
 Author-email: ruud@channable.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `opnieuw-1.2.1/setup.py` & `opnieuw-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Licensed under the 3-clause BSD license, see the LICENSE file in the repository root.
 
 import setuptools  # type: ignore
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-__version__ = "1.2.1"
+__version__ = "2.0.0"
 
 setuptools.setup(
     name="opnieuw",
     version=__version__,
     author="Channable",
     author_email="ruud@channable.com",
     description="Retries for humans",
```

### Comparing `opnieuw-1.2.1/tests/test_context_local.py` & `opnieuw-2.0.0/tests/test_context_local.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
+from __future__ import annotations
+
 import asyncio
 import threading
 import time
-import typing
 import unittest
 from collections import Counter
 
-from opnieuw.retries import retry_async, retry
+from opnieuw.retries import retry, retry_async
 from opnieuw.test_util import retry_immediately
 from opnieuw.util import no_retries
 from tests.utils import AsyncTestCase
 
-
 # The barriers are used to ensure all asyncio tasks/threads have their retry state modified
 # even while the other asyncio tasks/threads are still running.
 # Otherwise, one asyncio task/thread could finish and revert the retry state before the other starts.
 # We want to test the retry state context during concurrency, so the flow should be:
 #
 #        T1         |       T2
 # ------------------|------------------
@@ -40,15 +40,15 @@
         self._current += 1
         if self._current == self.n:
             self.event.set()
         await self.event.wait()
 
 
 class TestAsyncContext(AsyncTestCase):
-    counter: typing.Counter[str] = Counter()
+    counter: Counter[str] = Counter()
 
     MAX_TOTAL_CALLS = 3
 
     @retry_async(
         retry_on_exceptions=TypeError,
         max_calls_total=MAX_TOTAL_CALLS,
         retry_window_after_first_call_in_seconds=3,
@@ -172,15 +172,15 @@
                 ("no_retry_with_nested_retry_immediately", 1),
             ]
 
         self._run_async(_test_inner())
 
 
 class TestThreadedContext(unittest.TestCase):
-    counter: typing.Counter[str] = Counter()
+    counter: Counter[str] = Counter()
 
     @retry(
         retry_on_exceptions=TypeError,
         max_calls_total=3,
         retry_window_after_first_call_in_seconds=3,
     )
     def foo(self, counter_key: str) -> None:
```

### Comparing `opnieuw-1.2.1/tests/test_exponential_multiplier.py` & `opnieuw-2.0.0/tests/test_exponential_multiplier.py`

 * *Files identical despite different names*

### Comparing `opnieuw-1.2.1/tests/test_opnieuw.py` & `opnieuw-2.0.0/tests/test_opnieuw.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 # Copyright 2019 Channable
 #
 # Licensed under the 3-clause BSD license, see the LICENSE file in the repository root.
 
 import time
 import unittest
 
-from opnieuw.clock import TestClock, MonotonicClock
-from opnieuw.retries import RetryState, DoCall, retry
+from opnieuw.clock import DummyClock, MonotonicClock
+from opnieuw.retries import DoCall, RetryState, retry
 from opnieuw.test_util import retry_immediately
 
 
 class TestRetryState(unittest.TestCase):
     def test_never_stop(self) -> None:
         retry_state = RetryState(
             MonotonicClock(),
@@ -21,15 +21,15 @@
 
         for rt in retry_state:
             self.assertIsInstance(rt, DoCall)
 
 
 class TestRetryClock(unittest.TestCase):
     def setUp(self) -> None:
-        self.clock = TestClock()
+        self.clock = DummyClock()
 
     def test_negative_time_value(self) -> None:
         try:
             self.clock.advance_to(-60.00)
         except Exception as e:
             self.assertIsInstance(e, AssertionError)
             self.assertEqual(self.clock.time, 0.0)
```

