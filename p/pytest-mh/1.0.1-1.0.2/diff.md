# Comparing `tmp/pytest_mh-1.0.1.tar.gz` & `tmp/pytest_mh-1.0.2.tar.gz`

## Comparing `pytest_mh-1.0.1.tar` & `pytest_mh-1.0.2.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 pytest_mh-1.0.1/requirements.txt
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 pytest_mh-1.0.1/docs/requirements.txt
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 pytest_mh-1.0.1/pytest_mh/__init__.py
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 pytest_mh-1.0.1/pytest_mh/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_mh-1.0.1/pytest_mh/py.typed
--rw-r--r--   0        0        0    30978 2020-02-02 00:00:00.000000 pytest_mh-1.0.1/pytest_mh/ssh.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 pytest_mh-1.0.1/pytest_mh/_private/data.py
--rw-r--r--   0        0        0     8103 2020-02-02 00:00:00.000000 pytest_mh-1.0.1/pytest_mh/_private/fixtures.py
--rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 pytest_mh-1.0.1/pytest_mh/_private/logging.py
--rw-r--r--   0        0        0     8334 2020-02-02 00:00:00.000000 pytest_mh-1.0.1/pytest_mh/_private/marks.py
--rw-r--r--   0        0        0    16982 2020-02-02 00:00:00.000000 pytest_mh-1.0.1/pytest_mh/_private/multihost.py
--rw-r--r--   0        0        0    14927 2020-02-02 00:00:00.000000 pytest_mh-1.0.1/pytest_mh/_private/plugin.py
--rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 pytest_mh-1.0.1/pytest_mh/_private/topology.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 pytest_mh-1.0.1/pytest_mh/_private/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_mh-1.0.1/pytest_mh/utils/__init__.py
--rw-r--r--   0        0        0    14342 2020-02-02 00:00:00.000000 pytest_mh-1.0.1/pytest_mh/utils/fs.py
--rw-r--r--   0        0        0     7953 2020-02-02 00:00:00.000000 pytest_mh-1.0.1/pytest_mh/utils/services.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 pytest_mh-1.0.1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pytest_mh-1.0.1/LICENSE
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 pytest_mh-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 pytest_mh-1.0.1/readme.md
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 pytest_mh-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 pytest_mh-1.0.2/requirements.txt
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 pytest_mh-1.0.2/docs/requirements.txt
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 pytest_mh-1.0.2/pytest_mh/__init__.py
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 pytest_mh-1.0.2/pytest_mh/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_mh-1.0.2/pytest_mh/py.typed
+-rw-r--r--   0        0        0    31460 2020-02-02 00:00:00.000000 pytest_mh-1.0.2/pytest_mh/ssh.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 pytest_mh-1.0.2/pytest_mh/_private/data.py
+-rw-r--r--   0        0        0     8103 2020-02-02 00:00:00.000000 pytest_mh-1.0.2/pytest_mh/_private/fixtures.py
+-rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 pytest_mh-1.0.2/pytest_mh/_private/logging.py
+-rw-r--r--   0        0        0     8334 2020-02-02 00:00:00.000000 pytest_mh-1.0.2/pytest_mh/_private/marks.py
+-rw-r--r--   0        0        0    18781 2020-02-02 00:00:00.000000 pytest_mh-1.0.2/pytest_mh/_private/multihost.py
+-rw-r--r--   0        0        0    14927 2020-02-02 00:00:00.000000 pytest_mh-1.0.2/pytest_mh/_private/plugin.py
+-rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 pytest_mh-1.0.2/pytest_mh/_private/topology.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 pytest_mh-1.0.2/pytest_mh/_private/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_mh-1.0.2/pytest_mh/utils/__init__.py
+-rw-r--r--   0        0        0     9886 2020-02-02 00:00:00.000000 pytest_mh-1.0.2/pytest_mh/utils/firewall.py
+-rw-r--r--   0        0        0    14342 2020-02-02 00:00:00.000000 pytest_mh-1.0.2/pytest_mh/utils/fs.py
+-rw-r--r--   0        0        0     7953 2020-02-02 00:00:00.000000 pytest_mh-1.0.2/pytest_mh/utils/services.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pytest_mh-1.0.2/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pytest_mh-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 pytest_mh-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 pytest_mh-1.0.2/readme.md
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 pytest_mh-1.0.2/PKG-INFO
```

### Comparing `pytest_mh-1.0.1/pytest_mh/__init__.py` & `pytest_mh-1.0.2/pytest_mh/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.1/pytest_mh/cli.py` & `pytest_mh-1.0.2/pytest_mh/cli.py`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.1/pytest_mh/ssh.py` & `pytest_mh-1.0.2/pytest_mh/ssh.py`

 * *Files 2% similar despite different names*

```diff
@@ -898,38 +898,46 @@
             env=env,
             input=input,
             read_timeout=read_timeout,
             log_level=log_level,
             raise_on_error=raise_on_error,
         )
 
-    def expect(self, expect_script: str) -> SSHProcessResult:
+    def expect(self, expect_script: str, raise_on_error: bool = False) -> SSHProcessResult:
         """
         Run expect script.
 
         :param expect_script: Expect script.
         :type expect_script: str
+        :param raise_on_error: If True, raise :class:`SSHProcessError` if
+            command exited with non-zero return code, defaults to False
+        :type raise_on_error: bool, optional
         :return: Expect script result.
         :rtype: SSHProcessResult
         """
-        return self.run("/bin/expect -d", input=expect_script, raise_on_error=False)
+        return self.run("/bin/expect -d", input=expect_script, raise_on_error=raise_on_error)
 
-    def expect_nobody(self, expect_script: str) -> SSHProcessResult:
+    def expect_nobody(self, expect_script: str, raise_on_error: bool = False) -> SSHProcessResult:
         """
         Run expect script as user nobody.
 
         The main use case is to avoid running the command as root if the client
         is connected to the root user SSH session.
 
         :param expect_script: Expect script.
         :type expect_script: str
+        :param raise_on_error: If True, raise :class:`SSHProcessError` if
+            command exited with non-zero return code, defaults to False
+        :type raise_on_error: bool, optional
         :return: Expect return code.
         :rtype: SSHProcessResult
         """
-        return self.run('su --shell /bin/sh nobody -c "/bin/expect -d"', input=expect_script, raise_on_error=False)
+        return self.run(
+            'su --shell /bin/sh nobody -c "/bin/expect -d"', input=expect_script, raise_on_error=raise_on_error
+        )
 
     def __enter__(self) -> SSHClient:
         """
         Connect to the host.
 
         :return: SSHClient instance.
         :rtype: SSHClient
```

### Comparing `pytest_mh-1.0.1/pytest_mh/_private/data.py` & `pytest_mh-1.0.2/pytest_mh/_private/data.py`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.1/pytest_mh/_private/fixtures.py` & `pytest_mh-1.0.2/pytest_mh/_private/fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.1/pytest_mh/_private/logging.py` & `pytest_mh-1.0.2/pytest_mh/_private/logging.py`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.1/pytest_mh/_private/marks.py` & `pytest_mh-1.0.2/pytest_mh/_private/marks.py`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.1/pytest_mh/_private/multihost.py` & `pytest_mh-1.0.2/pytest_mh/_private/multihost.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import inspect
 from abc import ABC, abstractmethod
 from base64 import b64decode
 from enum import Enum
+from functools import wraps
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Generic, Type, TypeVar
 
 from ..cli import CLIBuilder
 from ..ssh import SSHBashProcess, SSHClient, SSHLog, SSHPowerShellProcess, SSHProcess
 from .logging import MultihostLogger
 from .marks import TopologyMark
@@ -490,28 +491,73 @@
 
     def __init__(self, host: HostType) -> None:
         """
         :param host: Remote host instance.
         :type host: HostType
         """
         self.host: HostType = host
+        """Multihost host."""
+
         self.logger: MultihostLogger = self.host.logger
+        """Multihost logger."""
+
+        self.used: bool = False
+        """Indicate if this utility instance was already used or not within current test."""
+
+        # Enable first use setup
+        disallowed = [
+            "setup",
+            "teardown",
+            "setup_when_used",
+            "teardown_when_used",
+            "GetUtilityAttributes",
+            "SetupUtilityAttributes",
+            "TeardownUtilityAttributes",
+        ]
+        for name, method in inspect.getmembers(self, inspect.ismethod):
+            if name in disallowed or name.startswith("_") or hasattr(method, "__mh_ignore_call"):
+                continue
+
+            setattr(self, name, self.__setup_when_used(method))
 
     def setup(self) -> None:
         """
         Setup object.
         """
         pass
 
     def teardown(self) -> None:
         """
         Teardown object.
         """
         pass
 
+    def setup_when_used(self) -> None:
+        """
+        Setup the object when it is used for the first time.
+        """
+        pass
+
+    def teardown_when_used(self) -> None:
+        """
+        Teardown the object only if it was used.
+        """
+        pass
+
+    def __setup_when_used(self, method):
+        @wraps(method)
+        def wrapper(*args, **kwargs):
+            if not self.used:
+                self.setup_when_used()
+
+            self.used = True
+            return method(*args, **kwargs)
+
+        return wrapper
+
     @staticmethod
     def GetUtilityAttributes(o: object) -> dict[str, MultihostUtility]:
         """
         Get all attributes of the ``o`` that are instance of
         :class:`MultihostUtility`.
 
         :param o: Any object.
@@ -540,14 +586,30 @@
         object.
 
         :param o: Any object.
         :type o: object
         """
         errors = []
         for util in cls.GetUtilityAttributes(o).values():
+            if util.used:
+                try:
+                    util.teardown_when_used()
+                except Exception as e:
+                    errors.append(e)
+
             try:
                 util.teardown()
             except Exception as e:
                 errors.append(e)
 
         if errors:
             raise Exception(errors)
+
+    @classmethod
+    def IgnoreCall(cls, method):
+        """
+        Calling a method decorated with IgnoreCall does not execute neither
+        :meth:`setup_when_used` nor :meth:`teardown_when_used`. It does not
+        count as "using" the class.
+        """
+        method.__mh_ignore_call = True
+        return method
```

### Comparing `pytest_mh-1.0.1/pytest_mh/_private/plugin.py` & `pytest_mh-1.0.2/pytest_mh/_private/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.1/pytest_mh/_private/topology.py` & `pytest_mh-1.0.2/pytest_mh/_private/topology.py`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.1/pytest_mh/_private/utils.py` & `pytest_mh-1.0.2/pytest_mh/_private/utils.py`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.1/pytest_mh/utils/fs.py` & `pytest_mh-1.0.2/pytest_mh/utils/fs.py`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.1/pytest_mh/utils/services.py` & `pytest_mh-1.0.2/pytest_mh/utils/services.py`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.1/LICENSE` & `pytest_mh-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.1/pyproject.toml` & `pytest_mh-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.1/readme.md` & `pytest_mh-1.0.2/readme.md`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.1/PKG-INFO` & `pytest_mh-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-mh
-Version: 1.0.1
+Version: 1.0.2
 Summary: Pytest multihost plugin
 Project-URL: Homepage, https://github.com/next-actions/pytest-mh
 Project-URL: Bug Tracker, https://github.com/next-actions/pytest-mh/issues
 Author-email: Pavel Březina <pbrezina@redhat.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

