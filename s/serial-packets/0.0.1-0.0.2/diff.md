# Comparing `tmp/serial_packets-0.0.1.tar.gz` & `tmp/serial_packets-0.0.2.tar.gz`

## Comparing `serial_packets-0.0.1.tar` & `serial_packets-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,23 @@
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 serial_packets-0.0.1/TODO.txt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 serial_packets-0.0.1/src/.gitignore
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 serial_packets-0.0.1/src/requirements.txt
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 serial_packets-0.0.1/src/.vscode/launch.json
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 serial_packets-0.0.1/src/.vscode/settings.json
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 serial_packets-0.0.1/src/examples/.run.sh
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 serial_packets-0.0.1/src/examples/.run1.sh
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 serial_packets-0.0.1/src/examples/.run2.sh
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 serial_packets-0.0.1/src/examples/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 serial_packets-0.0.1/src/serial_packets/__init__.py
--rw-r--r--   0        0        0     5800 2020-02-02 00:00:00.000000 serial_packets-0.0.1/src/serial_packets/_packet_decoder.py
--rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 serial_packets-0.0.1/src/serial_packets/_packet_encoder.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 serial_packets-0.0.1/src/serial_packets/_packets.py
--rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 serial_packets-0.0.1/src/serial_packets/client.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 serial_packets-0.0.1/src/serial_packets/packets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 serial_packets-0.0.1/src/serial_packets/py.typed
--rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 serial_packets-0.0.1/LICENSE
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 serial_packets-0.0.1/README.md
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 serial_packets-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 serial_packets-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 serial_packets-0.0.2/TODO.txt
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 serial_packets-0.0.2/build.sh
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 serial_packets-0.0.2/upload_pypi.sh
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 serial_packets-0.0.2/upload_testpypi.sh
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 serial_packets-0.0.2/src/.gitignore
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 serial_packets-0.0.2/src/requirements.txt
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 serial_packets-0.0.2/src/.vscode/launch.json
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 serial_packets-0.0.2/src/.vscode/settings.json
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 serial_packets-0.0.2/src/examples/.run.sh
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 serial_packets-0.0.2/src/examples/.run1.sh
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 serial_packets-0.0.2/src/examples/.run2.sh
+-rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 serial_packets-0.0.2/src/examples/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 serial_packets-0.0.2/src/serial_packets/__init__.py
+-rw-r--r--   0        0        0     5800 2020-02-02 00:00:00.000000 serial_packets-0.0.2/src/serial_packets/_packet_decoder.py
+-rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 serial_packets-0.0.2/src/serial_packets/_packet_encoder.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 serial_packets-0.0.2/src/serial_packets/_packets.py
+-rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 serial_packets-0.0.2/src/serial_packets/client.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 serial_packets-0.0.2/src/serial_packets/packets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 serial_packets-0.0.2/src/serial_packets/py.typed
+-rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 serial_packets-0.0.2/LICENSE
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 serial_packets-0.0.2/README.md
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 serial_packets-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 serial_packets-0.0.2/PKG-INFO
```

### Comparing `serial_packets-0.0.1/src/examples/main.py` & `serial_packets-0.0.2/src/examples/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 # This will use the local copy of serial_packets. Comment
 # out to use the pip loaded version
-import sys
-sys.path.insert(0, "..")
+#import sys
+#sys.path.insert(0, "..")
 
 import argparse
 import asyncio
 import logging
 from typing import Tuple, Optional
 from serial_packets.client import SerialPacketsClient
 from serial_packets.packets import PacketStatus
```

### Comparing `serial_packets-0.0.1/src/serial_packets/_packet_decoder.py` & `serial_packets-0.0.2/src/serial_packets/_packet_decoder.py`

 * *Files identical despite different names*

### Comparing `serial_packets-0.0.1/src/serial_packets/_packet_encoder.py` & `serial_packets-0.0.2/src/serial_packets/_packet_encoder.py`

 * *Files identical despite different names*

### Comparing `serial_packets-0.0.1/src/serial_packets/_packets.py` & `serial_packets-0.0.2/src/serial_packets/_packets.py`

 * *Files identical despite different names*

### Comparing `serial_packets-0.0.1/src/serial_packets/client.py` & `serial_packets-0.0.2/src/serial_packets/client.py`

 * *Files identical despite different names*

### Comparing `serial_packets-0.0.1/src/serial_packets/packets.py` & `serial_packets-0.0.2/src/serial_packets/packets.py`

 * *Files identical despite different names*

### Comparing `serial_packets-0.0.1/LICENSE` & `serial_packets-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `serial_packets-0.0.1/pyproject.toml` & `serial_packets-0.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "serial_packets"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Zapta", email="zapta@zapta.com" },
 ]
 description = "A Python impelementation of the Serial Packets protocol"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication",
     "Operating System :: OS Independent",
 ]
 
+dependencies = [
+    "pyserial-asyncio >=0.6.0",
+    "pythoncrc >=1.21.0",
+]
+
 [project.urls]
 "Homepage" = "https://github.com/zapta/serial_packets_py"
 "Bug Tracker" = "https://github.com/zapta/serial_packets_py/issues"
```

### Comparing `serial_packets-0.0.1/PKG-INFO` & `serial_packets-0.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: serial_packets
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python impelementation of the Serial Packets protocol
 Project-URL: Homepage, https://github.com/zapta/serial_packets_py
 Project-URL: Bug Tracker, https://github.com/zapta/serial_packets_py/issues
 Author-email: Zapta <zapta@zapta.com>
 License-File: LICENSE
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
+Requires-Dist: pyserial-asyncio>=0.6.0
+Requires-Dist: pythoncrc>=1.21.0
 Description-Content-Type: text/markdown
 
 # serial_packets_py
 Python implementations of the Serial Packets protocol.
 
 WORK IN PROGRESS, NOT READY FOR PUBLIC RELEASE.
```

