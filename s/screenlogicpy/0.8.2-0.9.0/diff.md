# Comparing `tmp/screenlogicpy-0.8.2.tar.gz` & `tmp/screenlogicpy-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "screenlogicpy-0.8.2.tar", last modified: Thu Mar 16 15:42:03 2023, max compression
+gzip compressed data, was "screenlogicpy-0.9.0.tar", last modified: Thu May  4 07:09:41 2023, max compression
```

## Comparing `screenlogicpy-0.8.2.tar` & `screenlogicpy-0.9.0.tar`

### file list

```diff
@@ -1,48 +1,61 @@
-drwxrwxrwx   0        0        0        0 2023-03-16 15:42:03.549002 screenlogicpy-0.8.2/
--rw-rw-rw-   0        0        0    35803 2020-01-02 07:35:49.000000 screenlogicpy-0.8.2/LICENSE
--rw-rw-rw-   0        0        0    27105 2023-03-16 15:42:03.548003 screenlogicpy-0.8.2/PKG-INFO
--rw-rw-rw-   0        0        0    26347 2023-03-05 23:13:04.000000 screenlogicpy-0.8.2/README.md
--rw-rw-rw-   0        0        0      108 2021-11-08 00:04:54.000000 screenlogicpy-0.8.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-03-16 15:42:03.486005 screenlogicpy-0.8.2/screenlogicpy/
--rw-rw-rw-   0        0        0      225 2023-03-16 15:10:02.000000 screenlogicpy-0.8.2/screenlogicpy/__init__.py
--rw-rw-rw-   0        0        0      384 2023-02-26 09:22:41.000000 screenlogicpy-0.8.2/screenlogicpy/__main__.py
--rw-rw-rw-   0        0        0    18626 2023-03-04 09:17:37.000000 screenlogicpy-0.8.2/screenlogicpy/cli.py
--rw-rw-rw-   0        0        0     7929 2023-03-16 15:10:02.000000 screenlogicpy-0.8.2/screenlogicpy/client.py
--rw-rw-rw-   0        0        0    10632 2023-03-16 15:10:02.000000 screenlogicpy-0.8.2/screenlogicpy/const.py
--rw-rw-rw-   0        0        0     3844 2021-11-08 00:04:54.000000 screenlogicpy-0.8.2/screenlogicpy/discovery.py
--rw-rw-rw-   0        0        0    16191 2023-03-16 15:10:02.000000 screenlogicpy-0.8.2/screenlogicpy/gateway.py
-drwxrwxrwx   0        0        0        0 2023-03-16 15:42:03.536003 screenlogicpy-0.8.2/screenlogicpy/requests/
--rw-rw-rw-   0        0        0      804 2023-03-16 15:10:02.000000 screenlogicpy-0.8.2/screenlogicpy/requests/__init__.py
--rw-rw-rw-   0        0        0      510 2023-03-05 23:13:04.000000 screenlogicpy-0.8.2/screenlogicpy/requests/button.py
--rw-rw-rw-   0        0        0     9679 2023-03-05 23:13:04.000000 screenlogicpy-0.8.2/screenlogicpy/requests/chemistry.py
--rw-rw-rw-   0        0        0      921 2023-03-05 23:13:04.000000 screenlogicpy-0.8.2/screenlogicpy/requests/client.py
--rw-rw-rw-   0        0        0     4841 2023-03-05 23:13:04.000000 screenlogicpy-0.8.2/screenlogicpy/requests/config.py
--rw-rw-rw-   0        0        0     1716 2023-03-05 23:13:04.000000 screenlogicpy-0.8.2/screenlogicpy/requests/equipment.py
--rw-rw-rw-   0        0        0      414 2023-03-05 23:13:04.000000 screenlogicpy-0.8.2/screenlogicpy/requests/gateway.py
--rw-rw-rw-   0        0        0      851 2023-03-05 23:13:04.000000 screenlogicpy-0.8.2/screenlogicpy/requests/heat.py
--rw-rw-rw-   0        0        0     1046 2023-03-05 23:13:04.000000 screenlogicpy-0.8.2/screenlogicpy/requests/lights.py
--rw-rw-rw-   0        0        0     4524 2023-03-16 15:10:02.000000 screenlogicpy-0.8.2/screenlogicpy/requests/login.py
--rw-rw-rw-   0        0        0      326 2023-03-06 20:33:38.000000 screenlogicpy-0.8.2/screenlogicpy/requests/ping.py
--rw-rw-rw-   0        0        0    10729 2023-03-16 15:10:02.000000 screenlogicpy-0.8.2/screenlogicpy/requests/protocol.py
--rw-rw-rw-   0        0        0     2921 2023-03-05 23:13:04.000000 screenlogicpy-0.8.2/screenlogicpy/requests/pump.py
--rw-rw-rw-   0        0        0     2229 2023-03-16 15:10:02.000000 screenlogicpy-0.8.2/screenlogicpy/requests/request.py
--rw-rw-rw-   0        0        0     2244 2023-03-05 23:13:04.000000 screenlogicpy-0.8.2/screenlogicpy/requests/scg.py
--rw-rw-rw-   0        0        0     6771 2023-03-05 23:13:04.000000 screenlogicpy-0.8.2/screenlogicpy/requests/status.py
--rw-rw-rw-   0        0        0     4204 2023-03-12 18:03:52.000000 screenlogicpy-0.8.2/screenlogicpy/requests/utility.py
-drwxrwxrwx   0        0        0        0 2023-03-16 15:42:03.509004 screenlogicpy-0.8.2/screenlogicpy.egg-info/
--rw-rw-rw-   0        0        0    27105 2023-03-16 15:42:03.000000 screenlogicpy-0.8.2/screenlogicpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1150 2023-03-16 15:42:03.000000 screenlogicpy-0.8.2/screenlogicpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-16 15:42:03.000000 screenlogicpy-0.8.2/screenlogicpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-03-16 15:42:03.000000 screenlogicpy-0.8.2/screenlogicpy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       21 2023-03-16 15:42:03.000000 screenlogicpy-0.8.2/screenlogicpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-03-16 15:42:03.000000 screenlogicpy-0.8.2/screenlogicpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-16 15:42:03.549002 screenlogicpy-0.8.2/setup.cfg
--rw-rw-rw-   0        0        0     1171 2023-03-16 15:10:02.000000 screenlogicpy-0.8.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-16 15:42:03.546003 screenlogicpy-0.8.2/tests/
--rw-rw-rw-   0        0        0     5770 2023-03-04 09:17:37.000000 screenlogicpy-0.8.2/tests/test_cli.py
--rw-rw-rw-   0        0        0     5635 2023-03-16 15:10:02.000000 screenlogicpy-0.8.2/tests/test_client.py
--rw-rw-rw-   0        0        0     1861 2022-06-17 08:22:16.000000 screenlogicpy-0.8.2/tests/test_decode.py
--rw-rw-rw-   0        0        0     1374 2021-11-08 00:04:54.000000 screenlogicpy-0.8.2/tests/test_discovery.py
--rw-rw-rw-   0        0        0     9102 2023-03-16 15:10:02.000000 screenlogicpy-0.8.2/tests/test_gateway.py
--rw-rw-rw-   0        0        0     3407 2023-03-16 15:10:02.000000 screenlogicpy-0.8.2/tests/test_login.py
--rw-rw-rw-   0        0        0     2641 2023-03-16 15:10:02.000000 screenlogicpy-0.8.2/tests/test_protocol.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:09:41.145745 screenlogicpy-0.9.0/
+-rw-rw-rw-   0        0        0    35803 2020-01-02 07:35:49.000000 screenlogicpy-0.9.0/LICENSE
+-rw-rw-rw-   0        0        0    29010 2023-05-04 07:09:41.145745 screenlogicpy-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0    28299 2023-05-04 03:20:05.000000 screenlogicpy-0.9.0/README.md
+-rw-rw-rw-   0        0        0      108 2021-11-08 00:04:54.000000 screenlogicpy-0.9.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-04 07:09:41.074744 screenlogicpy-0.9.0/screenlogicpy/
+-rw-rw-rw-   0        0        0      232 2023-05-03 06:01:03.000000 screenlogicpy-0.9.0/screenlogicpy/__init__.py
+-rw-rw-rw-   0        0        0      384 2023-03-26 07:00:05.000000 screenlogicpy-0.9.0/screenlogicpy/__main__.py
+-rw-rw-rw-   0        0        0    18425 2023-05-03 06:01:03.000000 screenlogicpy-0.9.0/screenlogicpy/cli.py
+-rw-rw-rw-   0        0        0     7946 2023-05-03 06:01:03.000000 screenlogicpy-0.9.0/screenlogicpy/client.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:09:41.102742 screenlogicpy-0.9.0/screenlogicpy/const/
+-rw-rw-rw-   0        0        0       95 2023-05-03 06:01:03.000000 screenlogicpy-0.9.0/screenlogicpy/const/__init__.py
+-rw-rw-rw-   0        0        0     3022 2023-05-03 06:01:03.000000 screenlogicpy-0.9.0/screenlogicpy/const/common.py
+-rw-rw-rw-   0        0        0     4074 2023-05-03 06:01:03.000000 screenlogicpy-0.9.0/screenlogicpy/const/data.py
+-rw-rw-rw-   0        0        0     1099 2023-05-03 06:01:03.000000 screenlogicpy-0.9.0/screenlogicpy/const/msg.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:09:41.112743 screenlogicpy-0.9.0/screenlogicpy/device_const/
+-rw-rw-rw-   0        0        0        0 2023-05-03 06:01:03.000000 screenlogicpy-0.9.0/screenlogicpy/device_const/__init__.py
+-rw-rw-rw-   0        0        0     1709 2023-05-03 06:01:03.000000 screenlogicpy-0.9.0/screenlogicpy/device_const/chemistry.py
+-rw-rw-rw-   0        0        0      857 2023-05-03 06:01:03.000000 screenlogicpy-0.9.0/screenlogicpy/device_const/circuit.py
+-rw-rw-rw-   0        0        0      347 2023-05-03 06:01:03.000000 screenlogicpy-0.9.0/screenlogicpy/device_const/heat.py
+-rw-rw-rw-   0        0        0      262 2023-05-03 06:01:03.000000 screenlogicpy-0.9.0/screenlogicpy/device_const/pump.py
+-rw-rw-rw-   0        0        0      114 2023-05-03 06:01:03.000000 screenlogicpy-0.9.0/screenlogicpy/device_const/scg.py
+-rw-rw-rw-   0        0        0     2268 2023-05-03 06:01:03.000000 screenlogicpy-0.9.0/screenlogicpy/device_const/system.py
+-rw-rw-rw-   0        0        0     3851 2023-05-03 06:01:03.000000 screenlogicpy-0.9.0/screenlogicpy/discovery.py
+-rw-rw-rw-   0        0        0    18490 2023-05-03 06:01:03.000000 screenlogicpy-0.9.0/screenlogicpy/gateway.py
+-rw-rw-rw-   0        0        0      910 2023-05-03 06:01:03.000000 screenlogicpy-0.9.0/screenlogicpy/path_dict.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:09:41.134743 screenlogicpy-0.9.0/screenlogicpy/requests/
+-rw-rw-rw-   0        0        0      804 2023-03-22 16:11:06.000000 screenlogicpy-0.9.0/screenlogicpy/requests/__init__.py
+-rw-rw-rw-   0        0        0      514 2023-05-03 06:01:03.000000 screenlogicpy-0.9.0/screenlogicpy/requests/button.py
+-rw-rw-rw-   0        0        0    11047 2023-05-03 06:01:03.000000 screenlogicpy-0.9.0/screenlogicpy/requests/chemistry.py
+-rw-rw-rw-   0        0        0      944 2023-05-03 06:01:03.000000 screenlogicpy-0.9.0/screenlogicpy/requests/client.py
+-rw-rw-rw-   0        0        0     5302 2023-05-03 06:01:03.000000 screenlogicpy-0.9.0/screenlogicpy/requests/config.py
+-rw-rw-rw-   0        0        0     1720 2023-05-03 06:01:03.000000 screenlogicpy-0.9.0/screenlogicpy/requests/equipment.py
+-rw-rw-rw-   0        0        0      716 2023-05-03 06:01:04.000000 screenlogicpy-0.9.0/screenlogicpy/requests/gateway.py
+-rw-rw-rw-   0        0        0      855 2023-05-03 06:01:04.000000 screenlogicpy-0.9.0/screenlogicpy/requests/heat.py
+-rw-rw-rw-   0        0        0     1057 2023-05-03 06:01:04.000000 screenlogicpy-0.9.0/screenlogicpy/requests/lights.py
+-rw-rw-rw-   0        0        0     4538 2023-05-03 06:01:04.000000 screenlogicpy-0.9.0/screenlogicpy/requests/login.py
+-rw-rw-rw-   0        0        0      330 2023-05-03 06:01:04.000000 screenlogicpy-0.9.0/screenlogicpy/requests/ping.py
+-rw-rw-rw-   0        0        0    10730 2023-05-03 06:01:04.000000 screenlogicpy-0.9.0/screenlogicpy/requests/protocol.py
+-rw-rw-rw-   0        0        0     3521 2023-05-03 06:01:04.000000 screenlogicpy-0.9.0/screenlogicpy/requests/pump.py
+-rw-rw-rw-   0        0        0     2266 2023-05-03 06:01:04.000000 screenlogicpy-0.9.0/screenlogicpy/requests/request.py
+-rw-rw-rw-   0        0        0     3075 2023-05-03 06:01:04.000000 screenlogicpy-0.9.0/screenlogicpy/requests/scg.py
+-rw-rw-rw-   0        0        0     8052 2023-05-03 06:01:04.000000 screenlogicpy-0.9.0/screenlogicpy/requests/status.py
+-rw-rw-rw-   0        0        0     4286 2023-05-03 06:01:04.000000 screenlogicpy-0.9.0/screenlogicpy/requests/utility.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:09:41.098742 screenlogicpy-0.9.0/screenlogicpy.egg-info/
+-rw-rw-rw-   0        0        0    29010 2023-05-04 07:09:41.000000 screenlogicpy-0.9.0/screenlogicpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1529 2023-05-04 07:09:41.000000 screenlogicpy-0.9.0/screenlogicpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 07:09:41.000000 screenlogicpy-0.9.0/screenlogicpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-05-04 07:09:41.000000 screenlogicpy-0.9.0/screenlogicpy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       21 2023-05-04 07:09:41.000000 screenlogicpy-0.9.0/screenlogicpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-04 07:09:41.000000 screenlogicpy-0.9.0/screenlogicpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 07:09:41.145745 screenlogicpy-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     1121 2023-05-03 06:01:04.000000 screenlogicpy-0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:09:41.143744 screenlogicpy-0.9.0/tests/
+-rw-rw-rw-   0        0        0     5854 2023-05-03 06:01:04.000000 screenlogicpy-0.9.0/tests/test_cli.py
+-rw-rw-rw-   0        0        0     5672 2023-05-03 06:01:04.000000 screenlogicpy-0.9.0/tests/test_client.py
+-rw-rw-rw-   0        0        0     1894 2023-05-03 06:01:04.000000 screenlogicpy-0.9.0/tests/test_decode.py
+-rw-rw-rw-   0        0        0     1374 2021-11-08 00:04:54.000000 screenlogicpy-0.9.0/tests/test_discovery.py
+-rw-rw-rw-   0        0        0    12345 2023-05-03 06:01:04.000000 screenlogicpy-0.9.0/tests/test_gateway.py
+-rw-rw-rw-   0        0        0     3457 2023-05-03 06:01:04.000000 screenlogicpy-0.9.0/tests/test_login.py
+-rw-rw-rw-   0        0        0     2619 2023-05-03 06:01:04.000000 screenlogicpy-0.9.0/tests/test_protocol.py
```

### Comparing `screenlogicpy-0.8.2/LICENSE` & `screenlogicpy-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `screenlogicpy-0.8.2/PKG-INFO` & `screenlogicpy-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: screenlogicpy
-Version: 0.8.2
+Version: 0.9.0
 Summary: Interface for Pentair ScreenLogic connected pool controllers over IP via Python
 Home-page: https://github.com/dieselrabbit/screenlogicpy
 Author: Kevin Worrel
 Author-email: kevinworrel@yahoo.com
 License: GPLv3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # screenlogicpy
 
 ![PyPI](https://img.shields.io/pypi/v/screenlogicpy) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/screenlogicpy)
 
@@ -30,27 +29,28 @@
 ```shell
 $ pip install screenlogicpy
 ```
 
 # Library usage
 
 * _Changed in v0.5.0: The screenlogicpy library has moved over to using asyncio for all network I/O. Relevant methods now require the `async`/`await` syntax._
-* _**New in v0.8.0**: Support for Python 3.8 and 3.9 is being phased out across future releases. This will be the last version to support Python 3.8._
+* _New in v0.8.0: Support for Python 3.8 and 3.9 is being phased out across future releases. Version 0.8.x will be the last versions to support Python 3.8._
+* _**New in v0.9.0**: Support for Python 3.8 has been removed. Support for Python 3.9 is being phased out across future releases. Version 0.9.x will be the last versions to support Python 3.9._
 
 The `ScreenLogicGateway` class is the primary interface.
 
 ```python
 from screenlogicpy import ScreenLogicGateway
 
     gateway = ScreenLogicGateway()
 ```
 
 * _Changed in v0.5.0: Instantiating the gateway no longer automatically connects to the protocol adapter or performs an initial update._  
 * _Changed in v0.7.0: Passing adapter connection info when instantiating the gateway is deprecated and will be removed in a future release. Connection info should be passed to `async_connect()` instead._  
-* _**Changed in v0.8.0:** Support for passing connection info to gateway constructor is fully deprecated and has been removed. Ability to specify client id used for push subscriptions, and to specify maximum number of times to retry a request has replaced it._
+* _Changed in v0.8.0: Support for passing connection info to gateway constructor is fully deprecated and has been removed. Ability to specify client id used for push subscriptions, and to specify maximum number of times to retry a request has replaced it._
 
 ## Connecting to a ScreenLogic Protocol Adapter
 
 Once instantiated, use `async_connect()` to connect and login to the ScreenLogic protocol adapter, and gather the pool configuration.
 
 If disconnected, this method may be called without any parameters to reconnect with the previous connection info, or with new parameters to connect to a different host.
 
@@ -145,14 +145,60 @@
 
 The `ScreenLogicGateway` class caches all data from the ScreenLogic protocol adapter as a single `dict` object for continued reference by the consuming application. This includes any data processed via push or polling. The consuming application may get this data at anytime with the `get_data()` method.
 
 ```python
 data = gateway.get_data()
 ```
 
+`get_data()` now supports specifying a path directly to the data desired. A path can be any length. By default, if the data path is not found, `get_data()` will return `None`, similar to `dict.get()`. Alternatively `strict=True` keyword argument can be added to force the `ScreenLogicGateway` to raise a `KeyError` exception if the path is not found.
+
+The majority of data points normally available to the end-user via the official apps are presented as `dict` objects containing "name" and "value" keys/pairs. Additional keys may be present depending on the type of data.
+
+For example, let's consider the following scenario:
+
+```python
+gateway._data = {
+    "controller": {
+        "sensor": {
+            "air_temperature": {
+                "name": "Air Temperature",
+                "value": 57,
+                "unit": "Â°F",
+                "device_type": "temperature",
+                "state_type": "measurement",
+            },
+        }
+    }
+}
+data_path = ("controller", "sensor", "air_temperature")
+
+temperature_sensor = gateway.get_data(*data_path)
+```
+
+Here, `temperature_sensor` would be a `dict` of all key/value pairs under the "air_temperature" key.
+
+The `ScreenLogicGateway` also provides shortcut methods `get_name()` and `get_value()` to get the "name" or "value" values respectively from the specified data path.
+
+```python
+# sensor_value = 57
+sensor_value = gateway.get_value(*data_path)
+
+# sensor_name = "Air Temperature"
+sensor_name = gateway.get_name(*data_path)
+```
+
+To get other values directly, use `get_data()` with the full key path:
+
+```python
+# sensor_unit = "Â°F"
+sensor_unit = gateway.get_data("controller", "sensor", "air_temperature", "unit")
+```
+
+* _**New in v0.9.0**._
+
 ## Disconnecting
 
 When done, use `async_disconnect()` to unsubscribe from push updates and close the connection to the protocol adapter.
 
 ```python
 await gateway.async_disconnect()  
 ```
```

### Comparing `screenlogicpy-0.8.2/README.md` & `screenlogicpy-0.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -11,27 +11,28 @@
 ```shell
 $ pip install screenlogicpy
 ```
 
 # Library usage
 
 * _Changed in v0.5.0: The screenlogicpy library has moved over to using asyncio for all network I/O. Relevant methods now require the `async`/`await` syntax._
-* _**New in v0.8.0**: Support for Python 3.8 and 3.9 is being phased out across future releases. This will be the last version to support Python 3.8._
+* _New in v0.8.0: Support for Python 3.8 and 3.9 is being phased out across future releases. Version 0.8.x will be the last versions to support Python 3.8._
+* _**New in v0.9.0**: Support for Python 3.8 has been removed. Support for Python 3.9 is being phased out across future releases. Version 0.9.x will be the last versions to support Python 3.9._
 
 The `ScreenLogicGateway` class is the primary interface.
 
 ```python
 from screenlogicpy import ScreenLogicGateway
 
     gateway = ScreenLogicGateway()
 ```
 
 * _Changed in v0.5.0: Instantiating the gateway no longer automatically connects to the protocol adapter or performs an initial update._  
 * _Changed in v0.7.0: Passing adapter connection info when instantiating the gateway is deprecated and will be removed in a future release. Connection info should be passed to `async_connect()` instead._  
-* _**Changed in v0.8.0:** Support for passing connection info to gateway constructor is fully deprecated and has been removed. Ability to specify client id used for push subscriptions, and to specify maximum number of times to retry a request has replaced it._
+* _Changed in v0.8.0: Support for passing connection info to gateway constructor is fully deprecated and has been removed. Ability to specify client id used for push subscriptions, and to specify maximum number of times to retry a request has replaced it._
 
 ## Connecting to a ScreenLogic Protocol Adapter
 
 Once instantiated, use `async_connect()` to connect and login to the ScreenLogic protocol adapter, and gather the pool configuration.
 
 If disconnected, this method may be called without any parameters to reconnect with the previous connection info, or with new parameters to connect to a different host.
 
@@ -126,14 +127,60 @@
 
 The `ScreenLogicGateway` class caches all data from the ScreenLogic protocol adapter as a single `dict` object for continued reference by the consuming application. This includes any data processed via push or polling. The consuming application may get this data at anytime with the `get_data()` method.
 
 ```python
 data = gateway.get_data()
 ```
 
+`get_data()` now supports specifying a path directly to the data desired. A path can be any length. By default, if the data path is not found, `get_data()` will return `None`, similar to `dict.get()`. Alternatively `strict=True` keyword argument can be added to force the `ScreenLogicGateway` to raise a `KeyError` exception if the path is not found.
+
+The majority of data points normally available to the end-user via the official apps are presented as `dict` objects containing "name" and "value" keys/pairs. Additional keys may be present depending on the type of data.
+
+For example, let's consider the following scenario:
+
+```python
+gateway._data = {
+    "controller": {
+        "sensor": {
+            "air_temperature": {
+                "name": "Air Temperature",
+                "value": 57,
+                "unit": "°F",
+                "device_type": "temperature",
+                "state_type": "measurement",
+            },
+        }
+    }
+}
+data_path = ("controller", "sensor", "air_temperature")
+
+temperature_sensor = gateway.get_data(*data_path)
+```
+
+Here, `temperature_sensor` would be a `dict` of all key/value pairs under the "air_temperature" key.
+
+The `ScreenLogicGateway` also provides shortcut methods `get_name()` and `get_value()` to get the "name" or "value" values respectively from the specified data path.
+
+```python
+# sensor_value = 57
+sensor_value = gateway.get_value(*data_path)
+
+# sensor_name = "Air Temperature"
+sensor_name = gateway.get_name(*data_path)
+```
+
+To get other values directly, use `get_data()` with the full key path:
+
+```python
+# sensor_unit = "°F"
+sensor_unit = gateway.get_data("controller", "sensor", "air_temperature", "unit")
+```
+
+* _**New in v0.9.0**._
+
 ## Disconnecting
 
 When done, use `async_disconnect()` to unsubscribe from push updates and close the connection to the protocol adapter.
 
 ```python
 await gateway.async_disconnect()  
 ```
```

### Comparing `screenlogicpy-0.8.2/screenlogicpy/cli.py` & `screenlogicpy-0.9.0/screenlogicpy/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import asyncio
 import string
 import json
 import argparse
 from screenlogicpy.discovery import async_discover
 from screenlogicpy.gateway import ScreenLogicGateway
-from screenlogicpy.const import (
-    BODY_TYPE,
-    COLOR_MODE,
-    CHEMISTRY,
-    DATA,
-    EQUIPMENT,
-    HEAT_MODE,
+from screenlogicpy.const.common import (
     ON_OFF,
     RANGE,
     SL_GATEWAY_IP,
     SL_GATEWAY_NAME,
     SL_GATEWAY_PORT,
+    SLIntEnum,
     ScreenLogicError,
     ScreenLogicWarning,
 )
+from screenlogicpy.device_const.chemistry import RANGE_ORP_SETPOINT, RANGE_PH_SETPOINT
+from screenlogicpy.device_const.heat import HEAT_MODE
+from screenlogicpy.device_const.system import BODY_TYPE, COLOR_MODE
+from screenlogicpy.const.data import ATTR, DEVICE, GROUP, VALUE
 
 
 def cliFormat(name: str):
     table = str.maketrans(" ", "_", string.punctuation)
     return name.translate(table).lower()
 
 
@@ -47,218 +46,207 @@
 # Entry function
 async def cli(cli_args):
     """Handle command line args"""
 
     def vFormat(slElement: dict, slClass=None):
         if args.verbose:
             if slClass:
-                return (
-                    f"{slElement['name']}: {slClass.NAME_FOR_NUM[slElement['value']]}"
-                )
+                if issubclass(slClass, SLIntEnum):
+                    return f"{slElement[ATTR.NAME]}: {slClass(slElement[ATTR.VALUE]).title}"
+                else:
+                    return f"{slElement[ATTR.NAME]}: {slClass.NAME_FOR_NUM[slElement[ATTR.VALUE]]}"
             else:
-                return f"{slElement['name']}: {slElement['value']}"
+                return f"{slElement[ATTR.NAME]}: {slElement[ATTR.VALUE]}"
         else:
-            return slElement["value"]
+            if slClass and issubclass(slClass, SLIntEnum):
+                return slClass(slElement[ATTR.VALUE]).value
+            else:
+                return slElement[ATTR.VALUE]
 
     # Parser functions
     async def async_get_circuit():
-        if not int(args.circuit_num) in gateway.get_data()[DATA.KEY_CIRCUITS]:
+        circuit_id = int(args.circuit_num)
+        if circuit_id not in gateway.get_data(DEVICE.CIRCUIT):
             print(f"Invalid circuit number: {args.circuit_num}")
             return 4
         print(
             vFormat(
-                gateway.get_data()[DATA.KEY_CIRCUITS][int(args.circuit_num)],
+                gateway.get_data(DEVICE.CIRCUIT, circuit_id),
                 ON_OFF,
             )
         )
         return 0
 
     async def async_set_circuit():
-        state = 0
-        if args.state == "1" or args.state.lower() == "on":
-            state = 1
-        if not int(args.circuit_num) in gateway.get_data()[DATA.KEY_CIRCUITS]:
+        state = ON_OFF.parse(args.state).value
+        circuit_id = int(args.circuit_num)
+        if circuit_id not in gateway.get_data(DEVICE.CIRCUIT):
             print(f"Invalid circuit number: {args.circuit_num}")
             return 4
-        if await gateway.async_set_circuit(int(args.circuit_num), state):
+        if await gateway.async_set_circuit(circuit_id, state):
             await gateway.async_update()
         else:
             return 4
         print(
             vFormat(
-                gateway.get_data()[DATA.KEY_CIRCUITS][int(args.circuit_num)],
+                gateway.get_data(DEVICE.CIRCUIT, circuit_id),
                 ON_OFF,
             )
         )
         return 0
 
     async def async_get_heat_mode():
-        body = 0
-        if args.body == "1" or args.body.lower() == "spa":
-            body = 1
+        body = BODY_TYPE.parse(args.body).value
         print(
             vFormat(
-                gateway.get_data()[DATA.KEY_BODIES][int(body)]["heat_mode"],
+                gateway.get_data(DEVICE.BODY, int(body), VALUE.HEAT_MODE),
                 HEAT_MODE,
             )
         )
         return 0
 
     async def async_set_heat_mode():
-        body = 0
-        mode = 0
-        if args.body == "1" or args.body.lower() == "spa":
-            body = 1
-        if args.mode in cliFormatDict(HEAT_MODE.NUM_FOR_NAME):
-            mode = cliFormatDict(HEAT_MODE.NUM_FOR_NAME)[args.mode]
-        else:
-            mode = int(args.mode)
-        if await gateway.async_set_heat_mode(int(body), mode):
+        body = BODY_TYPE.parse(args.body).value
+        mode = HEAT_MODE.parse(args.mode).value
+        if await gateway.async_set_heat_mode(body, mode):
             await gateway.async_update()
         else:
             return 8
         print(
             vFormat(
-                gateway.get_data()[DATA.KEY_BODIES][int(body)]["heat_mode"],
+                gateway.get_data(DEVICE.BODY, body, VALUE.HEAT_MODE),
                 HEAT_MODE,
             )
         )
         return 0
 
     async def async_get_heat_temp():
-        body = 0
-        if args.body == "1" or args.body.lower() == "spa":
-            body = 1
+        body = BODY_TYPE.parse(args.body).value
         print(
             vFormat(
-                gateway.get_data()[DATA.KEY_BODIES][int(body)]["heat_set_point"],
+                gateway.get_data(DEVICE.BODY, body, VALUE.HEAT_SETPOINT),
             )
         )
         return 0
 
     async def async_set_heat_temp():
-        body = 0
-        if args.body == "1" or args.body.lower() == "spa":
-            body = 1
+        body = BODY_TYPE.parse(args.body).value
         if args.temp != -1:
-            if await gateway.async_set_heat_temp(int(body), int(args.temp)):
+            if await gateway.async_set_heat_temp(body, int(args.temp)):
                 await gateway.async_update()
             else:
                 return 16
         print(
             vFormat(
-                gateway.get_data()[DATA.KEY_BODIES][int(body)]["heat_set_point"],
+                gateway.get_data(DEVICE.BODY, body, VALUE.HEAT_SETPOINT),
             )
         )
         return 0
 
     async def async_get_heat_state():
-        body = 0
-        if args.body == "1" or args.body.lower() == "spa":
-            body = 1
+        body = BODY_TYPE.parse(args.body).value
         print(
             vFormat(
-                gateway.get_data()[DATA.KEY_BODIES][int(body)]["heat_status"],
+                gateway.get_data(DEVICE.BODY, body, VALUE.HEAT_STATE),
                 ON_OFF,
             )
         )
         return 0
 
     async def async_get_current_temp():
-        body = 0
-        if args.body == "1" or args.body.lower() == "spa":
-            body = 1
+        body = BODY_TYPE.parse(args.body)
         print(
             vFormat(
-                gateway.get_data()[DATA.KEY_BODIES][int(body)]["last_temperature"],
+                gateway.get_data(DEVICE.BODY, body, VALUE.LAST_TEMPERATURE),
             )
         )
         return 0
 
     async def async_set_color_light():
-        mode = cliFormatDict(COLOR_MODE.NUM_FOR_NAME).get(args.mode)
+        mode = COLOR_MODE.parse(args.mode).value
         if mode is None:
             mode = int(args.mode)
         if await gateway.async_set_color_lights(mode):
             print(
-                f"Set color mode to {COLOR_MODE.NAME_FOR_NUM[mode]}"
-                if args.verbose
-                else mode
+                f"Set color mode to {COLOR_MODE(mode).title}" if args.verbose else mode
             )
             return 0
         return 32
 
     async def async_set_scg_config():
         if args.scg_pool == "*" and args.scg_spa == "*":
-            print("No new SCG values. Nothing to do.")
+            print("No new Chlorinator values. Nothing to do.")
             return 65
 
-        scg_data = gateway.get_data()[DATA.KEY_SCG]
+        scg_config_data = gateway.get_data(DEVICE.SCG, GROUP.CONFIGURATION)
         try:
             scg_1 = (
-                scg_data["scg_level1"]["value"]
+                scg_config_data[VALUE.POOL_SETPOINT][ATTR.VALUE]
                 if args.scg_pool == "*"
                 else int(args.scg_pool)
             )
             scg_2 = (
-                scg_data["scg_level2"]["value"]
+                scg_config_data[VALUE.SPA_SETPOINT][ATTR.VALUE]
                 if args.scg_spa == "*"
                 else int(args.scg_spa)
             )
         except ValueError:
-            print("Invalid SCG value")
+            print("Invalid Chlorinator value")
             return 66
 
         if await gateway.async_set_scg_config(scg_1, scg_2):
             await gateway.async_update()
-            new_data = gateway.get_data()
+            new_scg_config_data = gateway.get_data(DEVICE.SCG, GROUP.CONFIGURATION)
             print(
-                vFormat(new_data[DATA.KEY_SCG]["scg_level1"]),
-                vFormat(new_data[DATA.KEY_SCG]["scg_level2"]),
+                vFormat(new_scg_config_data[VALUE.POOL_SETPOINT]),
+                vFormat(new_scg_config_data[VALUE.SPA_SETPOINT]),
             )
             return 0
         return 64
 
     async def async_set_chem_data():
         if args.ph_setpoint == "*" and args.orp_setpoint == "*":
             print("No new setpoint values. Nothing to do.")
             return 129
 
-        chem_data = gateway.get_data()[DATA.KEY_CHEMISTRY]
+        chem_config_data = gateway.get_data(DEVICE.INTELLICHEM, GROUP.CONFIGURATION)
         try:
             ph = (
-                chem_data["ph_setpoint"]["value"]
+                chem_config_data[VALUE.PH_SETPOINT][ATTR.VALUE]
                 if args.ph_setpoint == "*"
                 else float(args.ph_setpoint)
             )
             orp = (
-                chem_data["orp_setpoint"]["value"]
+                chem_config_data[VALUE.ORP_SETPOINT][ATTR.VALUE]
                 if args.orp_setpoint == "*"
                 else int(args.orp_setpoint)
             )
         except ValueError:
             print("Invalid Chemistry Setpoint value")
             return 130
 
-        ch = chem_data["calcium_harness"]["value"]
-        ta = chem_data["total_alkalinity"]["value"]
-        ca = chem_data["cya"]["value"]
-        sa = chem_data["salt_tds_ppm"]["value"]
+        ch = chem_config_data[VALUE.CALCIUM_HARNESS][ATTR.VALUE]
+        ta = chem_config_data[VALUE.TOTAL_ALKALINITY][ATTR.VALUE]
+        ca = chem_config_data[VALUE.CYA][ATTR.VALUE]
+        sa = chem_config_data[VALUE.SALT_TDS_PPM][ATTR.VALUE]
 
         if await gateway.async_set_chem_data(ph, orp, ch, ta, ca, sa):
             await asyncio.sleep(3)
             await gateway.async_update()
-            new_data = gateway.get_data()
+            new_chem_config_data = gateway.get_data(
+                DEVICE.INTELLICHEM, GROUP.CONFIGURATION
+            )
             print(
-                vFormat(new_data[DATA.KEY_CHEMISTRY]["ph_setpoint"]),
-                vFormat(new_data[DATA.KEY_CHEMISTRY]["orp_setpoint"]),
+                vFormat(new_chem_config_data[VALUE.PH_SETPOINT]),
+                vFormat(new_chem_config_data[VALUE.ORP_SETPOINT]),
             )
             return 0
         return 128
 
+    # Begin Parser Setup
     async def async_get_json():
         print(json.dumps(gateway.get_data(), indent=2))
         return 0
 
     option_parser = argparse.ArgumentParser(
         description="Interface for Pentair Screenlogic gateway"
     )
@@ -286,15 +274,15 @@
         "type": int,
         "help": "Circuit number",
     }
     get_circuit_parser = get_subparsers.add_parser("circuit", aliases=["c"])
     get_circuit_parser.add_argument(**ARGUMENT_CIRCUIT_NUM)
     get_circuit_parser.set_defaults(async_func=async_get_circuit)
 
-    body_options = optionsFromDict(BODY_TYPE.NAME_FOR_NUM)
+    body_options = BODY_TYPE.parsable()
     ARGUMENT_BODY = {
         "dest": "body",
         "metavar": "BODY",
         "type": str,
         "choices": body_options,
         "help": f"Body of water. One of: {body_options}",
     }
@@ -318,40 +306,40 @@
     get_json_parser.set_defaults(async_func=async_get_json)
 
     # Set options
     set_parser = subparsers.add_parser("set")
     set_subparsers = set_parser.add_subparsers(dest="set_option")
     set_subparsers.required = True
 
-    on_off_options = optionsFromDict(ON_OFF.NAME_FOR_NUM)
+    on_off_options = ON_OFF.parsable()
     set_circuit_parser = set_subparsers.add_parser("circuit", aliases=["c"])
     set_circuit_parser.add_argument(**ARGUMENT_CIRCUIT_NUM)
     set_circuit_parser.add_argument(
         "state",
         metavar="STATE",
         type=str,
         choices=on_off_options,
         help=f"State to set. One of {on_off_options}",
     )
 
-    cl_options = optionsFromDict(COLOR_MODE.NAME_FOR_NUM)
+    cl_options = COLOR_MODE.parsable()
     set_circuit_parser.set_defaults(async_func=async_set_circuit)
     set_color_light_parser = set_subparsers.add_parser("color-lights", aliases=["cl"])
     set_color_light_parser.add_argument(
         "mode",
         metavar="MODE",
         type=str,
         choices=cl_options,
         help=f"Color lights command, color or show. One of :{cl_options}",
     )
     set_color_light_parser.set_defaults(async_func=async_set_color_light)
 
     set_heat_mode_parser = set_subparsers.add_parser("heat-mode", aliases=["hm"])
     set_heat_mode_parser.add_argument(**ARGUMENT_BODY)
-    hm_options = optionsFromDict(HEAT_MODE.NAME_FOR_NUM)
+    hm_options = HEAT_MODE.parsable()
     set_heat_mode_parser.add_argument(
         "mode",
         metavar="MODE",
         type=str,
         choices=hm_options,
         default=hm_options[0],
         help=f"Heat mode to set. One of: {hm_options}",
@@ -388,22 +376,22 @@
 
     set_chem_data_parser = set_subparsers.add_parser("chem-data", aliases=["ch"])
     set_chem_data_parser.add_argument(
         "ph_setpoint",
         type=str,
         metavar="PH_SETPOINT",
         default=None,
-        help=f"PH set point for IntelliChem. {CHEMISTRY.RANGE_PH_SETPOINT[RANGE.MIN]}-{CHEMISTRY.RANGE_PH_SETPOINT[RANGE.MAX]}, or * to keep current value.",
+        help=f"PH set point for IntelliChem. {RANGE_PH_SETPOINT[RANGE.MIN]}-{RANGE_PH_SETPOINT[RANGE.MAX]}, or * to keep current value.",
     )
     set_chem_data_parser.add_argument(
         "orp_setpoint",
         type=str,
         metavar="ORP_SETPOINT",
         default=None,
-        help=f"ORP set point for IntelliChem. {CHEMISTRY.RANGE_ORP_SETPOINT[RANGE.MIN]}-{CHEMISTRY.RANGE_ORP_SETPOINT[RANGE.MAX]}, or * to keep current value.",
+        help=f"ORP set point for IntelliChem. {RANGE_ORP_SETPOINT[RANGE.MIN]}-{RANGE_ORP_SETPOINT[RANGE.MAX]}, or * to keep current value.",
     )
     set_chem_data_parser.set_defaults(async_func=async_set_chem_data)
 
     args = option_parser.parse_args(cli_args)
 
     try:
         host = {SL_GATEWAY_IP: args.ip, SL_GATEWAY_PORT: args.port}
@@ -446,72 +434,64 @@
 
         gateway = ScreenLogicGateway()
 
         await gateway.async_connect(**host)
 
         await gateway.async_update()
 
-        if DATA.KEY_CONFIG not in gateway.get_data():
+        if DEVICE.CONTROLLER not in gateway.get_data():
             return 1
 
         def print_gateway():
-            verb = "Using"
-            if discovered:
-                verb = "Discovered"
+            verb = "Discovered" if discovered else "Using"
             print(
                 "{} '{}' at {}:{}".format(verb, gateway.name, gateway.ip, gateway.port)
             )
-            print(
-                EQUIPMENT.CONTROLLER_HARDWARE[
-                    gateway.get_data()[DATA.KEY_CONFIG]["controller_type"]
-                ][gateway.get_data()[DATA.KEY_CONFIG]["hardware_type"]]
-            )
+            print(gateway.get_value(DEVICE.CONTROLLER, VALUE.MODEL))
             if args.verbose:
                 print(f"Version: {gateway.version}")
 
         def print_circuits():
             print("{}  {}  {}".format("ID".rjust(3), "STATE", "NAME"))
             print("--------------------------")
-            for id in gateway.get_data()[DATA.KEY_CIRCUITS]:
-                circuit = gateway.get_data()[DATA.KEY_CIRCUITS][int(id)]
+            for id, circuit in gateway.get_data(DEVICE.CIRCUIT).items():
                 print(
                     "{}  {}  {}".format(
-                        circuit["id"],
-                        ON_OFF.NAME_FOR_NUM[circuit["value"]].rjust(5),
-                        circuit["name"],
+                        id,
+                        ON_OFF(circuit[ATTR.VALUE]).title.rjust(5),
+                        circuit[ATTR.NAME],
                     )
                 )
 
         def print_heat():
-            for id in gateway.get_data()[DATA.KEY_BODIES]:
-                body = gateway.get_data()[DATA.KEY_BODIES][int(id)]
+            for body in gateway.get_data(DEVICE.BODY).values():
                 print(
                     "{} temperature is last {}{}".format(
-                        BODY_TYPE.NAME_FOR_NUM[body["body_type"]["value"]],
-                        body["last_temperature"]["value"],
-                        body["last_temperature"]["unit"],
+                        BODY_TYPE(body[ATTR.BODY_TYPE]).title,
+                        body[VALUE.LAST_TEMPERATURE][ATTR.VALUE],
+                        body[VALUE.LAST_TEMPERATURE][ATTR.UNIT],
                     )
                 )
                 print(
                     "{}: {}{}".format(
-                        body["heat_set_point"]["name"],
-                        body["heat_set_point"]["value"],
-                        body["last_temperature"]["unit"],
+                        body[VALUE.HEAT_SETPOINT][ATTR.NAME],
+                        body[VALUE.HEAT_SETPOINT][ATTR.VALUE],
+                        body[VALUE.LAST_TEMPERATURE][ATTR.UNIT],
                     )
                 )
                 print(
                     "{}: {}".format(
-                        body["heat_status"]["name"],
-                        HEAT_MODE.NAME_FOR_NUM[body["heat_status"]["value"]],
+                        body[VALUE.HEAT_STATE][ATTR.NAME],
+                        HEAT_MODE(body[VALUE.HEAT_STATE][ATTR.VALUE]).title,
                     )
                 )
                 print(
                     "{}: {}".format(
-                        body["heat_mode"]["name"],
-                        HEAT_MODE.NAME_FOR_NUM[body["heat_mode"]["value"]],
+                        body[VALUE.HEAT_MODE][ATTR.NAME],
+                        HEAT_MODE(body[VALUE.HEAT_MODE][ATTR.VALUE]).title,
                     )
                 )
                 print("--------------------------")
 
         def print_dashboard():
             print_gateway()
             print("**************************")
```

### Comparing `screenlogicpy-0.8.2/screenlogicpy/client.py` & `screenlogicpy-0.9.0/screenlogicpy/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """Client manager for a connection to a ScreenLogic protocol adapter."""
 import asyncio
 import logging
 import random
-from typing import Awaitable, Callable
+from typing import Any, Awaitable, Callable
 
-from .const import (
+from .const.common import COM_KEEPALIVE, ScreenLogicRequestError
+from .const.msg import (
     CODE,
-    COM_KEEPALIVE,
-    MESSAGE,
-    ScreenLogicRequestError,
+    COM_MAX_RETRIES,
 )
 from .requests import (
     async_request_add_client,
     async_request_ping,
     async_request_remove_client,
 )
 from .requests.chemistry import decode_chemistry
@@ -24,27 +23,27 @@
 
 
 class ClientManager:
     """Class to manage callback subscriptions to specific ScreenLogic messages."""
 
     def __init__(
         self,
-        async_request_manager: Callable[[bytes, any], Awaitable[any]],
+        async_request_manager: Callable[[bytes, Any], Awaitable[Any]],
         client_id: int = None,
     ) -> None:
         self._async_managed_request = async_request_manager
         self._client_id = (
             client_id if client_id is not None else random.randint(32767, 65535)
         )
         self._listeners = {}
         self._is_client = False
         self._client_sub_unsub_lock = asyncio.Lock()
         self._protocol = None
         self._data = None
-        self._max_retries = MESSAGE.COM_MAX_RETRIES
+        self._max_retries = COM_MAX_RETRIES
 
     @property
     def is_client(self) -> bool:
         """Return if connected to ScreenLogic as a client."""
         return self._is_client and self._protocol and self._protocol.is_connected
 
     @property
@@ -59,15 +58,15 @@
     def _attached(self) -> bool:
         return self._protocol and self._protocol.is_connected
 
     async def attach(
         self,
         protocol: ScreenLogicProtocol,
         data: dict,
-        max_retries: int = MESSAGE.COM_MAX_RETRIES,
+        max_retries: int = COM_MAX_RETRIES,
     ):
         """
         Update protocol and data reference.
 
         Updates this ClientManager's reference to a ScreenLogicProtocol instance
         and a current data dict. Will attempt to re-register any existing callbacks
         to the new protocol instance.
```

### Comparing `screenlogicpy-0.8.2/screenlogicpy/discovery.py` & `screenlogicpy-0.9.0/screenlogicpy/discovery.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Discovery for screenlogic gateways."""
 import asyncio
 import ipaddress
 import logging
 import socket
 import struct
 
-from .const import (  # pylint: disable=relative-beyond-top-level
+from .const.common import (  # pylint: disable=relative-beyond-top-level
     SL_GATEWAY_IP,
     SL_GATEWAY_NAME,
     SL_GATEWAY_PORT,
     SL_GATEWAY_SUBTYPE,
     SL_GATEWAY_TYPE,
     ScreenLogicError,
 )
```

### Comparing `screenlogicpy-0.8.2/screenlogicpy/gateway.py` & `screenlogicpy-0.9.0/screenlogicpy/gateway.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """Describes a ScreenLogicGateway class for interacting with a Pentair ScreenLogic system."""
 import asyncio
 import logging
 from typing import Awaitable, Callable
 
 from .client import ClientManager
-from .const import (
-    BODY_TYPE,
-    CHEMISTRY,
-    CIRCUIT_FUNCTION,
-    DATA,
-    MESSAGE,
+from .const.common import (
+    DATA_REQUEST,
     RANGE,
-    SCG,
     ScreenLogicError,
     ScreenLogicRequestError,
 )
+from .const.msg import COM_MAX_RETRIES
+from .device_const.chemistry import RANGE_PH_SETPOINT, RANGE_ORP_SETPOINT
+from .device_const.system import BODY_TYPE, EQUIPMENT_FLAG
+from .device_const.scg import LIMIT_FOR_BODY
+from .const.data import ATTR, DEVICE, GROUP, VALUE
 from .requests import (
     async_connect_to_gateway,
     async_request_gateway_version,
     async_request_pool_button_press,
     async_request_pool_config,
     async_request_pool_lights_command,
     async_request_pool_status,
@@ -28,14 +28,15 @@
     async_request_chemistry,
     async_request_scg_config,
     async_request_set_scg_config,
     async_request_set_chem_data,
     async_make_request,
 )
 from .requests.protocol import ScreenLogicProtocol
+from .requests.utility import getTemperatureUnit
 
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class ScreenLogicGateway:
     """Class for interacting and communicating with a ScreenLogic protocol adapter."""
@@ -72,15 +73,29 @@
 
     @property
     def mac(self) -> str:
         return self._mac
 
     @property
     def version(self) -> str:
-        return self._version
+        return self.get_value(DEVICE.ADAPTER, VALUE.FIRMWARE)
+
+    @property
+    def controller_model(self) -> str:
+        return self.get_value(DEVICE.CONTROLLER, VALUE.MODEL)
+
+    @property
+    def equipment_flags(self) -> EQUIPMENT_FLAG:
+        return EQUIPMENT_FLAG(
+            self.get_data(DEVICE.CONTROLLER, GROUP.EQUIPMENT, VALUE.FLAGS)
+        )
+
+    @property
+    def temperature_unit(self) -> str:
+        return getTemperatureUnit(self._data)
 
     @property
     def is_connected(self) -> bool:
         return self._protocol._connected if self._protocol else False
 
     @property
     def is_client(self) -> bool:
@@ -124,18 +139,18 @@
             self._ip,
             self._port,
             self._common_connection_closed_callback,
             self._max_retries,
         )
         if connectPkg:
             self._transport, self._protocol, self._mac = connectPkg
-            self._version = await async_request_gateway_version(
-                self._protocol, self._max_retries
+            await async_request_gateway_version(
+                self._protocol, self._data, self._max_retries
             )
-            if self._version:
+            if self.version:
                 _LOGGER.debug("Login successful")
                 await self.async_get_config()
                 await self._client_manager.attach(
                     self._protocol, self.get_data(), self._max_retries
                 )
                 return True
         _LOGGER.debug("Login failed")
@@ -168,60 +183,120 @@
 
     async def async_get_config(self):
         """Request pool configuration data."""
         _LOGGER.debug("Requesting config data")
         if last_raw := await self._async_connected_request(
             async_request_pool_config, self._data, reconnect_delay=1
         ):
-            self._last[DATA.KEY_CONFIG] = last_raw
+            self._last[DATA_REQUEST.CONFIG] = last_raw
 
     async def async_get_status(self):
         """Request pool state data."""
         _LOGGER.debug("Requesting pool status")
         if last_raw := await self._async_connected_request(
             async_request_pool_status, self._data, reconnect_delay=1
         ):
-            self._last["status"] = last_raw
+            self._last[DATA_REQUEST.STATUS] = last_raw
 
     async def async_get_pumps(self):
         """Request all pump state data."""
-        for pumpID in self._data[DATA.KEY_PUMPS]:
-            if self._data[DATA.KEY_PUMPS][pumpID]["data"] != 0:
+        for pumpID in self._data[DEVICE.PUMP]:
+            if self._data[DEVICE.PUMP][pumpID][VALUE.DATA] != 0:
                 _LOGGER.debug("Requesting pump %i data", pumpID)
-                last_pumps = self._last.setdefault(DATA.KEY_PUMPS, {})
+                last_pumps = self._last.setdefault(DATA_REQUEST.PUMPS, {})
                 if last_raw := await self._async_connected_request(
                     async_request_pump_status, self._data, pumpID, reconnect_delay=1
                 ):
                     last_pumps[pumpID] = last_raw
 
     async def async_get_chemistry(self):
         """Request IntelliChem controller data."""
         _LOGGER.debug("Requesting chemistry data")
         if last_raw := await self._async_connected_request(
             async_request_chemistry, self._data, reconnect_delay=1
         ):
-            self._last[DATA.KEY_CHEMISTRY] = last_raw
+            self._last[DATA_REQUEST.CHEMISTRY] = last_raw
 
     async def async_get_scg(self):
         """Request salt chlorine generator state data."""
         _LOGGER.debug("Requesting scg data")
         if last_raw := await self._async_connected_request(
             async_request_scg_config, self._data, reconnect_delay=1
         ):
-            self._last[DATA.KEY_SCG] = last_raw
+            self._last[DATA_REQUEST.SCG] = last_raw
+
+    # def get_data(self) -> dict:
+    #    """Return the data."""
+    #    return self._data
+
+    def get_data(self, *keypath, strict: bool = False):
+        """
+        Return a data value from a key path.
+
+        Returns the value of the key at the end of the keypath. Returns None if any key along the path is not found, or
+        raises a KeyError if 'strict' == True.
+        Returns the entire data dict if no 'keypath' is specified.
+        """
+
+        if not keypath:
+            return self._data
 
-    def get_data(self) -> dict:
-        """Return the data."""
-        return self._data
+        next = self._data
+
+        def get_next(key):
+            if current is None:
+                return None
+            if isinstance(current, dict):
+                return current.get(key)
+            if isinstance(current, list) and key in range(len(current)):
+                return current[key]
+            return None
+
+        for key in keypath:
+            current = next
+            next = get_next(key)
+            if next is None:
+                if strict:
+                    raise KeyError(f"'{key}' not found in '{keypath}'")
+                break
+        return next
+
+    def get_value(self, *keypath, strict: bool = False):
+        """
+        Returns the 'value' key of the dict at the end of the key path.
+
+        Shortcut to 'get_data(*keypath, "value")'.
+        """
+        data = self.get_data(*keypath, strict=strict)
+        if isinstance(data, dict) and (val := data.get(ATTR.VALUE)) is not None:
+            return val
+        else:
+            if strict:
+                raise KeyError(f"Value for {keypath} not found")
+            return None
+
+    def get_name(self, *keypath, strict: bool = False):
+        """
+        Returns the 'name' key of the dict at the end of the key path.
+
+        Shortcut to 'get_data(*keypath, "name")'.
+        """
+        data = self.get_data(*keypath, strict=strict)
+        if isinstance(data, dict) and (val := data.get(ATTR.NAME)) is not None:
+            return val
+        else:
+            if strict:
+                raise KeyError(f"Value for {keypath} not found")
+            return None
 
     def get_debug(self) -> dict:
         """Return the debug last-received data."""
         return self._last
 
-    def set_max_retries(self, max_retries: int = MESSAGE.COM_MAX_RETRIES) -> None:
+    def set_max_retries(self, max_retries: int = COM_MAX_RETRIES) -> None:
         if 0 < max_retries < 6:
             self._max_retries = max_retries
         else:
             raise ValueError(f"Invalid max_retries: {max_retries}")
 
     async def async_set_circuit(self, circuitID: int, circuitState: int):
         """Set the circuit state for the specified circuit."""
@@ -380,59 +455,48 @@
     def _common_connection_closed_callback(self):
         """Perform any needed cleanup."""
         if self._custom_connection_closed_callback:
             self._custom_connection_closed_callback()
 
     def _is_valid_circuit(self, circuit):
         """Validate circuit number."""
-        return circuit in self._data[DATA.KEY_CIRCUITS]
+        return circuit in self._data[DEVICE.CIRCUIT]
 
     def _is_valid_circuit_state(self, state):
         """Validate circuit state number."""
         return state == 0 or state == 1
 
     def _is_valid_body(self, body):
         """Validate body of water number."""
-        return body in self._data[DATA.KEY_BODIES]
+        return body in self._data[DEVICE.BODY]
 
     def _is_valid_heatmode(self, heatmode):
         """Validate heat mode number."""
         return 0 <= heatmode < 5
 
     def _is_valid_heattemp(self, body, temp):
         """Validate heat tem for body."""
-        min_temp = self._data[DATA.KEY_BODIES][int(body)]["min_set_point"]["value"]
-        max_temp = self._data[DATA.KEY_BODIES][int(body)]["max_set_point"]["value"]
+        min_temp = self.get_data(DEVICE.BODY, int(body), ATTR.MIN_SETPOINT)
+        max_temp = self.get_data(DEVICE.BODY, int(body), ATTR.MAX_SETPOINT)
         return min_temp <= temp <= max_temp
 
     def _is_valid_color_mode(self, mode):
         """Validate color mode number."""
         return 0 <= mode <= 21
 
     def _is_valid_scg_value(self, scg_value, body_type):
         """Validate chlorinator value for body."""
-        return 0 <= scg_value <= SCG.LIMIT_FOR_BODY[body_type]
+        return 0 <= scg_value <= LIMIT_FOR_BODY[body_type]
 
     def _is_valid_ph_setpoint(self, ph_setpoint: float):
         """Validate pH setpoint."""
         return (
-            CHEMISTRY.RANGE_PH_SETPOINT[RANGE.MIN]
-            <= ph_setpoint
-            <= CHEMISTRY.RANGE_PH_SETPOINT[RANGE.MAX]
+            RANGE_PH_SETPOINT[RANGE.MIN] <= ph_setpoint <= RANGE_PH_SETPOINT[RANGE.MAX]
         )
 
     def _is_valid_orp_setpoint(self, orp_setpoint: int):
         """Validate ORP setpoint."""
         return (
-            CHEMISTRY.RANGE_ORP_SETPOINT[RANGE.MIN]
+            RANGE_ORP_SETPOINT[RANGE.MIN]
             <= orp_setpoint
-            <= CHEMISTRY.RANGE_ORP_SETPOINT[RANGE.MAX]
+            <= RANGE_ORP_SETPOINT[RANGE.MAX]
         )
-
-    # Promote?
-    def _has_color_lights(self):
-        """Return if any configured lights support color modes."""
-        if circuits := self._data.get(DATA.KEY_CIRCUITS, None):
-            for circuit in circuits.values():
-                if circuit["function"] in CIRCUIT_FUNCTION.GROUP_LIGHTS_COLOR:
-                    return True
-        return False
```

### Comparing `screenlogicpy-0.8.2/screenlogicpy/requests/__init__.py` & `screenlogicpy-0.9.0/screenlogicpy/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `screenlogicpy-0.8.2/screenlogicpy/requests/client.py` & `screenlogicpy-0.9.0/screenlogicpy/requests/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import struct
 
-from ..const import CODE, CLIENT_ID, MESSAGE
+from ..const.common import CLIENT_ID
+from ..const.msg import CODE, COM_MAX_RETRIES
 from .protocol import ScreenLogicProtocol
 from .request import async_make_request
 
 
 async def async_request_add_client(
     protocol: ScreenLogicProtocol,
     clientID: int = CLIENT_ID,
-    max_retries: int = MESSAGE.COM_MAX_RETRIES,
+    max_retries: int = COM_MAX_RETRIES,
 ) -> bool:
     return (
         await async_make_request(
             protocol,
             CODE.ADD_CLIENT_QUERY,
             struct.pack("<II", 0, clientID),
             max_retries,
@@ -20,15 +21,15 @@
         == b""
     )
 
 
 async def async_request_remove_client(
     protocol: ScreenLogicProtocol,
     clientID: int = CLIENT_ID,
-    max_retries: int = MESSAGE.COM_MAX_RETRIES,
+    max_retries: int = COM_MAX_RETRIES,
 ) -> bool:
     return (
         await async_make_request(
             protocol,
             CODE.REMOVE_CLIENT_QUERY,
             struct.pack("<II", 0, clientID),
             max_retries,
```

### Comparing `screenlogicpy-0.8.2/screenlogicpy/requests/equipment.py` & `screenlogicpy-0.9.0/screenlogicpy/requests/equipment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import struct
 
-from ..const import CODE
+from ..const.msg import CODE
 from .protocol import ScreenLogicProtocol
 from .request import async_make_request
 from .utility import getSome, getArray
 
 
 async def async_request_equipment_config(
     protocol: ScreenLogicProtocol, data: dict, max_retries: int
```

### Comparing `screenlogicpy-0.8.2/screenlogicpy/requests/heat.py` & `screenlogicpy-0.9.0/screenlogicpy/requests/button.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,19 @@
 import struct
 
-from ..const import CODE
+from ..const.msg import CODE
 from .protocol import ScreenLogicProtocol
 from .request import async_make_request
 
 
-async def async_request_set_heat_setpoint(
-    protocol: ScreenLogicProtocol, body: int, set_point: float, max_retries: int
+async def async_request_pool_button_press(
+    protocol: ScreenLogicProtocol, circuit_id: int, circuit_state: int, max_retries: int
 ) -> bool:
     return (
         await async_make_request(
             protocol,
-            CODE.SETHEATTEMP_QUERY,
-            struct.pack("<III", 0, body, set_point),
-            max_retries,
-        )
-        == b""
-    )
-
-
-async def async_request_set_heat_mode(
-    protocol: ScreenLogicProtocol, body: int, heat_mode: int, max_retries: int
-) -> bool:
-    return (
-        await async_make_request(
-            protocol,
-            CODE.SETHEATMODE_QUERY,
-            struct.pack("<III", 0, body, heat_mode),
+            CODE.BUTTONPRESS_QUERY,
+            struct.pack("<III", 0, circuit_id, circuit_state),
             max_retries,
         )
         == b""
     )
```

### Comparing `screenlogicpy-0.8.2/screenlogicpy/requests/lights.py` & `screenlogicpy-0.9.0/screenlogicpy/requests/lights.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import struct
 
-from ..const import CODE, DATA
+from ..const.msg import CODE
+from ..const.data import ATTR, DEVICE, GROUP
 from .protocol import ScreenLogicProtocol
 from .request import async_make_request
 from .utility import getSome, getString
 
 
 async def async_request_pool_lights_command(
     protocol: ScreenLogicProtocol, light_command: int, max_retries: int
@@ -17,22 +18,18 @@
             max_retries,
         )
         == b""
     )
 
 
 def decode_color_update(buff: bytes, data: dict):
-    config = data.setdefault(DATA.KEY_CONFIG, {})
+    controller: dict = data.setdefault(DEVICE.CONTROLLER, {})
 
-    color_state = config.setdefault("color_state", {})
+    color_state: dict = controller.setdefault(GROUP.COLOR_LIGHTS, {})
 
-    mode, offset = getSome("I", buff, 0)  # 0
-    color_state["mode"] = mode
+    color_state[ATTR.COLOR_MODE], offset = getSome("I", buff, 0)  # 0
 
-    progress, offset = getSome("I", buff, offset)  # 4
-    color_state["progress"] = progress
+    color_state[ATTR.PROGRESS], offset = getSome("I", buff, offset)  # 4
 
-    limit, offset = getSome("I", buff, offset)  # 8
-    color_state["limit"] = limit
+    color_state[ATTR.LIMIT], offset = getSome("I", buff, offset)  # 8
 
-    text, offset = getString(buff, offset)  # 12
-    color_state["text"] = text
+    color_state[ATTR.TEXT], offset = getString(buff, offset)  # 12
```

### Comparing `screenlogicpy-0.8.2/screenlogicpy/requests/login.py` & `screenlogicpy-0.9.0/screenlogicpy/requests/login.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import asyncio
 import logging
 import struct
-from typing import Callable, Tuple
+from typing import Callable
 
-from ..const import CODE, MESSAGE, ScreenLogicError, ScreenLogicRequestError
+from ..const import ScreenLogicError, ScreenLogicRequestError
+from ..const.msg import CODE, COM_MAX_RETRIES, COM_TIMEOUT
 from .protocol import ScreenLogicProtocol
 from .request import async_make_request
 from .utility import asyncio_timeout, decodeMessageString, encodeMessageString
 
 _LOGGER = logging.getLogger(__name__)
 
 
@@ -33,33 +34,33 @@
     fmt = f"<II{len(clientVersion)}s{len(passwdPayload)}sI{len(mac)}sI"
     return struct.pack(
         fmt, schema, connectionType, clientVersion, passwdPayload, pid, mac, 0
     )
 
 
 async def async_get_mac_address(
-    gateway_ip: str, gateway_port: int, max_retries: int = MESSAGE.COM_MAX_RETRIES
+    gateway_ip: str, gateway_port: int, max_retries: int = COM_MAX_RETRIES
 ) -> str:
     """Connect to a screenlogic gateway and return the mac address only."""
     transport, protocol = await async_create_connection(gateway_ip, gateway_port)
     mac = await async_gateway_connect(transport, protocol, max_retries)
     if transport and not transport.is_closing():
         transport.close()
     return mac
 
 
 async def async_create_connection(
     gateway_ip: str, gateway_port: int, connection_lost_callback: Callable = None
-) -> Tuple[asyncio.Transport, ScreenLogicProtocol]:
+) -> tuple[asyncio.Transport, ScreenLogicProtocol]:
     try:
         loop = asyncio.get_running_loop()
 
         # on_con_lost = loop.create_future()
         _LOGGER.debug("Creating connection")
-        async with asyncio_timeout(MESSAGE.COM_TIMEOUT):
+        async with asyncio_timeout(COM_TIMEOUT):
             return await loop.create_connection(
                 lambda: ScreenLogicProtocol(loop, connection_lost_callback),
                 gateway_ip,
                 gateway_port,
             )
     except (OSError, asyncio.TimeoutError) as ex:
         raise ScreenLogicError(
@@ -109,15 +110,15 @@
         raise ScreenLogicError(f"Failed to logon to gateway: {re.msg}") from re
 
 
 async def async_connect_to_gateway(
     gateway_ip,
     gateway_port,
     connection_lost_callback: Callable = None,
-    max_retries: int = MESSAGE.COM_MAX_RETRIES,
-) -> Tuple[asyncio.Transport, ScreenLogicProtocol, str]:
+    max_retries: int = COM_MAX_RETRIES,
+) -> tuple[asyncio.Transport, ScreenLogicProtocol, str]:
     transport, protocol = await async_create_connection(
         gateway_ip, gateway_port, connection_lost_callback
     )
     mac_address = await async_gateway_connect(transport, protocol, max_retries)
     if await async_gateway_login(protocol, max_retries):
         return transport, protocol, mac_address
```

### Comparing `screenlogicpy-0.8.2/screenlogicpy/requests/protocol.py` & `screenlogicpy-0.9.0/screenlogicpy/requests/protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Defines an asyncio.Protocol for communicating with Pentair ScreenLogic systems."""
 import asyncio
 import itertools
 import logging
 import struct
 import time
-from typing import Awaitable, Callable, Tuple, List
+from typing import Awaitable, Callable
 
-from ..const import MESSAGE, ScreenLogicError
+from ..const import ScreenLogicError
+from ..const.msg import HEADER_LENGTH
 from .utility import makeMessage, takeMessage
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class ScreenLogicProtocol(asyncio.Protocol):
     """asyncio.Protocol for handling connection to a ScreenLogic protocol adapter."""
@@ -90,29 +91,29 @@
 
     def data_received(self, data: bytes) -> None:
         """Called with data is received."""
 
         if self._closing:
             return
 
-        def complete_messages(data: bytes) -> List[Tuple[int, int, bytes]]:
+        def complete_messages(data: bytes) -> list[tuple[int, int, bytes]]:
             """Return only complete ScreenLogic messages."""
 
             # Some pool configurations can require SL messages larger than can
             # come through in a single call to data_received(), so lets wait until
             # we have at least enough data to make a complete message before we
             # process and pass it on. Conversely, multiple SL messages may come in
             # a single call to data_received() so we collect all complete messages
             # before sending on.
 
             self._buff.extend(data)
             complete = []
-            while len(self._buff) >= MESSAGE.HEADER_LENGTH:
+            while len(self._buff) >= HEADER_LENGTH:
                 dataLen = struct.unpack_from("<I", self._buff, 4)[0]
-                totalLen = MESSAGE.HEADER_LENGTH + dataLen
+                totalLen = HEADER_LENGTH + dataLen
                 if len(self._buff) >= totalLen:
                     out = bytearray()
                     for _ in range(totalLen):
                         out.append(self._buff.pop(0))
                     complete.append(takeMessage(bytes(out)))
                 else:
                     break
@@ -249,15 +250,15 @@
             """Get response future for message ID."""
             fut: asyncio.Future
             if (fut := self._collection.pop(msgID, None)) is not None:
                 if not fut.cancelled():
                     return fut
             return None
 
-        def mark_done(self, message: Tuple[int, int, bytes]) -> bool:
+        def mark_done(self, message: tuple[int, int, bytes]) -> bool:
             """Mark future done and add response."""
             msgID, _, _ = message
             if (fut := self.try_get(msgID)) is not None:
                 try:
                     fut.set_result(message)
                 except asyncio.exceptions.InvalidStateError as ise:
                     raise ScreenLogicError(
```

### Comparing `screenlogicpy-0.8.2/screenlogicpy/requests/request.py` & `screenlogicpy-0.9.0/screenlogicpy/requests/request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import asyncio
 import logging
 
-from ..const import CODE, MESSAGE, ScreenLogicRequestError
+from ..const import ScreenLogicRequestError
+from ..const.msg import CODE, COM_MAX_RETRIES, COM_RETRY_WAIT, COM_TIMEOUT
 from .protocol import ScreenLogicProtocol
 from .utility import asyncio_timeout
 
 _LOGGER = logging.getLogger(__name__)
 
 
 async def async_make_request(
     protocol: ScreenLogicProtocol,
     requestCode: int,
     requestData: bytes = b"",
-    max_retries: int = MESSAGE.COM_MAX_RETRIES,
+    max_retries: int = COM_MAX_RETRIES,
 ) -> bytes:
     for attempt in range(0, max_retries + 1):
         request = protocol.await_send_message(requestCode, requestData)
         try:
-            async with asyncio_timeout(MESSAGE.COM_TIMEOUT):
+            async with asyncio_timeout(COM_TIMEOUT):
                 await request
         except asyncio.TimeoutError:
             error_message = (
                 f"Timeout waiting for response to message code '{requestCode}'"
             )
         except asyncio.CancelledError:
             _LOGGER.debug(f"Future for request '{requestCode}' was canceled!")
@@ -42,15 +43,15 @@
                 error_message = f"Unexpected response code '{responseCode}' for request code: {requestCode}, request: {requestData}"
 
         if attempt == max_retries:
             raise ScreenLogicRequestError(
                 f"{error_message} after {max_retries + 1} attempts"
             )
 
-        retry_delay = MESSAGE.COM_RETRY_WAIT * (attempt + 1)
+        retry_delay = COM_RETRY_WAIT * (attempt + 1)
 
         _LOGGER.debug(
             error_message + ". Will retry %i more time(s) in %i seconds",
             max_retries - attempt,
             retry_delay,
         )
```

### Comparing `screenlogicpy-0.8.2/screenlogicpy/requests/status.py` & `screenlogicpy-0.9.0/screenlogicpy/requests/config.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,205 +1,151 @@
 # import json
 import struct
 
-from ..const import (
-    CODE,
-    BODY_TYPE,
-    DATA,
-    DEVICE_TYPE,
-    ON_OFF,
-    STATE_TYPE,
-    UNIT,
-)
+from ..const.msg import CODE
+from ..const.data import ATTR, DEVICE, GROUP, VALUE, UNKNOWN
+from ..device_const.system import CONTROLLER, EQUIPMENT_FLAG, EQUIPMENT_MASK
 from .protocol import ScreenLogicProtocol
 from .request import async_make_request
-from .utility import getSome, getTemperatureUnit
+from .utility import getSome, getString
 
 
-async def async_request_pool_status(
+async def async_request_pool_config(
     protocol: ScreenLogicProtocol, data: dict, max_retries: int
 ) -> bytes:
     if result := await async_make_request(
-        protocol, CODE.POOLSTATUS_QUERY, struct.pack("<I", 0), max_retries
+        protocol,
+        CODE.CTRLCONFIG_QUERY,
+        struct.pack("<2I", 0, 0),  # 0,1 yields different return
+        max_retries,
     ):
-        decode_pool_status(result, data)
+        decode_pool_config(result, data)
         return result
 
 
-def decode_pool_status(buff: bytes, data: dict) -> None:
-    config = data.setdefault(DATA.KEY_CONFIG, {})
+def decode_pool_config(buff: bytes, data: dict) -> dict:
+    controller: dict = data.setdefault(DEVICE.CONTROLLER, {})
 
-    ok, offset = getSome("I", buff, 0)  # byte offset 0
-    config["ok"] = ok
+    controller[VALUE.CONTROLLER_ID], offset = getSome("I", buff, 0)
 
-    freezeMode, offset = getSome("B", buff, offset)  # byte offset 4
-    config["freeze_mode"] = {
-        "name": "Freeze Mode",
-        "value": ON_OFF.from_bool(freezeMode & 0x08),
-    }
-
-    remotes, offset = getSome("B", buff, offset)  # 5
-    config["remotes"] = {"name": "Remotes", "value": remotes}
+    controller_config: dict = controller.setdefault(GROUP.CONFIGURATION, {})
+    body_type_setpoint: dict = controller_config.setdefault(ATTR.BODY_TYPE, {})
 
-    poolDelay, offset = getSome("B", buff, offset)  # 6
-    config["pool_delay"] = {"name": "Pool Delay", "value": poolDelay}
+    for i in range(2):
+        body_type_setpoint_indexed: dict = body_type_setpoint.setdefault(i, {})
 
-    spaDelay, offset = getSome("B", buff, offset)  # 7
-    config["spa_delay"] = {"name": "Spa Delay", "value": spaDelay}
+        minSetPoint, offset = getSome("B", buff, offset)
+        body_type_setpoint_indexed[ATTR.MIN_SETPOINT] = minSetPoint
 
-    cleanerDelay, offset = getSome("B", buff, offset)  # 8
-    config["cleaner_delay"] = {"name": "Cleaner Delay", "value": cleanerDelay}
+        maxSetPoint, offset = getSome("B", buff, offset)
+        body_type_setpoint_indexed[ATTR.MAX_SETPOINT] = maxSetPoint
 
-    config[f"unknown_at_offset_{offset:02}"], offset = getSome("B", buff, offset)  # 9
-    config[f"unknown_at_offset_{offset:02}"], offset = getSome("B", buff, offset)  # 10
-    config[f"unknown_at_offset_{offset:02}"], offset = getSome("B", buff, offset)  # 11
+    degC, offset = getSome("B", buff, offset)
+    controller_config[VALUE.IS_CELSIUS] = {
+        ATTR.NAME: "Is Celsius",
+        ATTR.VALUE: degC,
+    }
 
-    sensors = data.setdefault(DATA.KEY_SENSORS, {})
+    c_type, offset = getSome("B", buff, offset)
+    controller_config[VALUE.CONTROLLER_TYPE] = c_type
 
-    temperature_unit = getTemperatureUnit(data)
+    h_type, offset = getSome("B", buff, offset)
+    controller_config[VALUE.HARDWARE_TYPE] = h_type
 
-    airTemp, offset = getSome("i", buff, offset)  # 12
-    sensors["air_temperature"] = {
-        "name": "Air Temperature",
-        "value": airTemp,
-        "unit": temperature_unit,
-        "device_type": DEVICE_TYPE.TEMPERATURE,
-        "state_type": STATE_TYPE.MEASUREMENT,
+    controller[VALUE.MODEL] = {
+        ATTR.NAME: "Model",
+        ATTR.VALUE: CONTROLLER.model_from_type(c_type, h_type),
     }
 
-    bodiesCount, offset = getSome("I", buff, offset)  # 16
+    controller_config[VALUE.CONTROLLER_DATA], offset = getSome("B", buff, offset)
 
-    # Should this default to 2?
-    bodiesCount = min(bodiesCount, 2)
+    controller_equipment: dict = controller.setdefault(GROUP.EQUIPMENT, {})
+    equipFlags, offset = getSome("I", buff, offset)
 
-    bodies: dict = data.setdefault(DATA.KEY_BODIES, {})
+    # Include only known flags.
+    controller_equipment[VALUE.FLAGS] = equipFlags & EQUIPMENT_MASK
 
-    for i in range(bodiesCount):
-        currentBody: dict = bodies.setdefault(i, {})
+    controller_equipment[VALUE.LIST] = [
+        # What's needed? Friendly name or FLAG name?
+        member.name  # .title
+        for member in EQUIPMENT_FLAG
+        if member in EQUIPMENT_FLAG(equipFlags)
+    ]
 
-        bodyType, offset = getSome("I", buff, offset)
-        if bodyType not in range(2):
-            bodyType = 0
+    controller_config[VALUE.DEFAULT_CIRCUIT_NAME], offset = getString(buff, offset)
 
-        currentBody.setdefault("min_set_point", {})["unit"] = temperature_unit
+    circuitCount, offset = getSome("I", buff, offset)
+    controller_config[VALUE.CIRCUIT_COUNT] = circuitCount
 
-        currentBody.setdefault("max_set_point", {})["unit"] = temperature_unit
+    circuit: dict = data.setdefault(DEVICE.CIRCUIT, {})
 
-        currentBody["body_type"] = {"name": "Type of body of water", "value": bodyType}
+    for i in range(circuitCount):
 
-        lastTemp, offset = getSome("i", buff, offset)
-        bodyName = "Last {} Temperature".format(BODY_TYPE.NAME_FOR_NUM[bodyType])
-        currentBody["last_temperature"] = {
-            "name": bodyName,
-            "value": lastTemp,
-            "unit": temperature_unit,
-            "device_type": DEVICE_TYPE.TEMPERATURE,
-            "state_type": STATE_TYPE.MEASUREMENT,
-        }
+        circuit_id, offset = getSome("i", buff, offset)
 
-        heatStatus, offset = getSome("i", buff, offset)
-        heaterName = "{} Heat".format(BODY_TYPE.NAME_FOR_NUM[bodyType])
-        currentBody["heat_status"] = {"name": heaterName, "value": heatStatus}
-
-        heatSetPoint, offset = getSome("i", buff, offset)
-        hspName = "{} Heat Set Point".format(BODY_TYPE.NAME_FOR_NUM[bodyType])
-        currentBody["heat_set_point"] = {
-            "name": hspName,
-            "value": heatSetPoint,
-            "unit": temperature_unit,
-            "device_type": DEVICE_TYPE.TEMPERATURE,
-        }
+        circuit_indexed: dict = circuit.setdefault(circuit_id, {})
 
-        coolSetPoint, offset = getSome("i", buff, offset)
-        cspName = "{} Cool Set Point".format(BODY_TYPE.NAME_FOR_NUM[bodyType])
-        currentBody["cool_set_point"] = {
-            "name": cspName,
-            "value": coolSetPoint,
-            "unit": temperature_unit,
-        }
+        circuit_indexed[ATTR.CIRCUIT_ID] = circuit_id
 
-        heatMode, offset = getSome("i", buff, offset)
-        hmName = "{} Heat Mode".format(BODY_TYPE.NAME_FOR_NUM[bodyType])
-        currentBody["heat_mode"] = {
-            "name": hmName,
-            "value": heatMode,
-        }
+        circuit_indexed[ATTR.NAME], offset = getString(buff, offset)
 
-    circuitCount, offset = getSome("I", buff, offset)
+        circuit_indexed_config: dict = circuit_indexed.setdefault(
+            GROUP.CONFIGURATION, {}
+        )
+        circuit_indexed_config[ATTR.NAME_INDEX], offset = getSome("B", buff, offset)
 
-    circuits: dict = data.setdefault(DATA.KEY_CIRCUITS, {})
+        func, offset = getSome("B", buff, offset)
+        circuit_indexed[ATTR.FUNCTION] = func  # CIRCUIT_FUNCTION(func)
 
-    for i in range(circuitCount):
-        circuitID, offset = getSome("I", buff, offset)
+        interface, offset = getSome("B", buff, offset)
+        circuit_indexed[ATTR.INTERFACE] = interface  # INTERFACE_GROUP(interface)
 
-        currentCircuit = circuits.setdefault(circuitID, {})
+        circuit_indexed_config[VALUE.FLAGS], offset = getSome("B", buff, offset)
 
-        if "id" not in currentCircuit:
-            currentCircuit["id"] = circuitID
+        color_set, offset = getSome("B", buff, offset)
+        color_position, offset = getSome("B", buff, offset)
+        color_stagger, offset = getSome("B", buff, offset)
+        circuit_indexed[GROUP.COLOR] = {
+            ATTR.COLOR_SET: color_set,
+            ATTR.COLOR_POSITION: color_position,
+            ATTR.COLOR_STAGGER: color_stagger,
+        }
 
-        circuitState, offset = getSome("I", buff, offset)
-        currentCircuit["value"] = circuitState
+        circuit_indexed[ATTR.DEVICE_ID], offset = getSome("B", buff, offset)
 
-        cColorSet, offset = getSome("B", buff, offset)
-        currentCircuit["color_set"] = cColorSet
+        circuit_indexed_config[ATTR.DEFAULT_RUNTIME], offset = getSome(
+            "H", buff, offset
+        )
 
-        cColorPos, offset = getSome("B", buff, offset)
-        currentCircuit["color_position"] = cColorPos
+        circuit_indexed_config[UNKNOWN(offset)], offset = getSome("B", buff, offset)
 
-        cColorStagger, offset = getSome("B", buff, offset)
-        currentCircuit["color_stagger"] = cColorStagger
+        circuit_indexed_config[UNKNOWN(offset)], offset = getSome("B", buff, offset)
 
-        circuitDelay, offset = getSome("B", buff, offset)
-        currentCircuit["delay"] = circuitDelay
+    colorCount, offset = getSome("I", buff, offset)
+    controller_config[VALUE.COLOR_COUNT] = colorCount
 
-    pH, offset = getSome("i", buff, offset)
-    sensors["ph"] = {
-        "name": "pH",
-        "value": (pH / 100),
-        "unit": UNIT.PH,
-        "state_type": STATE_TYPE.MEASUREMENT,
-    }
+    color: list = controller_config.setdefault(GROUP.COLOR, [])
 
-    orp, offset = getSome("i", buff, offset)
-    sensors["orp"] = {
-        "name": "ORP",
-        "value": orp,
-        "unit": UNIT.MILLIVOLT,
-        "state_type": STATE_TYPE.MEASUREMENT,
-    }
+    for i in range(colorCount):
+        colorName, offset = getString(buff, offset)
+        rgbR, offset = getSome("I", buff, offset)
+        rgbG, offset = getSome("I", buff, offset)
+        rgbB, offset = getSome("I", buff, offset)
+        color.append(
+            {
+                ATTR.NAME: colorName,
+                ATTR.VALUE: (rgbR, rgbG, rgbB),
+            }
+        )
 
-    saturation, offset = getSome("i", buff, offset)
-    sensors["saturation"] = {
-        "name": "Saturation Index",
-        "value": (saturation / 100),
-        "unit": UNIT.SATURATION_INDEX,
-        "state_type": STATE_TYPE.MEASUREMENT,
-    }
+    pump_count = 8
 
-    saltPPM, offset = getSome("i", buff, offset)
-    sensors["salt_ppm"] = {
-        "name": "Salt",
-        "value": (saltPPM * 50),
-        "unit": UNIT.PARTS_PER_MILLION,
-        "state_type": STATE_TYPE.MEASUREMENT,
-    }
+    pump: dict = data.setdefault(DEVICE.PUMP, {})
 
-    pHTank, offset = getSome("i", buff, offset)
-    sensors["ph_supply_level"] = {
-        "name": "pH Supply Level",
-        "value": pHTank,
-        "state_type": STATE_TYPE.MEASUREMENT,
-    }
+    for i in range(pump_count):
+        pump_indexed = pump.setdefault(i, {})
 
-    orpTank, offset = getSome("i", buff, offset)
-    sensors["orp_supply_level"] = {
-        "name": "ORP Supply Level",
-        "value": orpTank,
-        "state_type": STATE_TYPE.MEASUREMENT,
-    }
+        pump_indexed[VALUE.DATA], offset = getSome("B", buff, offset)
 
-    alarm, offset = getSome("i", buff, offset)
-    sensors["chem_alarm"] = {
-        "name": "Chemistry Alarm",
-        "value": alarm,
-        "device_type": DEVICE_TYPE.ALARM,
-    }
+    controller_config[VALUE.INTERFACE_TAB_FLAGS], offset = getSome("I", buff, offset)
+
+    controller_config[VALUE.SHOW_ALARMS], offset = getSome("I", buff, offset)
```

### Comparing `screenlogicpy-0.8.2/screenlogicpy/requests/utility.py` & `screenlogicpy-0.9.0/screenlogicpy/requests/utility.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 import struct
 import sys
-from typing import Any, List, Tuple
+from typing import Any
 
-from ..const import DATA, MESSAGE, UNIT, ScreenLogicError
+from ..const import ScreenLogicError
+from ..const.common import UNIT
+from ..const.msg import HEADER_FORMAT, HEADER_LENGTH
+from ..const.data import ATTR, DEVICE, GROUP, VALUE
 
 if sys.version_info[:2] < (3, 11):
     from async_timeout import timeout as asyncio_timeout  # noqa F401
 else:
     from asyncio import timeout as asyncio_timeout  # noqa F401
 
 
 def makeMessage(msgID: int, msgCode: int, messageData: bytes = b""):
     """Returns packed bytes formatted as a ready-to-send ScreenLogic message."""
     return struct.pack(
-        f"{MESSAGE.HEADER_FORMAT}{str(len(messageData))}s",
+        f"{HEADER_FORMAT}{str(len(messageData))}s",
         msgID,
         msgCode,
         len(messageData),
         messageData,
     )
 
 
-def takeMessage(data: bytes) -> Tuple[int, int, bytes]:
+def takeMessage(data: bytes) -> tuple[int, int, bytes]:
     """Return (messageID, messageCode, message) from raw ScreenLogic message bytes."""
-    messageBytes = len(data) - MESSAGE.HEADER_LENGTH
+    messageBytes = len(data) - HEADER_LENGTH
     msgID, msgCode, msgLen, msgData = struct.unpack(
-        f"{MESSAGE.HEADER_FORMAT}{messageBytes}s", data
+        f"{HEADER_FORMAT}{messageBytes}s", data
     )
     if msgLen != messageBytes:
         raise ScreenLogicError(
             f"Response length invalid. Claimed: {msgLen}. Received: {messageBytes}. Message ID: {msgID}. Message Code: {msgCode}. Data: {data}"
         )
     return msgID, msgCode, msgData  # return raw data
 
 
-def takeMessages(data: bytes) -> List[Tuple[int, int, bytes]]:
+def takeMessages(data: bytes) -> list[tuple[int, int, bytes]]:
     messages = []
     pos = 0
     try:
         while pos < len(data):
             msgID, pos = getSome("H", data, pos)
             msgCode, pos = getSome("H", data, pos)
             msgLength, pos = getSome("I", data, pos)
@@ -63,15 +66,15 @@
 def decodeMessageString(data) -> str:
     size = struct.unpack_from("<I", data, 0)[0]
     return struct.unpack_from(f"<{str(size)}s", data, struct.calcsize("<I"))[0].decode(
         "utf-8"
     )
 
 
-def getSome(format, buff, offset) -> Tuple[Any, int]:
+def getSome(format, buff, offset) -> tuple[Any, int]:
     fmt = format if format.startswith(">") else f"<{format}"
     newoffset = offset + struct.calcsize(fmt)
     return struct.unpack_from(fmt, buff, offset)[0], newoffset
 
 
 def getValueAt(buff, offset, want, **kwargs):
     fmt = want if want.startswith(">") else "<" + want
@@ -89,15 +92,15 @@
             data["device_type"] = device_type
     else:
         data = val
     newoffset = offset + struct.calcsize(fmt)
     return data, newoffset
 
 
-def getString(buff, offset) -> Tuple[str, int]:
+def getString(buff, offset) -> tuple[str, int]:
     fmtLen = "<I"
     offsetLen = offset + struct.calcsize(fmtLen)
     sLen = struct.unpack_from(fmtLen, buff, offset)[0]
     if sLen % 4 != 0:
         sLen += 4 - sLen % 4
 
     fmt = f"<{sLen}s"
@@ -117,12 +120,13 @@
         offset += offsetPad
     return items, offset
 
 
 def getTemperatureUnit(data: dict):
     return (
         UNIT.CELSIUS
-        if DATA.KEY_CONFIG in data
-        and "is_celsius" in data[DATA.KEY_CONFIG]
-        and data[DATA.KEY_CONFIG]["is_celsius"]["value"]
+        if data.get(DEVICE.CONTROLLER, {})
+        .get(GROUP.CONFIGURATION, {})
+        .get(VALUE.IS_CELSIUS, {})
+        .get(ATTR.VALUE)
         else UNIT.FAHRENHEIT
     )
```

### Comparing `screenlogicpy-0.8.2/screenlogicpy.egg-info/PKG-INFO` & `screenlogicpy-0.9.0/screenlogicpy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: screenlogicpy
-Version: 0.8.2
+Version: 0.9.0
 Summary: Interface for Pentair ScreenLogic connected pool controllers over IP via Python
 Home-page: https://github.com/dieselrabbit/screenlogicpy
 Author: Kevin Worrel
 Author-email: kevinworrel@yahoo.com
 License: GPLv3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # screenlogicpy
 
 ![PyPI](https://img.shields.io/pypi/v/screenlogicpy) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/screenlogicpy)
 
@@ -30,27 +29,28 @@
 ```shell
 $ pip install screenlogicpy
 ```
 
 # Library usage
 
 * _Changed in v0.5.0: The screenlogicpy library has moved over to using asyncio for all network I/O. Relevant methods now require the `async`/`await` syntax._
-* _**New in v0.8.0**: Support for Python 3.8 and 3.9 is being phased out across future releases. This will be the last version to support Python 3.8._
+* _New in v0.8.0: Support for Python 3.8 and 3.9 is being phased out across future releases. Version 0.8.x will be the last versions to support Python 3.8._
+* _**New in v0.9.0**: Support for Python 3.8 has been removed. Support for Python 3.9 is being phased out across future releases. Version 0.9.x will be the last versions to support Python 3.9._
 
 The `ScreenLogicGateway` class is the primary interface.
 
 ```python
 from screenlogicpy import ScreenLogicGateway
 
     gateway = ScreenLogicGateway()
 ```
 
 * _Changed in v0.5.0: Instantiating the gateway no longer automatically connects to the protocol adapter or performs an initial update._  
 * _Changed in v0.7.0: Passing adapter connection info when instantiating the gateway is deprecated and will be removed in a future release. Connection info should be passed to `async_connect()` instead._  
-* _**Changed in v0.8.0:** Support for passing connection info to gateway constructor is fully deprecated and has been removed. Ability to specify client id used for push subscriptions, and to specify maximum number of times to retry a request has replaced it._
+* _Changed in v0.8.0: Support for passing connection info to gateway constructor is fully deprecated and has been removed. Ability to specify client id used for push subscriptions, and to specify maximum number of times to retry a request has replaced it._
 
 ## Connecting to a ScreenLogic Protocol Adapter
 
 Once instantiated, use `async_connect()` to connect and login to the ScreenLogic protocol adapter, and gather the pool configuration.
 
 If disconnected, this method may be called without any parameters to reconnect with the previous connection info, or with new parameters to connect to a different host.
 
@@ -145,14 +145,60 @@
 
 The `ScreenLogicGateway` class caches all data from the ScreenLogic protocol adapter as a single `dict` object for continued reference by the consuming application. This includes any data processed via push or polling. The consuming application may get this data at anytime with the `get_data()` method.
 
 ```python
 data = gateway.get_data()
 ```
 
+`get_data()` now supports specifying a path directly to the data desired. A path can be any length. By default, if the data path is not found, `get_data()` will return `None`, similar to `dict.get()`. Alternatively `strict=True` keyword argument can be added to force the `ScreenLogicGateway` to raise a `KeyError` exception if the path is not found.
+
+The majority of data points normally available to the end-user via the official apps are presented as `dict` objects containing "name" and "value" keys/pairs. Additional keys may be present depending on the type of data.
+
+For example, let's consider the following scenario:
+
+```python
+gateway._data = {
+    "controller": {
+        "sensor": {
+            "air_temperature": {
+                "name": "Air Temperature",
+                "value": 57,
+                "unit": "Â°F",
+                "device_type": "temperature",
+                "state_type": "measurement",
+            },
+        }
+    }
+}
+data_path = ("controller", "sensor", "air_temperature")
+
+temperature_sensor = gateway.get_data(*data_path)
+```
+
+Here, `temperature_sensor` would be a `dict` of all key/value pairs under the "air_temperature" key.
+
+The `ScreenLogicGateway` also provides shortcut methods `get_name()` and `get_value()` to get the "name" or "value" values respectively from the specified data path.
+
+```python
+# sensor_value = 57
+sensor_value = gateway.get_value(*data_path)
+
+# sensor_name = "Air Temperature"
+sensor_name = gateway.get_name(*data_path)
+```
+
+To get other values directly, use `get_data()` with the full key path:
+
+```python
+# sensor_unit = "Â°F"
+sensor_unit = gateway.get_data("controller", "sensor", "air_temperature", "unit")
+```
+
+* _**New in v0.9.0**._
+
 ## Disconnecting
 
 When done, use `async_disconnect()` to unsubscribe from push updates and close the connection to the protocol adapter.
 
 ```python
 await gateway.async_disconnect()  
 ```
```

### Comparing `screenlogicpy-0.8.2/screenlogicpy.egg-info/SOURCES.txt` & `screenlogicpy-0.9.0/screenlogicpy.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -2,23 +2,34 @@
 README.md
 pyproject.toml
 setup.py
 screenlogicpy/__init__.py
 screenlogicpy/__main__.py
 screenlogicpy/cli.py
 screenlogicpy/client.py
-screenlogicpy/const.py
 screenlogicpy/discovery.py
 screenlogicpy/gateway.py
+screenlogicpy/path_dict.py
 screenlogicpy.egg-info/PKG-INFO
 screenlogicpy.egg-info/SOURCES.txt
 screenlogicpy.egg-info/dependency_links.txt
 screenlogicpy.egg-info/entry_points.txt
 screenlogicpy.egg-info/requires.txt
 screenlogicpy.egg-info/top_level.txt
+screenlogicpy/const/__init__.py
+screenlogicpy/const/common.py
+screenlogicpy/const/data.py
+screenlogicpy/const/msg.py
+screenlogicpy/device_const/__init__.py
+screenlogicpy/device_const/chemistry.py
+screenlogicpy/device_const/circuit.py
+screenlogicpy/device_const/heat.py
+screenlogicpy/device_const/pump.py
+screenlogicpy/device_const/scg.py
+screenlogicpy/device_const/system.py
 screenlogicpy/requests/__init__.py
 screenlogicpy/requests/button.py
 screenlogicpy/requests/chemistry.py
 screenlogicpy/requests/client.py
 screenlogicpy/requests/config.py
 screenlogicpy/requests/equipment.py
 screenlogicpy/requests/gateway.py
```

### Comparing `screenlogicpy-0.8.2/setup.py` & `screenlogicpy-0.9.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="screenlogicpy",
-    version="0.8.2",
+    version="0.9.0",
     author="Kevin Worrel",
     author_email="kevinworrel@yahoo.com",
     description="Interface for Pentair ScreenLogic connected pool controllers over IP via Python",
     license="GPLv3",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dieselrabbit/screenlogicpy",
     packages=setuptools.find_packages(include=["screenlogicpy", "screenlogicpy.*"]),
     classifiers=[
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
         "Development Status :: 3 - Alpha",
     ],
-    python_requires=">=3.8",
+    python_requires=">=3.9",
     install_requires=[
         "async_timeout>=3.0.0",
     ],
     entry_points={"console_scripts": ["screenlogicpy=screenlogicpy.__main__:main"]},
 )
```

### Comparing `screenlogicpy-0.8.2/tests/test_cli.py` & `screenlogicpy-0.9.0/tests/test_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import pytest
 from screenlogicpy.cli import cli
 from .const_data import (
     FAKE_GATEWAY_ADDRESS,
     FAKE_GATEWAY_NAME,
     FAKE_GATEWAY_PORT,
     FAKE_CONNECT_INFO,
+)
+from .expected_data import (
     EXPECTED_COMPLETE_DATA,
     EXPECTED_DASHBOARD,
     EXPECTED_VERBOSE_PREAMBLE,
 )
 
 
 async def run_cli_test(
@@ -166,18 +168,19 @@
 @pytest.mark.parametrize(
     "args, ret, expected",
     [
         ("set salt-generator 100 20", 0, "50 0"),
         (
             "-v set scg 20 0",
             0,
-            EXPECTED_VERBOSE_PREAMBLE + "Pool SCG Level: 50 Spa SCG Level: 0",
+            EXPECTED_VERBOSE_PREAMBLE
+            + "Pool Chlorinator Setpoint: 50 Spa Chlorinator Setpoint: 0",
         ),
-        ("set scg * *", 65, "No new SCG values. Nothing to do."),
-        ("set scg f *", 66, "Invalid SCG value"),
+        ("set scg * *", 65, "No new Chlorinator values. Nothing to do."),
+        ("set scg f *", 66, "Invalid Chlorinator value"),
     ],
 )
 async def test_set_scg(MockProtocolAdapter, capsys, args, ret, expected):
     await run_cli_test(MockProtocolAdapter, capsys, args, ret, expected)
 
 
 @pytest.mark.asyncio
```

### Comparing `screenlogicpy-0.8.2/tests/test_client.py` & `screenlogicpy-0.9.0/tests/test_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 import pytest
 import random
 import struct
 from unittest.mock import patch
 
 from screenlogicpy import ScreenLogicGateway
 from screenlogicpy.client import ClientManager
-from screenlogicpy.const import CODE
+from screenlogicpy.const.msg import CODE
 from .const_data import (
-    EXPECTED_CHEMISTRY_DATA,
-    EXPECTED_STATUS_DATA,
     FAKE_CHEMISTRY_RESPONSE,
     FAKE_CONNECT_INFO,
     FAKE_STATUS_RESPONSE,
 )
+from .expected_data import (
+    EXPECTED_CHEMISTRY_DATA,
+    EXPECTED_STATUS_DATA,
+)
 from .fake_gateway import expected_resp
 
 
 @pytest.mark.asyncio()
 async def test_sub_unsub(event_loop, MockProtocolAdapter):
     async with MockProtocolAdapter:
         clientID = random.randint(32767, 65535)
```

### Comparing `screenlogicpy-0.8.2/tests/test_decode.py` & `screenlogicpy-0.9.0/tests/test_decode.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from .const_data import (
-    EXPECTED_CONFIG_DATA,
-    EXPECTED_STATUS_DATA,
-    EXPECTED_PUMP_DATA,
-    EXPECTED_CHEMISTRY_DATA,
-    EXPECTED_SCG_DATA,
     FAKE_CONFIG_RESPONSE,
     FAKE_STATUS_RESPONSE,
     FAKE_PUMP_RESPONSE,
     FAKE_CHEMISTRY_RESPONSE,
     FAKE_SCG_RESPONSE,
 )
+from .expected_data import (
+    EXPECTED_CONFIG_DATA,
+    EXPECTED_STATUS_DATA,
+    EXPECTED_PUMP_DATA,
+    EXPECTED_CHEMISTRY_DATA,
+    EXPECTED_SCG_DATA,
+)
 from screenlogicpy.requests.config import decode_pool_config
 from screenlogicpy.requests.status import decode_pool_status
 from screenlogicpy.requests.pump import decode_pump_status
 from screenlogicpy.requests.chemistry import decode_chemistry
 from screenlogicpy.requests.scg import decode_scg_config
 from screenlogicpy.requests.utility import makeMessage, takeMessages
```

### Comparing `screenlogicpy-0.8.2/tests/test_discovery.py` & `screenlogicpy-0.9.0/tests/test_discovery.py`

 * *Files identical despite different names*

### Comparing `screenlogicpy-0.8.2/tests/test_gateway.py` & `screenlogicpy-0.9.0/tests/test_gateway.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,27 +3,28 @@
 import struct
 from unittest.mock import patch
 
 # from deepdiff import DeepDiff
 
 
 from tests.const_data import (
-    EXPECTED_COMPLETE_DATA,
     FAKE_CONNECT_INFO,
     FAKE_GATEWAY_ADDRESS,
     FAKE_GATEWAY_MAC,
     FAKE_GATEWAY_NAME,
     FAKE_GATEWAY_PORT,
     FAKE_GATEWAY_VERSION,
     FAKE_STATUS_RESPONSE,
 )
+from tests.expected_data import EXPECTED_COMPLETE_DATA
 from tests.fake_gateway import error_resp, expected_resp
 
 from screenlogicpy import ScreenLogicGateway
-from screenlogicpy.const import CODE, MESSAGE, ScreenLogicRequestError
+from screenlogicpy.const.common import ScreenLogicRequestError
+from screenlogicpy.const.msg import CODE
 
 
 @pytest.mark.asyncio
 async def test_gateway(MockConnectedGateway):
     gateway = MockConnectedGateway
     assert gateway.ip == FAKE_GATEWAY_ADDRESS
     assert gateway.port == FAKE_GATEWAY_PORT
@@ -56,14 +57,133 @@
         assert gateway.name == FAKE_GATEWAY_NAME
         assert gateway.version == FAKE_GATEWAY_VERSION
         assert gateway.mac == FAKE_GATEWAY_MAC
         assert gateway.is_connected
         await gateway.async_disconnect()
 
 
+@pytest.mark.parametrize(
+    "path, expected",
+    [
+        (
+            ("controller", "sensor", "air_temperature"),
+            {
+                "name": "Air Temperature",
+                "value": 57,
+                "unit": "°F",
+                "device_type": "temperature",
+                "state_type": "measurement",
+            },
+        ),
+        (
+            ("controller", "equipment"),
+            {
+                "flags": 98360,
+                "list": [
+                    "INTELLIBRITE",
+                    "INTELLIFLO_0",
+                    "INTELLIFLO_1",
+                    "INTELLICHEM",
+                    "HYBRID_HEATER",
+                ],
+            },
+        ),
+        (
+            ("adapter",),
+            {"firmware": {"name": "Protocol Adapter Firmware", "value": "fake 0.0.3"}},
+        ),
+        (
+            ("intellichem", "alarm", "does_not_exist"),
+            None,
+        ),
+        (
+            ("controller", "configuration", "color", 20),
+            None,
+        ),
+    ],
+)
+def test_get_data(MockConnectedGateway: ScreenLogicGateway, path, expected):
+    assert MockConnectedGateway.get_data(*path) == expected
+
+
+@pytest.mark.parametrize(
+    "path, expected",
+    [
+        (
+            ("controller", "configuration", "color", 2),
+            (0, 255, 80),
+        ),
+        (
+            ("controller", "sensor", "air_temperature"),
+            57,
+        ),
+        (
+            ("circuit", 502),
+            1,
+        ),
+        (
+            ("intellichem", "alarm", "does_not_exist"),
+            None,
+        ),
+        (
+            ("controller", "configuration", "color", 20),
+            None,
+        ),
+    ],
+)
+def test_get_value(MockConnectedGateway: ScreenLogicGateway, path, expected):
+    assert MockConnectedGateway.get_value(*path) == expected
+
+
+@pytest.mark.parametrize(
+    "path, expected",
+    [
+        (
+            ("controller", "configuration", "color", 2),
+            "Green",
+        ),
+        (
+            ("controller", "sensor", "air_temperature"),
+            "Air Temperature",
+        ),
+        (
+            ("circuit", 502),
+            "Pool Light",
+        ),
+        (
+            ("intellichem", "alarm", "does_not_exist"),
+            None,
+        ),
+        (
+            ("controller", "configuration", "color", 20),
+            None,
+        ),
+    ],
+)
+def test_get_name(MockConnectedGateway: ScreenLogicGateway, path, expected):
+    assert MockConnectedGateway.get_name(*path) == expected
+
+
+def test_get_strict(MockConnectedGateway: ScreenLogicGateway):
+    with pytest.raises(KeyError):
+        MockConnectedGateway.get_data(
+            "intellichem", "alarm", "does_not_exist", strict=True
+        )
+
+    with pytest.raises(KeyError):
+        MockConnectedGateway.get_value(
+            "controller", "configuration", "body_type", 0, strict=True
+        )
+
+    with pytest.raises(KeyError):
+        MockConnectedGateway.get_name(
+            "controller", "configuration", "color", 20, strict=True
+        )
+
+
 @pytest.mark.asyncio
 async def test_async_set_circuit(
     event_loop: asyncio.AbstractEventLoop, MockConnectedGateway
 ):
     circuit_id = 505
     circuit_state = 1
     button_code = 12530
@@ -101,15 +221,15 @@
 
     with patch(
         "screenlogicpy.requests.button.ScreenLogicProtocol.await_send_message",
         side_effect=(
             req_fut(error_resp(button_code)),
             req_fut(expected_resp(button_code)),
         ),
-    ) as mockRequest, patch.object(MESSAGE, "COM_RETRY_WAIT", 1):
+    ) as mockRequest, patch("screenlogicpy.const.msg.COM_RETRY_WAIT", 1):
         gateway = MockConnectedGateway
         assert await gateway.async_set_circuit(circuit_id, circuit_state)
         await gateway.async_disconnect()
         assert mockRequest.call_count == 2
         assert mockRequest.call_args.args[0] == button_code
         assert mockRequest.call_args.args[1] == struct.pack(
             "<III", 0, circuit_id, circuit_state
@@ -139,16 +259,16 @@
         "screenlogicpy.requests.button.ScreenLogicProtocol.await_send_message",
         side_effect=(
             event_loop.create_future(),
             event_loop.create_future(),
         ),
     ) as mockRequest, patch.object(
         ScreenLogicGateway, "_async_connected_request", patched_request
-    ), patch.object(
-        MESSAGE, "COM_RETRY_WAIT", 1
+    ), patch(
+        "screenlogicpy.const.msg.COM_RETRY_WAIT", 1
     ):
         gateway: ScreenLogicGateway = MockConnectedGateway
         with pytest.raises(ScreenLogicRequestError) as e_info:
             await gateway.async_set_circuit(circuit_id, circuit_state)
         await gateway.async_disconnect()
         assert "Timeout" in e_info.value.msg
         assert mockRequest.call_count == 2
@@ -248,15 +368,15 @@
     event_loop: asyncio.AbstractEventLoop, MockConnectedGateway: ScreenLogicGateway
 ):
     result = event_loop.create_future()
     result.set_result(expected_resp(CODE.POOLSTATUS_QUERY, FAKE_STATUS_RESPONSE))
     with patch(
         "screenlogicpy.requests.gateway.ScreenLogicProtocol.await_send_message",
         side_effect=(event_loop.create_future(), event_loop.create_future(), result),
-    ) as mockRequest, patch.object(MESSAGE, "COM_RETRY_WAIT", 1):
+    ) as mockRequest, patch("screenlogicpy.const.msg.COM_RETRY_WAIT", 1):
         gateway = MockConnectedGateway
         gateway.set_max_retries(3)
         response = await gateway.async_send_message(
             CODE.POOLSTATUS_QUERY, struct.pack("<I", 0)
         )
         assert response == FAKE_STATUS_RESPONSE
         assert mockRequest.call_count == 3
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `screenlogicpy-0.8.2/tests/test_login.py` & `screenlogicpy-0.9.0/tests/test_login.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import asyncio
 import pytest
 from unittest.mock import patch
 
-from screenlogicpy.const import CODE, MESSAGE, ScreenLogicError
+from screenlogicpy.const.common import ScreenLogicError
+from screenlogicpy.const.msg import CODE
 from screenlogicpy.gateway import ScreenLogicGateway
 from screenlogicpy.requests.login import async_connect_to_gateway, async_get_mac_address
 from screenlogicpy.requests.utility import encodeMessageString
 from tests.const_data import (
     FAKE_CONNECT_INFO,
     FAKE_GATEWAY_ADDRESS,
     FAKE_GATEWAY_MAC,
@@ -58,15 +59,15 @@
                     expected_resp(
                         CODE.CHALLENGE_QUERY, encodeMessageString(FAKE_GATEWAY_MAC)
                     )
                 ),
                 req_fut(),
                 req_fut(),
             ),
-        ) as mockRequest, patch.object(MESSAGE, "COM_RETRY_WAIT", 1):
+        ) as mockRequest, patch("screenlogicpy.const.msg.COM_RETRY_WAIT", 1):
             gateway = ScreenLogicGateway()
             with pytest.raises(ScreenLogicError) as e_info:
                 await gateway.async_connect(**FAKE_CONNECT_INFO)
             assert "Timeout" in e_info.value.msg
             assert mockRequest.call_count == 3
 
 
@@ -90,13 +91,13 @@
                     expected_resp(
                         CODE.CHALLENGE_QUERY, encodeMessageString(FAKE_GATEWAY_MAC)
                     )
                 ),
                 req_fut(error_resp(CODE.LOCALLOGIN_QUERY)),
                 req_fut(error_resp(CODE.LOCALLOGIN_QUERY)),
             ),
-        ) as mockRequest, patch.object(MESSAGE, "COM_RETRY_WAIT", 1):
+        ) as mockRequest, patch("screenlogicpy.const.msg.COM_RETRY_WAIT", 1):
             gateway = ScreenLogicGateway()
             with pytest.raises(ScreenLogicError) as e_info:
                 await gateway.async_connect(**FAKE_CONNECT_INFO)
             assert "Rejected" in e_info.value.msg
             assert mockRequest.call_count == 3
```

### Comparing `screenlogicpy-0.8.2/tests/test_protocol.py` & `screenlogicpy-0.9.0/tests/test_protocol.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import asyncio
 import pytest
 
 from .const_data import FAKE_CONFIG_RESPONSE_LARGE
-from screenlogicpy.const import CODE as MSG_CODE, MESSAGE as CONST_MESSAGE
+from screenlogicpy.const.msg import CODE as MSG_CODE, HEADER_LENGTH
 from screenlogicpy.requests.protocol import ScreenLogicProtocol
 from screenlogicpy.requests.utility import makeMessage
 
 
 @pytest.mark.asyncio
 async def test_async_data_received(event_loop):
     CODE = 1196
@@ -31,15 +31,15 @@
 
     assert data.get("result") == MESSAGE
 
 
 @pytest.mark.asyncio
 async def test_async_large_data_received(event_loop):
     CODE = MSG_CODE.CTRLCONFIG_QUERY + 1
-    MESSAGE = FAKE_CONFIG_RESPONSE_LARGE[CONST_MESSAGE.HEADER_LENGTH :]
+    MESSAGE = FAKE_CONFIG_RESPONSE_LARGE[HEADER_LENGTH:]
 
     data = {}
 
     callback_triggered: asyncio.Future
     callback_triggered = event_loop.create_future()
 
     async def callback(message, target_data):
```

