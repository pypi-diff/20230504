# Comparing `tmp/POTHEAD-0.8.5.tar.gz` & `tmp/POTHEAD-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "POTHEAD-0.8.5.tar", last modified: Tue Apr  4 15:22:30 2023, max compression
+gzip compressed data, was "POTHEAD-0.8.6.tar", last modified: Thu May  4 15:23:07 2023, max compression
```

## Comparing `POTHEAD-0.8.5.tar` & `POTHEAD-0.8.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 ulrikm    (1000) ulrikm    (1000)        0 2023-04-04 15:22:30.125664 POTHEAD-0.8.5/
--rw-r--r--   0 ulrikm    (1000) ulrikm    (1000)    10174 2019-07-16 19:09:21.000000 POTHEAD-0.8.5/LICENSE
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     4214 2023-04-04 15:22:30.125664 POTHEAD-0.8.5/PKG-INFO
-drwxrwxr-x   0 ulrikm    (1000) ulrikm    (1000)        0 2023-04-04 15:22:30.121664 POTHEAD-0.8.5/POTHEAD.egg-info/
--rw-r--r--   0 ulrikm    (1000) ulrikm    (1000)     4214 2023-04-04 15:22:30.000000 POTHEAD-0.8.5/POTHEAD.egg-info/PKG-INFO
--rw-r--r--   0 ulrikm    (1000) ulrikm    (1000)      517 2023-04-04 15:22:30.000000 POTHEAD-0.8.5/POTHEAD.egg-info/SOURCES.txt
--rw-r--r--   0 ulrikm    (1000) ulrikm    (1000)        1 2023-04-04 15:22:30.000000 POTHEAD-0.8.5/POTHEAD.egg-info/dependency_links.txt
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)       71 2023-04-04 15:22:30.000000 POTHEAD-0.8.5/POTHEAD.egg-info/requires.txt
--rw-r--r--   0 ulrikm    (1000) ulrikm    (1000)        8 2023-04-04 15:22:30.000000 POTHEAD-0.8.5/POTHEAD.egg-info/top_level.txt
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     3700 2021-06-10 19:44:43.000000 POTHEAD-0.8.5/README.md
-drwxrwxr-x   0 ulrikm    (1000) ulrikm    (1000)        0 2023-04-04 15:22:30.125664 POTHEAD-0.8.5/pothead/
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)       17 2021-06-10 15:08:55.000000 POTHEAD-0.8.5/pothead/__init__.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     2934 2023-03-15 11:01:30.000000 POTHEAD-0.8.5/pothead/cgroups.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     7298 2023-03-15 10:50:06.000000 POTHEAD-0.8.5/pothead/gating.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     8198 2023-02-01 12:53:52.000000 POTHEAD-0.8.5/pothead/oob_response.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     2451 2021-06-10 15:08:55.000000 POTHEAD-0.8.5/pothead/resource_balancer.py
--rwxrwxr-x   0 ulrikm    (1000) ulrikm    (1000)     2494 2021-06-10 15:08:55.000000 POTHEAD-0.8.5/pothead/server.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)    11242 2023-04-04 15:05:09.000000 POTHEAD-0.8.5/pothead/subprocess_middleware.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     2282 2023-03-15 11:07:34.000000 POTHEAD-0.8.5/pothead/test_cgroups.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     2569 2021-06-10 15:08:55.000000 POTHEAD-0.8.5/pothead/test_resource_balancer.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)    14201 2023-04-04 15:03:04.000000 POTHEAD-0.8.5/pothead/test_subprocess_middleware.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     7997 2023-02-09 08:43:22.000000 POTHEAD-0.8.5/pothead/test_worker.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     1173 2023-02-09 14:53:08.000000 POTHEAD-0.8.5/pothead/util.py
--rwxrwxr-x   0 ulrikm    (1000) ulrikm    (1000)    14504 2023-03-09 15:36:20.000000 POTHEAD-0.8.5/pothead/worker.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     1239 2021-06-10 19:40:00.000000 POTHEAD-0.8.5/pothead/wsgi_typing.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)       38 2023-04-04 15:22:30.125664 POTHEAD-0.8.5/setup.cfg
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)      871 2023-04-04 15:21:46.000000 POTHEAD-0.8.5/setup.py
+drwxrwxr-x   0 ulrikm    (1000) ulrikm    (1000)        0 2023-05-04 15:23:07.176410 POTHEAD-0.8.6/
+-rw-r--r--   0 ulrikm    (1000) ulrikm    (1000)    10174 2019-07-16 19:09:21.000000 POTHEAD-0.8.6/LICENSE
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     4177 2023-05-04 15:23:07.176410 POTHEAD-0.8.6/PKG-INFO
+drwxrwxr-x   0 ulrikm    (1000) ulrikm    (1000)        0 2023-05-04 15:23:07.176410 POTHEAD-0.8.6/POTHEAD.egg-info/
+-rw-r--r--   0 ulrikm    (1000) ulrikm    (1000)     4177 2023-05-04 15:23:07.000000 POTHEAD-0.8.6/POTHEAD.egg-info/PKG-INFO
+-rw-r--r--   0 ulrikm    (1000) ulrikm    (1000)      517 2023-05-04 15:23:07.000000 POTHEAD-0.8.6/POTHEAD.egg-info/SOURCES.txt
+-rw-r--r--   0 ulrikm    (1000) ulrikm    (1000)        1 2023-05-04 15:23:07.000000 POTHEAD-0.8.6/POTHEAD.egg-info/dependency_links.txt
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)       76 2023-05-04 15:23:07.000000 POTHEAD-0.8.6/POTHEAD.egg-info/requires.txt
+-rw-r--r--   0 ulrikm    (1000) ulrikm    (1000)        8 2023-05-04 15:23:07.000000 POTHEAD-0.8.6/POTHEAD.egg-info/top_level.txt
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     3700 2021-06-10 19:44:43.000000 POTHEAD-0.8.6/README.md
+drwxrwxr-x   0 ulrikm    (1000) ulrikm    (1000)        0 2023-05-04 15:23:07.176410 POTHEAD-0.8.6/pothead/
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)       17 2021-06-10 15:08:55.000000 POTHEAD-0.8.6/pothead/__init__.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     2934 2023-03-15 11:01:30.000000 POTHEAD-0.8.6/pothead/cgroups.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     7298 2023-03-15 10:50:06.000000 POTHEAD-0.8.6/pothead/gating.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     8198 2023-02-01 12:53:52.000000 POTHEAD-0.8.6/pothead/oob_response.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     2451 2021-06-10 15:08:55.000000 POTHEAD-0.8.6/pothead/resource_balancer.py
+-rwxrwxr-x   0 ulrikm    (1000) ulrikm    (1000)     2494 2021-06-10 15:08:55.000000 POTHEAD-0.8.6/pothead/server.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)    11242 2023-04-04 15:05:09.000000 POTHEAD-0.8.6/pothead/subprocess_middleware.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     2282 2023-03-15 11:07:34.000000 POTHEAD-0.8.6/pothead/test_cgroups.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     2569 2021-06-10 15:08:55.000000 POTHEAD-0.8.6/pothead/test_resource_balancer.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)    14323 2023-04-24 20:03:05.000000 POTHEAD-0.8.6/pothead/test_subprocess_middleware.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     9156 2023-04-24 20:03:18.000000 POTHEAD-0.8.6/pothead/test_worker.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     1173 2023-02-09 14:53:08.000000 POTHEAD-0.8.6/pothead/util.py
+-rwxrwxr-x   0 ulrikm    (1000) ulrikm    (1000)    14570 2023-04-24 20:03:05.000000 POTHEAD-0.8.6/pothead/worker.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     1239 2021-06-10 19:40:00.000000 POTHEAD-0.8.6/pothead/wsgi_typing.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)       38 2023-05-04 15:23:07.176410 POTHEAD-0.8.6/setup.cfg
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)      876 2023-05-04 15:22:31.000000 POTHEAD-0.8.6/setup.py
```

### Comparing `POTHEAD-0.8.5/LICENSE` & `POTHEAD-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.5/PKG-INFO` & `POTHEAD-0.8.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: POTHEAD
-Version: 0.8.5
+Version: 0.8.6
 Summary: A reverse-http proxy implementation for non-concurrent requests
 Home-page: https://gitlab.com/rawler/pothead
 Author: Ulrik Mikaelsson
 Author-email: ulrik.mikaelsson@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
@@ -61,9 +59,7 @@
        http://www.apache.org/licenses/LICENSE-2.0
 
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
-
-
```

### Comparing `POTHEAD-0.8.5/POTHEAD.egg-info/PKG-INFO` & `POTHEAD-0.8.6/POTHEAD.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: POTHEAD
-Version: 0.8.5
+Version: 0.8.6
 Summary: A reverse-http proxy implementation for non-concurrent requests
 Home-page: https://gitlab.com/rawler/pothead
 Author: Ulrik Mikaelsson
 Author-email: ulrik.mikaelsson@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
@@ -61,9 +59,7 @@
        http://www.apache.org/licenses/LICENSE-2.0
 
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
-
-
```

### Comparing `POTHEAD-0.8.5/POTHEAD.egg-info/SOURCES.txt` & `POTHEAD-0.8.6/POTHEAD.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.5/README.md` & `POTHEAD-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.5/pothead/cgroups.py` & `POTHEAD-0.8.6/pothead/cgroups.py`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.5/pothead/gating.py` & `POTHEAD-0.8.6/pothead/gating.py`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.5/pothead/oob_response.py` & `POTHEAD-0.8.6/pothead/oob_response.py`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.5/pothead/resource_balancer.py` & `POTHEAD-0.8.6/pothead/resource_balancer.py`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.5/pothead/server.py` & `POTHEAD-0.8.6/pothead/server.py`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.5/pothead/subprocess_middleware.py` & `POTHEAD-0.8.6/pothead/subprocess_middleware.py`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.5/pothead/test_cgroups.py` & `POTHEAD-0.8.6/pothead/test_cgroups.py`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.5/pothead/test_resource_balancer.py` & `POTHEAD-0.8.6/pothead/test_resource_balancer.py`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.5/pothead/test_subprocess_middleware.py` & `POTHEAD-0.8.6/pothead/test_subprocess_middleware.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,17 @@
                     time.sleep(1)
 
             # This thread will prevent the subprocess from exiting normally
             t = Thread(target=sleep_forever, daemon=False)
             t.start()
 
             # This subprocess represents something that the app might spawn, that doesn't automatically exit on its own
-            subprocess.Popen(["bash", "-c", "while true; do sleep 1000; echo HI FROM APP; done"])
+            subprocess.Popen(
+                ["bash", "-c", "while true; do sleep 1000; echo HI FROM APP; done"]
+            )
 
             if request.path == "/test_successful_subprocess_is_shut_down":
                 start_response("200 OK", [], None)
             else:
                 raise Exception("This is an exception message")
         elif request.path == "/test_client_disconnect_while_sending_request":
             raise Exception("Should never make it to this point")
@@ -334,17 +336,21 @@
             # If the app leaked running subprocesses upon being killed, these will be orphaned by
             # the init process. To avoid getting false positives on this (in case the init process has
             # adopted some unrelated subprocesses while the test was being run), we only conclude that
             # a process was leaked if its cmdline matches a known string.
             init_subprocesses_after = set(init_process.children(recursive=True))
             if init_subprocesses_before != init_subprocesses_after:
                 # Avoid hanging the test itself in case it fails
-                extra_processes = init_subprocesses_after.difference(init_subprocesses_before)
+                extra_processes = init_subprocesses_after.difference(
+                    init_subprocesses_before
+                )
                 leaked_subprocess = None
                 for p in extra_processes:
                     if any(word for word in p.cmdline() if "HI FROM APP" in word):
                         leaked_subprocess = p
-                        print(f"Leaked subprocess: {leaked_subprocess} ({leaked_subprocess.cmdline()})")
+                        print(
+                            f"Leaked subprocess: {leaked_subprocess} ({leaked_subprocess.cmdline()})"
+                        )
                     p.terminate()
 
                 if leaked_subprocess:
                     assert False, f"Subprocess was leaked: {leaked_subprocess}"
```

### Comparing `POTHEAD-0.8.5/pothead/test_worker.py` & `POTHEAD-0.8.6/pothead/test_worker.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,52 +1,66 @@
-from socket import AF_INET, SOCK_STREAM, socket
-from socket import timeout as TimeoutError
+from socket import AF_INET, SOCK_STREAM, socket, timeout as TimeoutError, SHUT_RDWR
 from threading import Thread
 from time import sleep, monotonic
 from typing import Optional
 from unittest import TestCase
 from unittest.mock import MagicMock
 from urllib.request import urlopen
+from logging import INFO
+
+from pytest import fixture
 
 OOB_CLEANUP_INTERVAL_SECONDS = 0.05
 OOB_ITEM_EXPIRY_SECONDS = 0.5
+REQUEST_ID = "im-quite-unique!"
 
 from pothead.gating import wait_for_idle_cpus  # noqa: E402 override environ first
 
 from .util import ObjectProxy  # noqa: E402
 from .worker import LoadBalancer, Server  # noqa: E402
 
 
 def demo_app(environ, start_response):
     path = environ.get("PATH_INFO")
     if path == "/":
         start_response("200 OK", ())
-        return [b"Hello World!"]
+        yield b"Hello World!"
     elif path == "/crash":
         raise Exception("Nope nope nope")
+    elif path == "/slow_loris":
+        sleep(0.05)
+        start_response("200 OK", ())
+        for byte in b"This might take a while...":
+            sleep(0.1)
+            yield byte
     else:
         start_response("404 Not Found", ())
-        return []
 
 
 class WorkerConnection:
     def __init__(self, sock: socket):
         self.sock = sock
 
     def send_request(self, path="/"):
-        self.sock.sendall(b"GET " + path.encode() + b" HTTP/1.1\r\n\r\n")
+        self.sock.sendall(
+            f"GET {path} HTTP/1.1\r\nx-request-id: {REQUEST_ID}\r\n\r\n".encode("ascii")
+        )
 
     def read_response(self):
         buf = b""
         read = True
         while read:
             read = self.sock.recv(1024)
             buf += read
         return buf
 
+    def disconnect(self):
+        self.sock.shutdown(SHUT_RDWR)
+        self.sock.close()
+
 
 class DummyBroker:
     def __init__(self):
         self.sock = socket(AF_INET, SOCK_STREAM)
         self.sock.bind(("localhost", 0))
         self.sock.listen(1)
 
@@ -111,14 +125,19 @@
             from time import sleep
 
             while not halt():
                 sleep(0.05)
 
 
 class RedirectWorkerTest(TestCase):
+    @fixture(autouse=True)
+    def use_caplog(self, caplog):
+        caplog.set_level(INFO)
+        self.caplog = caplog
+
     def setUp(self):
         broker = DummyBroker()
         self.callbacks = MagicMock()
 
         app = ObjectProxy(demo_app)
         app.wait_for_slot = WaitForFirstSlot(self.callbacks)
 
@@ -195,14 +214,38 @@
 
         self.callbacks.done.assert_not_called()
 
         sleep(OOB_ITEM_EXPIRY_SECONDS + 2 * OOB_CLEANUP_INTERVAL_SECONDS)
 
         self.callbacks.done.assert_called()
 
+    def test_log_elapsed_after_success(self):
+        self.connection.send_request()
+        self.connection.read_response()
+
+        sleep(0.05)
+
+        assert f"[{REQUEST_ID}] Elapsed: " in self.caplog.text
+
+    def test_log_elapsed_after_crash(self):
+        self.connection.send_request("/crash")
+        self.connection.read_response()
+
+        sleep(0.05)
+
+        assert f"[{REQUEST_ID}] Elapsed: " in self.caplog.text
+
+    def test_log_elapsed_after_disconnect(self):
+        self.connection.send_request("/slow_loris")
+        self.connection.disconnect()
+
+        sleep(0.2)
+
+        assert f"[{REQUEST_ID}] Elapsed: " in self.caplog.text
+
 
 class TestShutdown(TestCase):
     DELAY_START_RESPONSE = 0.3
     DELAY_FINISH_RESPONSE = 0.8
 
     def setUp(self):
         broker = DummyBroker()
```

### Comparing `POTHEAD-0.8.5/pothead/util.py` & `POTHEAD-0.8.6/pothead/util.py`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.5/pothead/worker.py` & `POTHEAD-0.8.6/pothead/worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,19 @@
     def log_message(self, format, *args):
         LOGGER.info("[%s] " + format, self.request_id, *args)
 
     def log_request(self, code="-", size="-"):
         if isinstance(code, HTTPStatus):
             code = code.value
         LOGGER.info(
-            '[%s] "%s" %s %s', self.request_id, self.requestline, str(code), str(size)
+            'Starting request [%s] "%s" %s %s',
+            self.request_id,
+            self.requestline,
+            str(code),
+            str(size),
         )
 
     def log_error(self, format, *args):
         LOGGER.error("[%s] " + format, self.request_id, *args)
 
     def log_elapsed(self):
         LOGGER.info(
```

### Comparing `POTHEAD-0.8.5/pothead/wsgi_typing.py` & `POTHEAD-0.8.6/pothead/wsgi_typing.py`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.5/setup.py` & `POTHEAD-0.8.6/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 test_deps = ["aiohttp", "werkzeug", "tblib", "timeout-decorator"]
 
 setuptools.setup(
     name="POTHEAD",
-    version="0.8.5",
+    version="0.8.6",
     author="Ulrik Mikaelsson",
     author_email="ulrik.mikaelsson@gmail.com",
     description="A reverse-http proxy implementation for non-concurrent requests",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/rawler/pothead",
     packages=setuptools.find_packages(),
-    install_requires=["psutil", "werkzeug", "tblib"],
+    install_requires=["psutil", "werkzeug>=2.1", "tblib"],
     tests_require=test_deps,
     extras_require={
         "test": test_deps,
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
```

