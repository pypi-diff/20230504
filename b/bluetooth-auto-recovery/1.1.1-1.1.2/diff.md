# Comparing `tmp/bluetooth_auto_recovery-1.1.1.tar.gz` & `tmp/bluetooth_auto_recovery-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluetooth_auto_recovery-1.1.1.tar", max compression
+gzip compressed data, was "bluetooth_auto_recovery-1.1.2.tar", max compression
```

## Comparing `bluetooth_auto_recovery-1.1.1.tar` & `bluetooth_auto_recovery-1.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1072 2023-05-03 15:15:19.780969 bluetooth_auto_recovery-1.1.1/LICENSE
--rw-r--r--   0        0        0     3840 2023-05-03 15:15:19.780969 bluetooth_auto_recovery-1.1.1/README.md
--rw-r--r--   0        0        0     2490 2023-05-03 15:15:20.632976 bluetooth_auto_recovery-1.1.1/pyproject.toml
--rw-r--r--   0        0        0       91 2023-05-03 15:15:20.592976 bluetooth_auto_recovery-1.1.1/src/bluetooth_auto_recovery/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 15:15:19.784969 bluetooth_auto_recovery-1.1.1/src/bluetooth_auto_recovery/py.typed
--rw-r--r--   0        0        0    20857 2023-05-03 15:15:19.784969 bluetooth_auto_recovery-1.1.1/src/bluetooth_auto_recovery/recover.py
--rw-r--r--   0        0        0     5366 1970-01-01 00:00:00.000000 bluetooth_auto_recovery-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-04 12:36:05.129024 bluetooth_auto_recovery-1.1.2/LICENSE
+-rw-r--r--   0        0        0     3840 2023-05-04 12:36:05.129024 bluetooth_auto_recovery-1.1.2/README.md
+-rw-r--r--   0        0        0     2490 2023-05-04 12:36:06.029043 bluetooth_auto_recovery-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0       91 2023-05-04 12:36:05.973041 bluetooth_auto_recovery-1.1.2/src/bluetooth_auto_recovery/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 12:36:05.129024 bluetooth_auto_recovery-1.1.2/src/bluetooth_auto_recovery/py.typed
+-rw-r--r--   0        0        0    22119 2023-05-04 12:36:05.133024 bluetooth_auto_recovery-1.1.2/src/bluetooth_auto_recovery/recover.py
+-rw-r--r--   0        0        0     5366 1970-01-01 00:00:00.000000 bluetooth_auto_recovery-1.1.2/PKG-INFO
```

### Comparing `bluetooth_auto_recovery-1.1.1/LICENSE` & `bluetooth_auto_recovery-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bluetooth_auto_recovery-1.1.1/README.md` & `bluetooth_auto_recovery-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `bluetooth_auto_recovery-1.1.1/pyproject.toml` & `bluetooth_auto_recovery-1.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bluetooth-auto-recovery"
-version = "1.1.1"
+version = "1.1.2"
 description = "Recover bluetooth adapters that are in an stuck state"
 authors = ["J. Nick Koston <nick@koston.org>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bluetooth-devices/bluetooth-auto-recovery"
 documentation = "https://bluetooth-auto-recovery.readthedocs.io"
 classifiers = [
```

### Comparing `bluetooth_auto_recovery-1.1.1/src/bluetooth_auto_recovery/recover.py` & `bluetooth_auto_recovery-1.1.2/src/bluetooth_auto_recovery/recover.py`

 * *Files 4% similar despite different names*

```diff
@@ -447,15 +447,19 @@
             ex,
         )
         return False
     except OSError as ex:
         _LOGGER.warning("Bluetooth adapter %s could not be reset: %s", name, ex)
         return False
     except asyncio.TimeoutError:
-        _LOGGER.warning("Bluetooth adapter %s could not be reset due to timeout", name)
+        _LOGGER.warning(
+            "Bluetooth adapter %s could not be reset due to timeout after %s seconds",
+            name,
+            adapter.timeout,
+        )
         return False
 
 
 async def _usb_reset_adapter(hci: int) -> bool:
     """Reset the bluetooth adapter."""
     _LOGGER.debug("Executing USB reset for Bluetooth adapter hci%i", hci)
     dev = BluetoothDevice(hci)
@@ -513,62 +517,67 @@
             "%s seems not to exist (anymore), check BT interface mac address in your settings; "
             "Available adapters: %s ",
             name,
             adapter.presented_list,
         )
         return False
 
+    timed_out_getting_powered: bool = False
+    power_state_before_reset: bool | None = None
     try:
-        pstate_before = await adapter.get_powered()
+        power_state_before_reset = await adapter.get_powered()
     except AttributeError as ex:
         _LOGGER.warning(
             "Could not determine the power state of the Bluetooth adapter %s: %s",
             name,
             ex,
         )
-
-    if pstate_before is True:
-        _LOGGER.debug("Current power state of bluetooth adapter is ON.")
-        try:
-            await adapter.set_powered(False)
-        except AttributeError as ex:
-            _LOGGER.warning(
-                "Could not power cycle the Bluetooth adapter %s: %s", name, ex
-            )
-            return False
-        await adapter.wait_for_power_state(False, POWER_OFF_TIME)
-    elif pstate_before is False:
-        _LOGGER.debug(
-            "Current power state of bluetooth adapter %s is OFF, trying to turn it back ON",
+    except asyncio.TimeoutError:
+        _LOGGER.warning(
+            "Could not determine the power state of the Bluetooth adapter %s due to timeout after %s seconds",
             name,
+            adapter.timeout,
         )
-    else:
-        _LOGGER.debug("Power state of bluetooth adapter could not be determined")
+        timed_out_getting_powered = True
+
+    # Do not attempt to power off if it timed out getting the power state
+    # as it likely means the adapter interface is frozen and will not respond to
+    # power off commands so we need to proceed to bounce the interface
+    if not timed_out_getting_powered and not await _execute_power_off(
+        adapter, name, power_state_before_reset
+    ):
         return False
 
     try:
         await _bounce_adapter_interface(adapter)
     except Exception as ex:  # pylint: disable=broad-except
         _LOGGER.warning("Could not cycle the Bluetooth adapter %s: %s", name, ex)
 
+    return await _execute_power_on(adapter, name, power_state_before_reset)
+
+
+async def _execute_power_on(
+    adapter: MGMTBluetoothCtl, name: str, power_state_before_reset: bool | None
+) -> bool:
+    """Execute the power off."""
     try:
         await adapter.set_powered(True)
     except AttributeError as ex:
         _LOGGER.warning(
             "Could not re-enable power after cycle of the Bluetooth adapter %s: %s",
             name,
             ex,
         )
         return False
 
     pstate_after = await adapter.wait_for_power_state(True, POWER_ON_TIME)
 
     # Check the state after the reset
     if pstate_after is True:
-        if pstate_before is False:
+        if power_state_before_reset is False:
             _LOGGER.warning("Bluetooth adapter %s successfully turned back ON", name)
         else:
             _LOGGER.debug(
                 "Power state of bluetooth adapter %s is ON after power cycle", name
             )
         return True
 
@@ -581,14 +590,40 @@
     _LOGGER.debug(
         "Power state of bluetooth adapter %s could not be determined after power cycle",
         name,
     )
     return False
 
 
+async def _execute_power_off(
+    adapter: MGMTBluetoothCtl, name: str, power_state_before_reset: bool | None
+) -> bool:
+    """Execute the power off."""
+    if power_state_before_reset is True:
+        _LOGGER.debug("Current power state of bluetooth adapter is ON.")
+        try:
+            await adapter.set_powered(False)
+        except AttributeError as ex:
+            _LOGGER.warning(
+                "Could not power cycle the Bluetooth adapter %s: %s", name, ex
+            )
+            return False
+        await adapter.wait_for_power_state(False, POWER_OFF_TIME)
+    elif power_state_before_reset is False:
+        _LOGGER.debug(
+            "Current power state of bluetooth adapter %s is OFF, trying to turn it back ON",
+            name,
+        )
+    else:
+        _LOGGER.debug("Power state of bluetooth adapter could not be determined")
+        return False
+
+    return True
+
+
 def raw_open(adapter_idx: int) -> socket.socket:
     """Create a bluetooth socket for a specific adapter."""
     sock = socket.socket(AF_BLUETOOTH, socket.SOCK_RAW, BTPROTO_HCI)
     sock.bind((adapter_idx,))
     return sock
```

### Comparing `bluetooth_auto_recovery-1.1.1/PKG-INFO` & `bluetooth_auto_recovery-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluetooth-auto-recovery
-Version: 1.1.1
+Version: 1.1.2
 Summary: Recover bluetooth adapters that are in an stuck state
 Home-page: https://github.com/bluetooth-devices/bluetooth-auto-recovery
 License: MIT
 Author: J. Nick Koston
 Author-email: nick@koston.org
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bluetooth-auto-recovery Version: 1.1.1 Summary:
+Metadata-Version: 2.1 Name: bluetooth-auto-recovery Version: 1.1.2 Summary:
 Recover bluetooth adapters that are in an stuck state Home-page: https://
 github.com/bluetooth-devices/bluetooth-auto-recovery License: MIT Author: J.
 Nick Koston Author-email: nick@koston.org Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
 :: Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

