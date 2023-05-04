# Comparing `tmp/async_etcd3gw-0.5.tar.gz` & `tmp/async_etcd3gw-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_etcd3gw-0.5.tar", last modified: Wed May  3 06:51:57 2023, max compression
+gzip compressed data, was "async_etcd3gw-0.6.tar", last modified: Thu May  4 08:01:52 2023, max compression
```

## Comparing `async_etcd3gw-0.5.tar` & `async_etcd3gw-0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:51:57.423133 async_etcd3gw-0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-03 06:51:30.000000 async_etcd3gw-0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-05-03 06:51:57.423133 async_etcd3gw-0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-03 06:51:30.000000 async_etcd3gw-0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:51:57.419133 async_etcd3gw-0.5/async_etcd3gw/
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-03 06:51:30.000000 async_etcd3gw-0.5/async_etcd3gw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20705 2023-05-03 06:51:30.000000 async_etcd3gw-0.5/async_etcd3gw/async_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-05-03 06:51:30.000000 async_etcd3gw-0.5/async_etcd3gw/async_lease.py
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-05-03 06:51:30.000000 async_etcd3gw-0.5/async_etcd3gw/async_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-05-03 06:51:30.000000 async_etcd3gw-0.5/async_etcd3gw/async_watch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-03 06:51:30.000000 async_etcd3gw-0.5/async_etcd3gw/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-03 06:51:30.000000 async_etcd3gw-0.5/async_etcd3gw/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:51:57.423133 async_etcd3gw-0.5/async_etcd3gw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-05-03 06:51:57.000000 async_etcd3gw-0.5/async_etcd3gw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-03 06:51:57.000000 async_etcd3gw-0.5/async_etcd3gw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 06:51:57.000000 async_etcd3gw-0.5/async_etcd3gw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-03 06:51:57.000000 async_etcd3gw-0.5/async_etcd3gw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-03 06:51:57.000000 async_etcd3gw-0.5/async_etcd3gw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 06:51:57.000000 async_etcd3gw-0.5/async_etcd3gw.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-03 06:51:30.000000 async_etcd3gw-0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-03 06:51:57.423133 async_etcd3gw-0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-03 06:51:30.000000 async_etcd3gw-0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:51:57.423133 async_etcd3gw-0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    13511 2023-05-03 06:51:30.000000 async_etcd3gw-0.5/tests/test_async_etcd3gw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-03 06:51:30.000000 async_etcd3gw-0.5/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:01:52.679927 async_etcd3gw-0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-04 08:01:22.000000 async_etcd3gw-0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-05-04 08:01:52.679927 async_etcd3gw-0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-04 08:01:22.000000 async_etcd3gw-0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:01:52.675927 async_etcd3gw-0.6/async_etcd3gw/
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-04 08:01:22.000000 async_etcd3gw-0.6/async_etcd3gw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21099 2023-05-04 08:01:22.000000 async_etcd3gw-0.6/async_etcd3gw/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-05-04 08:01:22.000000 async_etcd3gw-0.6/async_etcd3gw/async_lease.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-05-04 08:01:22.000000 async_etcd3gw-0.6/async_etcd3gw/async_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-05-04 08:01:22.000000 async_etcd3gw-0.6/async_etcd3gw/async_watch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-04 08:01:22.000000 async_etcd3gw-0.6/async_etcd3gw/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-04 08:01:22.000000 async_etcd3gw-0.6/async_etcd3gw/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:01:52.679927 async_etcd3gw-0.6/async_etcd3gw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-05-04 08:01:52.000000 async_etcd3gw-0.6/async_etcd3gw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-04 08:01:52.000000 async_etcd3gw-0.6/async_etcd3gw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 08:01:52.000000 async_etcd3gw-0.6/async_etcd3gw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-04 08:01:52.000000 async_etcd3gw-0.6/async_etcd3gw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-04 08:01:52.000000 async_etcd3gw-0.6/async_etcd3gw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 08:01:52.000000 async_etcd3gw-0.6/async_etcd3gw.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-04 08:01:22.000000 async_etcd3gw-0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-04 08:01:52.679927 async_etcd3gw-0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-04 08:01:22.000000 async_etcd3gw-0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:01:52.679927 async_etcd3gw-0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    14019 2023-05-04 08:01:22.000000 async_etcd3gw-0.6/tests/test_async_etcd3gw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-04 08:01:22.000000 async_etcd3gw-0.6/tests/test_client.py
```

### Comparing `async_etcd3gw-0.5/LICENSE` & `async_etcd3gw-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `async_etcd3gw-0.5/PKG-INFO` & `async_etcd3gw-0.6/async_etcd3gw.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: async_etcd3gw
-Version: 0.5
+Name: async-etcd3gw
+Version: 0.6
 Summary: An async Python client for etcd3 grpc-gateway v3 API
 Home-page: https://github.com/DLBD-Department/async_etcd3gw
 Author: Alkemy spa
 Author-email: DLBDDepartment@alkemy.com
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/DLBD-Department/async_etcd3gw/issues
 Project-URL: Source Code, https://github.com/DLBD-Department/async_etcd3gw
@@ -48,35 +48,38 @@
 Basic usage example:
 
 ```python
 import asyncio
 from async_etcd3gw import AsyncEtcd3Client
 
 async def main():
-    client = AsyncEtcd3Client(host='etcd', port=2379)
+    client = AsyncEtcd3Client(host="etcd", port=2379)
 
     # Put key
-    await client.put(key='foo', value='bar')
+    await client.put(key="foo", value="bar")
 
     # Get key
-    print("get key foo", await client.get(key='foo'))
+    print("get key foo", await client.get(key="foo"))
 
     # Get all keys
     print("get all keys", await client.get_all())
 
     # Create lease and use it
     lease = await client.lease(ttl=100)
-    await client.put(key='foo', value='bar', lease=lease)
+    await client.put(key="foo", value="bar", lease=lease)
 
     # Get lease keys
     print("get lease keys", await lease.keys())
 
     # Refresh lease
     await lease.refresh()
 
+    # Release all acquired resources
+    await client.close()
+
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
 ### Links
 
 * [etcd](https://etcd.io)
```

### Comparing `async_etcd3gw-0.5/README.md` & `async_etcd3gw-0.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -20,35 +20,38 @@
 Basic usage example:
 
 ```python
 import asyncio
 from async_etcd3gw import AsyncEtcd3Client
 
 async def main():
-    client = AsyncEtcd3Client(host='etcd', port=2379)
+    client = AsyncEtcd3Client(host="etcd", port=2379)
 
     # Put key
-    await client.put(key='foo', value='bar')
+    await client.put(key="foo", value="bar")
 
     # Get key
-    print("get key foo", await client.get(key='foo'))
+    print("get key foo", await client.get(key="foo"))
 
     # Get all keys
     print("get all keys", await client.get_all())
 
     # Create lease and use it
     lease = await client.lease(ttl=100)
-    await client.put(key='foo', value='bar', lease=lease)
+    await client.put(key="foo", value="bar", lease=lease)
 
     # Get lease keys
     print("get lease keys", await lease.keys())
 
     # Refresh lease
     await lease.refresh()
 
+    # Release all acquired resources
+    await client.close()
+
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
 ### Links
 
 * [etcd](https://etcd.io)
```

### Comparing `async_etcd3gw-0.5/async_etcd3gw/__init__.py` & `async_etcd3gw-0.6/async_etcd3gw/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 #    https://opendev.org/openstack/etcd3gw/src/tag/2.1.0/etcd3gw/__init__.py
 
 from . import utils
 from .async_client import AsyncEtcd3Client, async_client
 from .async_lease import AsyncLease
 from .async_lock import AsyncLock
 
-__version__ = "0.5"
+__version__ = "0.6"
 
 __all__ = (
     "AsyncEtcd3Client",
     "AsyncLease",
     "AsyncLock",
     "async_client",
     "utils",
```

### Comparing `async_etcd3gw-0.5/async_etcd3gw/async_client.py` & `async_etcd3gw-0.6/async_etcd3gw/async_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,20 @@
 import uuid
 
 import aiohttp
 
 from .async_lease import AsyncLease
 from .async_lock import AsyncLock
 from .async_watch import AsyncWatcher
-from .exceptions import _EXCEPTIONS_BY_CODE, AsyncEtcd3Exception, ConnectionFailedError, ConnectionTimeoutError, WatchTimedOut
+from .exceptions import (
+    ConnectionFailedError,
+    ConnectionTimeoutError,
+    WatchTimedOut,
+    get_exception,
+)
 from .utils import DEFAULT_TIMEOUT, _decode, _encode, _increment_last_byte
 
 __all__ = [
     "AsyncEtcd3Client",
     "async_client",
     "DEFAULT_API_PATH",
     "DEFAULT_PORT",
@@ -96,14 +101,16 @@
 
         self.client_session_kwargs = {}
         if self.timeout is not None:
             self.client_session_kwargs["timeout"] = self.timeout
         if self.connector is not None:
             self.client_session_kwargs["connector"] = self.connector
 
+        self.session = aiohttp.ClientSession(**self.client_session_kwargs)
+
     def get_url(self, path):
         """Construct a full url to the v3 API given a specific path
 
         This method takes a path as an argument and returns a url that points to the v3 API of the host.
 
         Args:
             path (str): The path to append to the base url.
@@ -137,21 +144,19 @@
 
         Raises:
             AsyncEtcd3Exception: If the status code is not 200 and not in the predefined exceptions.
             ConnectionTimeoutError: If the request times out.
             ConnectionFailedError: If the connection fails.
         """
         try:
-            async with aiohttp.ClientSession(**self.client_session_kwargs) as session:
-                async with session.post(*args, **kwargs) as resp:
-                    if resp.status in _EXCEPTIONS_BY_CODE:
-                        raise _EXCEPTIONS_BY_CODE[resp.status](resp.text, resp.reason)
-                    if resp.status != 200:
-                        raise AsyncEtcd3Exception(resp.text, resp.reason)
-                    return await resp.json()
+            async with self.session.post(*args, **kwargs) as resp:
+                ex = get_exception(resp.status, resp.text, resp.reason)
+                if ex is not None:
+                    raise ex
+                return await resp.json()
         except asyncio.TimeoutError as ex:
             raise ConnectionTimeoutError(str(ex))
         except aiohttp.ClientConnectionError as ex:
             raise ConnectionFailedError(str(ex))
 
     async def status(self):
         """Status gets the status of the etcd cluster member.
@@ -508,14 +513,17 @@
             canceled.set()
             await event_queue.put(None)
             await w.stop()
 
         async def iterator():
             while not canceled.is_set():
                 event = await event_queue.get()
+                if isinstance(event, Exception):
+                    canceled.set()
+                    raise event
                 if event is None:
                     canceled.set()
                 if not canceled.is_set():
                     yield event
 
         return iterator(), cancel
 
@@ -553,14 +561,26 @@
             await w.stop()
 
     async def watch_prefix_once(self, key_prefix, timeout=None, **kwargs):
         """Watches a range of keys with a prefix, similar to watch_once"""
         kwargs["range_end"] = _increment_last_byte(key_prefix)
         return await self.watch_once(key_prefix, timeout=timeout, **kwargs)
 
+    async def close(self):
+        """Close the underlying connector and release all acquired resources."""
+        return await self.session.close()
+
+    async def __aenter__(self):
+        """Use the AsyncEtcd3Client as a contextmanager"""
+        return self
+
+    async def __aexit__(self, exception_type, exception_value, traceback):
+        """Use the AsyncEtcd3Client as a contextmanager"""
+        await self.close()
+
 
 def async_client(
     host="localhost",
     port=2379,
     ca_cert=None,
     cert_key=None,
     cert_cert=None,
```

### Comparing `async_etcd3gw-0.5/async_etcd3gw/async_lease.py` & `async_etcd3gw-0.6/async_etcd3gw/async_lease.py`

 * *Files identical despite different names*

### Comparing `async_etcd3gw-0.5/async_etcd3gw/async_lock.py` & `async_etcd3gw-0.6/async_etcd3gw/async_lock.py`

 * *Files identical despite different names*

### Comparing `async_etcd3gw-0.5/async_etcd3gw/async_watch.py` & `async_etcd3gw-0.6/async_etcd3gw/async_watch.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 #    https://opendev.org/openstack/etcd3gw/src/tag/2.1.0/etcd3gw/watch.py
 
 import asyncio
 import json
 
 import aiohttp
 
+from .exceptions import get_exception
 from .utils import _decode, _encode
 
 __all__ = ["AsyncWatcher"]
 
 
 class AsyncWatcher(object):
     KW_ARGS = ["start_revision", "progress_notify", "filters", "prev_kv"]
@@ -36,15 +37,20 @@
                 create_watch[arg] = kwargs[arg]
             elif arg in self.KW_ENCODED_ARGS:
                 create_watch[arg] = _encode(kwargs[arg])
         self.create_request = {"create_request": create_watch}
 
     async def start(self):
         "Start the watch task"
+        self.event = asyncio.Event()
+        self.exception = None
         self.watch_task = asyncio.create_task(self.watch())
+        await self.event.wait()
+        if self.exception is not None:
+            raise self.exception
 
     async def stop(self):
         "Request the watch task to be cancelled"
         self.watch_task.cancel()
         try:
             await self.watch_task
         except asyncio.CancelledError:
@@ -53,39 +59,47 @@
     async def process_chunk(self, line):
         "Process a chuck"
         decoded_line = line.decode("utf-8")
         try:
             payload = json.loads(decoded_line)
         except Exception as ex:
             raise ex
+        if "error" in payload:
+            raise get_exception(
+                payload["error"].get("http_code", 500), payload["error"].get("http_status", ""), payload["error"].get("message", "")
+            )
         if "created" in payload["result"]:
             if not payload["result"]["created"]:
                 raise Exception("Unable to create watch")
         if "events" in payload["result"]:
             for event in payload["result"]["events"]:
                 event["kv"]["key"] = _decode(event["kv"]["key"])
                 if "value" in event["kv"]:
                     event["kv"]["value"] = _decode(event["kv"]["value"])
                 await self.callback(event)
 
-    async def watch(self):
-        try:
-            # Set timeout
-            kwargs = dict(self.async_client.client_session_kwargs)
-            timeout = aiohttp.ClientTimeout(total=None, sock_read=None)
-            kwargs["timeout"] = timeout
-            async with aiohttp.ClientSession(**kwargs) as session:
-                async with session.post(self.async_client.get_url("/watch"), json=self.create_request) as resp:
-                    await self.read_and_process_chunk(resp.content)
-        except Exception:
-            await self.callback(None)
-
     async def read_and_process_chunk(self, content):
         while True:
             if content._exception is not None:
                 raise content._exception
 
             if not content._buffer and not content._eof:
                 await content._wait("readany")
 
             data = content._read_nowait(-1)
             await self.process_chunk(data)
+
+    async def watch(self):
+        try:
+            timeout = aiohttp.ClientTimeout(total=None, sock_read=None)
+            async with self.async_client.session.post(
+                self.async_client.get_url("/watch"), json=self.create_request, timeout=timeout
+            ) as resp:
+                ex = get_exception(resp.status, resp.text, resp.reason)
+                if ex:
+                    raise ex
+                self.event.set()
+                await self.read_and_process_chunk(resp.content)
+        except Exception as ex:
+            self.exception = ex
+            self.event.set()
+            await self.callback(ex)
```

### Comparing `async_etcd3gw-0.5/async_etcd3gw/exceptions.py` & `async_etcd3gw-0.6/async_etcd3gw/exceptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 #    License for the specific language governing permissions and limitations
 #    under the License.
 #
 #    Derived from:
 #    https://opendev.org/openstack/etcd3gw/src/tag/2.1.0/etcd3gw/exceptions.py
 
 __all__ = [
+    "get_exception",
     "AsyncEtcd3Exception",
     "WatchTimedOut",
     "InternalServerError",
     "ConnectionFailedError",
     "ConnectionTimeoutError",
     "PreconditionFailedError",
     "_EXCEPTIONS_BY_CODE",
@@ -53,7 +54,15 @@
 _EXCEPTIONS_BY_CODE = {
     500: InternalServerError,
     503: ConnectionFailedError,
     408: ConnectionTimeoutError,
     504: ConnectionTimeoutError,
     412: PreconditionFailedError,
 }
+
+
+def get_exception(status, text, reason):
+    if status in _EXCEPTIONS_BY_CODE:
+        return _EXCEPTIONS_BY_CODE[status](text, reason)
+    if status != 200:
+        return AsyncEtcd3Exception(text, reason)
+    return None
```

### Comparing `async_etcd3gw-0.5/async_etcd3gw/utils.py` & `async_etcd3gw-0.6/async_etcd3gw/utils.py`

 * *Files identical despite different names*

### Comparing `async_etcd3gw-0.5/async_etcd3gw.egg-info/PKG-INFO` & `async_etcd3gw-0.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: async-etcd3gw
-Version: 0.5
+Name: async_etcd3gw
+Version: 0.6
 Summary: An async Python client for etcd3 grpc-gateway v3 API
 Home-page: https://github.com/DLBD-Department/async_etcd3gw
 Author: Alkemy spa
 Author-email: DLBDDepartment@alkemy.com
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/DLBD-Department/async_etcd3gw/issues
 Project-URL: Source Code, https://github.com/DLBD-Department/async_etcd3gw
@@ -48,35 +48,38 @@
 Basic usage example:
 
 ```python
 import asyncio
 from async_etcd3gw import AsyncEtcd3Client
 
 async def main():
-    client = AsyncEtcd3Client(host='etcd', port=2379)
+    client = AsyncEtcd3Client(host="etcd", port=2379)
 
     # Put key
-    await client.put(key='foo', value='bar')
+    await client.put(key="foo", value="bar")
 
     # Get key
-    print("get key foo", await client.get(key='foo'))
+    print("get key foo", await client.get(key="foo"))
 
     # Get all keys
     print("get all keys", await client.get_all())
 
     # Create lease and use it
     lease = await client.lease(ttl=100)
-    await client.put(key='foo', value='bar', lease=lease)
+    await client.put(key="foo", value="bar", lease=lease)
 
     # Get lease keys
     print("get lease keys", await lease.keys())
 
     # Refresh lease
     await lease.refresh()
 
+    # Release all acquired resources
+    await client.close()
+
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
 ### Links
 
 * [etcd](https://etcd.io)
```

### Comparing `async_etcd3gw-0.5/setup.cfg` & `async_etcd3gw-0.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `async_etcd3gw-0.5/tests/test_async_etcd3gw.py` & `async_etcd3gw-0.6/tests/test_async_etcd3gw.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,40 +13,41 @@
 import asyncio
 import os
 import uuid
 from time import perf_counter
 
 import pytest
 
-from async_etcd3gw import exceptions, utils, AsyncEtcd3Client
+from async_etcd3gw import AsyncEtcd3Client, exceptions, utils
 from async_etcd3gw.async_client import DEFAULT_API_PATH
 
 ETCD_HOST = os.environ.get("ETCD_HOST", "localhost")
 API_PATH = os.environ.get("API_PATH", DEFAULT_API_PATH)
 
 
 @pytest.mark.etcd
 @pytest.mark.asyncio
 async def test_client_status():
-    client = AsyncEtcd3Client(host=ETCD_HOST, api_path=API_PATH)
-    response = await client.status()
-    assert response is not None
-    assert "version" in response
-    assert "header" in response
-    assert "cluster_id" in response["header"]
+    async with AsyncEtcd3Client(host=ETCD_HOST, api_path=API_PATH) as client:
+        response = await client.status()
+        assert response is not None
+        assert "version" in response
+        assert "header" in response
+        assert "cluster_id" in response["header"]
 
 
 @pytest.mark.etcd
 @pytest.mark.asyncio
 async def test_client_members():
     client = AsyncEtcd3Client(host=ETCD_HOST, api_path=API_PATH)
     response = await client.members()
     assert len(response) > 0
     assert "clientURLs" in response[0]
     assert "peerURLs" in response[0]
+    await client.close()
 
 
 @pytest.mark.etcd
 @pytest.mark.asyncio
 async def test_client_with_keys_and_values():
     client = AsyncEtcd3Client(host=ETCD_HOST, api_path=API_PATH)
     assert await client.put("foo0", "bar0")
@@ -58,14 +59,15 @@
     assert [b"bar2"] == await client.get("foo2")
 
     assert await client.delete("foo0")
     assert [] == await client.get("foo0")
 
     assert not await client.delete("foo0")
     assert len(await client.get_all()) > 0
+    await client.close()
 
 
 @pytest.mark.etcd
 @pytest.mark.asyncio
 async def test_get_and_delete_prefix():
     client = AsyncEtcd3Client(host=ETCD_HOST, api_path=API_PATH)
     for i in range(20):
@@ -76,14 +78,15 @@
     for value, metadata in values:
         assert b"i am a range" == value
         assert metadata["key"].startswith(b"/doot1/range")
 
     assert await client.delete_prefix("/doot1/range")
     values = list(await client.get_prefix("/doot1/range"))
     assert len(values) == 0
+    await client.close()
 
 
 @pytest.mark.etcd
 @pytest.mark.asyncio
 async def test_get_prefix_sort_order():
     client = AsyncEtcd3Client(host=ETCD_HOST, api_path=API_PATH)
 
@@ -103,14 +106,15 @@
     assert keys == initial_keys.encode("latin-1")
 
     reverse_keys = b""
     for value, meta in await client.get_prefix("/doot2", sort_order="descend"):
         reverse_keys += remove_prefix(meta["key"], "/doot2/")
 
     assert reverse_keys == "".join(reversed(initial_keys)).encode("latin-1")
+    await client.close()
 
 
 @pytest.mark.etcd
 @pytest.mark.asyncio
 async def test_get_prefix_sort_order_explicit_sort_target_key():
     client = AsyncEtcd3Client(host=ETCD_HOST, api_path=API_PATH)
 
@@ -131,14 +135,15 @@
     assert keys == initial_keys_ordered.encode("latin-1")
 
     reverse_keys = b""
     for value, meta in await client.get_prefix("/doot2", sort_order="descend", sort_target="key"):
         reverse_keys += remove_prefix(meta["key"], "/doot2/")
 
     assert reverse_keys == "".join(reversed(initial_keys_ordered)).encode("latin-1")
+    await client.close()
 
 
 @pytest.mark.etcd
 @pytest.mark.asyncio
 async def test_get_prefix_sort_order_explicit_sort_target_rev():
     client = AsyncEtcd3Client(host=ETCD_HOST, api_path=API_PATH)
 
@@ -158,38 +163,41 @@
     assert keys == initial_keys.encode("latin-1")
 
     reverse_keys = b""
     for value, meta in await client.get_prefix("/expsortmod", sort_order="descend", sort_target="mod"):
         reverse_keys += remove_prefix(meta["key"], "/expsortmod/")
 
     assert reverse_keys == "".join(reversed(initial_keys)).encode("latin-1")
+    await client.close()
 
 
 @pytest.mark.etcd
 @pytest.mark.asyncio
 async def test_replace_success():
     client = AsyncEtcd3Client(host=ETCD_HOST, api_path=API_PATH)
     key = "/doot/thing" + str(uuid.uuid4())
     await client.put(key, "toot")
     status = await client.replace(key, "toot", "doot")
     v = await client.get(key)
     assert [b"doot"] == v
     assert status
+    await client.close()
 
 
 @pytest.mark.etcd
 @pytest.mark.asyncio
 async def test_replace_fail():
     client = AsyncEtcd3Client(host=ETCD_HOST, api_path=API_PATH)
     key = "/doot/thing" + str(uuid.uuid4())
     await client.put(key, "boot")
     status = await client.replace(key, "toot", "doot")
     v = await client.get(key)
     assert [b"boot"] == v
     assert not status
+    await client.close()
 
 
 @pytest.mark.etcd
 @pytest.mark.asyncio
 async def test_client_lease():
     client = AsyncEtcd3Client(host=ETCD_HOST, api_path=API_PATH)
     lease = await client.lease(ttl=60)
@@ -201,14 +209,15 @@
     keys = await lease.keys()
     assert [] == keys
 
     ttl = await lease.refresh()
     assert 0 <= ttl <= 60
 
     assert await lease.revoke()
+    await client.close()
 
 
 @pytest.mark.etcd
 @pytest.mark.asyncio
 async def test_client_lease_with_keys():
     client = AsyncEtcd3Client(host=ETCD_HOST, api_path=API_PATH)
     lease = await client.lease(ttl=60)
@@ -222,14 +231,15 @@
     assert b"foo12" in keys
     assert b"foo13" in keys
 
     assert [b"bar12"] == await client.get("foo12")
     assert [b"bar13"] == await client.get("foo13")
 
     assert await lease.revoke()
+    await client.close()
 
 
 @pytest.mark.etcd
 @pytest.mark.asyncio
 async def test_watch_key():
     client = AsyncEtcd3Client(host=ETCD_HOST, api_path=API_PATH)
     key = "/%s-watch_key/watch" % str(uuid.uuid4())
@@ -264,14 +274,15 @@
 
         change_count += 1
         if change_count > 2:
             # if cancel not work, we will block in this for-loop forever
             await cancel()
 
     await t
+    await client.close()
 
 
 @pytest.mark.etcd
 @pytest.mark.asyncio
 async def test_watch_prefix():
     client = AsyncEtcd3Client(host=ETCD_HOST, api_path=API_PATH)
     key = "/%s-watch_prefix/watch/prefix/" % str(uuid.uuid4())
@@ -326,27 +337,29 @@
         await client.watch_prefix_once("/doot/", 1)
     except exceptions.WatchTimedOut:
         pass
     try:
         await client.watch_prefix_once("/doot/", 1)
     except exceptions.WatchTimedOut:
         pass
+    await client.close()
 
 
 @pytest.mark.etcd
 @pytest.mark.asyncio
 async def test_client_lock_acquire_release():
     client = AsyncEtcd3Client(host=ETCD_HOST, api_path=API_PATH)
     async with await client.lock(ttl=60) as lock:
         ttl = await lock.refresh()
         assert 0 <= ttl <= 60
     assert not await lock.is_acquired()
 
     async with await client.lock(ttl=60) as lock:
         assert not await lock.acquire()
+    await client.close()
 
 
 @pytest.mark.etcd
 @pytest.mark.asyncio
 async def test_client_locks():
     client = AsyncEtcd3Client(host=ETCD_HOST, api_path=API_PATH)
     lock = await client.lock(id="xyz-%s" % perf_counter(), ttl=60)
@@ -358,28 +371,30 @@
     ttl = await lock.refresh()
     assert 0 <= ttl <= 60
 
     assert await lock.is_acquired()
     assert await lock.release()
     assert not await lock.release()
     assert not await lock.is_acquired()
+    await client.close()
 
 
 @pytest.mark.etcd
 @pytest.mark.asyncio
 async def test_create_success():
     client = AsyncEtcd3Client(host=ETCD_HOST, api_path=API_PATH)
     key = "/foo/unique" + str(uuid.uuid4())
     # Verify that key is empty
     assert [] == await client.get(key)
 
     status = await client.create(key, "bar")
     # Verify that key is 'bar'
     assert [b"bar"] == await client.get(key)
     assert status
+    await client.close()
 
 
 @pytest.mark.etcd
 @pytest.mark.asyncio
 async def test_create_fail():
     client = AsyncEtcd3Client(host=ETCD_HOST, api_path=API_PATH)
     key = "/foo/" + str(uuid.uuid4())
@@ -387,14 +402,15 @@
     await client.put(key, "bar")
     assert [b"bar"] == await client.get(key)
 
     status = await client.create(key, "goo")
     # Verify that key is still 'bar'
     assert [b"bar"] == await client.get(key)
     assert not status
+    await client.close()
 
 
 @pytest.mark.etcd
 @pytest.mark.asyncio
 async def test_create_with_lease_success():
     client = AsyncEtcd3Client(host=ETCD_HOST, api_path=API_PATH)
     key = "/foo/unique" + str(uuid.uuid4())
@@ -405,14 +421,15 @@
     status = await client.create(key, "bar", lease=lease)
     # Verify that key is 'bar'
     assert [b"bar"] == await client.get(key)
     assert status
     keys = await lease.keys()
     assert 1 == len(keys)
     assert key.encode("latin-1") in keys
+    await client.close()
 
 
 async def _post_key(client, key_name, provide_value=True):
     payload = {"key": utils._encode(key_name)}
     if provide_value:
         payload["value"] = utils._encode(key_name)
     await client.post(client.get_url("/kv/put"), json=payload)
@@ -424,20 +441,22 @@
     client = AsyncEtcd3Client(host=ETCD_HOST, api_path=API_PATH)
     test_key_value = b"some_key"
     await _post_key(client, test_key_value)
     result = await client.get(test_key_value, metadata=True)
     assert len(result) > 0
     value, metadata = result[0]
     assert value == test_key_value
+    await client.close()
 
 
 @pytest.mark.etcd
 @pytest.mark.asyncio
 async def test_client_keys_with_metadata_and_no_value():
     client = AsyncEtcd3Client(host=ETCD_HOST, api_path=API_PATH)
     value_is_not_set_default = b""
     test_key = b"some_key"
     await _post_key(client, test_key, provide_value=False)
     result = await client.get(test_key, metadata=True)
     assert len(result) > 0
     value, metadata = result[0]
     assert value == value_is_not_set_default
+    await client.close()
```

### Comparing `async_etcd3gw-0.5/tests/test_client.py` & `async_etcd3gw-0.6/tests/test_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,25 +15,29 @@
 from async_etcd3gw import AsyncEtcd3Client
 
 
 @pytest.mark.asyncio
 async def test_client_default():
     client = AsyncEtcd3Client()
     assert "http://localhost:2379%slease/grant" % client.api_path == client.get_url("/lease/grant")
+    await client.close()
 
 
 @pytest.mark.asyncio
 async def test_client_ipv4():
     client = AsyncEtcd3Client(host="127.0.0.1")
     assert "http://127.0.0.1:2379%slease/grant" % client.api_path == client.get_url("/lease/grant")
+    await client.close()
 
 
 @pytest.mark.asyncio
 async def test_client_ipv6():
     client = AsyncEtcd3Client(host="::1")
     assert "http://[::1]:2379%slease/grant" % client.api_path == client.get_url("/lease/grant")
+    await client.close()
 
 
 @pytest.mark.asyncio
 async def test_client_api_path():
     client = AsyncEtcd3Client(host="127.0.0.1", api_path="/v3/")
     assert "http://127.0.0.1:2379/v3/lease/grant" == client.get_url("/lease/grant")
+    await client.close()
```

