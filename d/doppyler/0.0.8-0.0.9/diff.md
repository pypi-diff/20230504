# Comparing `tmp/doppyler-0.0.8.tar.gz` & `tmp/doppyler-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doppyler-0.0.8.tar", last modified: Thu Oct  6 00:12:41 2022, max compression
+gzip compressed data, was "doppyler-0.0.9.tar", last modified: Thu Oct  6 01:38:27 2022, max compression
```

## Comparing `doppyler-0.0.8.tar` & `doppyler-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 00:12:41.620387 doppyler-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)      680 2022-10-06 00:12:41.620387 doppyler-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-10-06 00:12:39.000000 doppyler-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 00:12:41.616387 doppyler-0.0.8/doppyler/
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-10-06 00:12:39.000000 doppyler-0.0.8/doppyler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9601 2022-10-06 00:12:39.000000 doppyler-0.0.8/doppyler/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     2579 2022-10-06 00:12:39.000000 doppyler-0.0.8/doppyler/const.py
--rw-r--r--   0 runner    (1001) docker     (121)     1188 2022-10-06 00:12:39.000000 doppyler-0.0.8/doppyler/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 00:12:41.620387 doppyler-0.0.8/doppyler/model/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-10-06 00:12:39.000000 doppyler-0.0.8/doppyler/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2627 2022-10-06 00:12:39.000000 doppyler-0.0.8/doppyler/model/alarm.py
--rw-r--r--   0 runner    (1001) docker     (121)     1414 2022-10-06 00:12:39.000000 doppyler-0.0.8/doppyler/model/color.py
--rw-r--r--   0 runner    (1001) docker     (121)    32420 2022-10-06 00:12:39.000000 doppyler-0.0.8/doppyler/model/doppler.py
--rw-r--r--   0 runner    (1001) docker     (121)     5149 2022-10-06 00:12:39.000000 doppyler-0.0.8/doppyler/model/light_bar.py
--rw-r--r--   0 runner    (1001) docker     (121)     1224 2022-10-06 00:12:39.000000 doppyler-0.0.8/doppyler/model/main_display_text.py
--rw-r--r--   0 runner    (1001) docker     (121)     1122 2022-10-06 00:12:39.000000 doppyler-0.0.8/doppyler/model/mini_display_number.py
--rw-r--r--   0 runner    (1001) docker     (121)     1246 2022-10-06 00:12:39.000000 doppyler-0.0.8/doppyler/model/smart_button.py
--rw-r--r--   0 runner    (1001) docker     (121)      268 2022-10-06 00:12:39.000000 doppyler-0.0.8/doppyler/model/sound.py
--rw-r--r--   0 runner    (1001) docker     (121)     1874 2022-10-06 00:12:39.000000 doppyler-0.0.8/doppyler/model/weather.py
--rw-r--r--   0 runner    (1001) docker     (121)      949 2022-10-06 00:12:39.000000 doppyler-0.0.8/doppyler/model/wifi.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 00:12:41.620387 doppyler-0.0.8/doppyler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      680 2022-10-06 00:12:41.000000 doppyler-0.0.8/doppyler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      606 2022-10-06 00:12:41.000000 doppyler-0.0.8/doppyler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-06 00:12:41.000000 doppyler-0.0.8/doppyler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-06 00:12:41.000000 doppyler-0.0.8/doppyler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-10-06 00:12:41.000000 doppyler-0.0.8/doppyler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-10-06 00:12:41.000000 doppyler-0.0.8/doppyler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      380 2022-10-06 00:12:41.620387 doppyler-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1042 2022-10-06 00:12:39.000000 doppyler-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 01:38:27.239815 doppyler-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      680 2022-10-06 01:38:27.239815 doppyler-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      363 2022-10-06 01:38:24.000000 doppyler-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 01:38:27.235814 doppyler-0.0.9/doppyler/
+-rw-r--r--   0 runner    (1001) docker     (121)      153 2022-10-06 01:38:24.000000 doppyler-0.0.9/doppyler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9715 2022-10-06 01:38:24.000000 doppyler-0.0.9/doppyler/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2579 2022-10-06 01:38:24.000000 doppyler-0.0.9/doppyler/const.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1188 2022-10-06 01:38:24.000000 doppyler-0.0.9/doppyler/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 01:38:27.239815 doppyler-0.0.9/doppyler/model/
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-10-06 01:38:24.000000 doppyler-0.0.9/doppyler/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2627 2022-10-06 01:38:24.000000 doppyler-0.0.9/doppyler/model/alarm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1414 2022-10-06 01:38:24.000000 doppyler-0.0.9/doppyler/model/color.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32594 2022-10-06 01:38:24.000000 doppyler-0.0.9/doppyler/model/doppler.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5149 2022-10-06 01:38:24.000000 doppyler-0.0.9/doppyler/model/light_bar.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1224 2022-10-06 01:38:24.000000 doppyler-0.0.9/doppyler/model/main_display_text.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1122 2022-10-06 01:38:24.000000 doppyler-0.0.9/doppyler/model/mini_display_number.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-10-06 01:38:24.000000 doppyler-0.0.9/doppyler/model/smart_button.py
+-rw-r--r--   0 runner    (1001) docker     (121)      268 2022-10-06 01:38:24.000000 doppyler-0.0.9/doppyler/model/sound.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1874 2022-10-06 01:38:24.000000 doppyler-0.0.9/doppyler/model/weather.py
+-rw-r--r--   0 runner    (1001) docker     (121)      949 2022-10-06 01:38:24.000000 doppyler-0.0.9/doppyler/model/wifi.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 01:38:27.239815 doppyler-0.0.9/doppyler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      680 2022-10-06 01:38:27.000000 doppyler-0.0.9/doppyler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      606 2022-10-06 01:38:27.000000 doppyler-0.0.9/doppyler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-06 01:38:27.000000 doppyler-0.0.9/doppyler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-06 01:38:27.000000 doppyler-0.0.9/doppyler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-10-06 01:38:27.000000 doppyler-0.0.9/doppyler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-10-06 01:38:27.000000 doppyler-0.0.9/doppyler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      380 2022-10-06 01:38:27.239815 doppyler-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1042 2022-10-06 01:38:24.000000 doppyler-0.0.9/setup.py
```

### Comparing `doppyler-0.0.8/PKG-INFO` & `doppyler-0.0.9/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doppyler
-Version: 0.0.8
+Version: 0.0.9
 Summary: A library to interact with the Sandman Doppler Clock API
 Home-page: https://github.com/pa-innovation/doppyler
 Author: Sandman Doppler
 Author-email: hi@paloaltoinnovation.com
 License: UNKNOWN
 Keywords: doppyler
 Platform: UNKNOWN
```

### Comparing `doppyler-0.0.8/doppyler/client.py` & `doppyler-0.0.9/doppyler/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -129,26 +129,26 @@
             try:
                 resp_data = await resp.json(content_type=None)
             except JSONDecodeError:
                 resp_data = await resp.text()
 
             if resp.status in (200, 201):
                 if isinstance(resp_data, str):
-                    raise InvalidDataReturned(resp_data)
+                    raise InvalidDataReturned(resp_data, method, url, data)
                 return resp_data
 
             if resp.status == 400:
-                raise BadRequestException(resp_data)
+                raise BadRequestException(resp_data, method, url, data)
             if resp.status in (401, 403):
-                raise UnauthorizedException(resp_data)
+                raise UnauthorizedException(resp_data, method, url, data)
             if resp.status == 410:
-                raise ExpiredNonce(resp_data)
+                raise ExpiredNonce(resp_data, method, url, data)
             if resp.status == 408:
-                raise CantConnectException(resp_data)
-            raise UnknownException(resp_data)
+                raise CantConnectException(resp_data, method, url, data)
+            raise UnknownException(resp_data, method, url, data)
 
     async def get_token(self) -> None:
         """Get token."""
         self._token_event.clear()
         auth_payload = {
             "authenticationDetails": {
                 "applicationId": self.application_name,
```

### Comparing `doppyler-0.0.8/doppyler/const.py` & `doppyler-0.0.9/doppyler/const.py`

 * *Files identical despite different names*

### Comparing `doppyler-0.0.8/doppyler/exceptions.py` & `doppyler-0.0.9/doppyler/exceptions.py`

 * *Files identical despite different names*

### Comparing `doppyler-0.0.8/doppyler/model/alarm.py` & `doppyler-0.0.9/doppyler/model/alarm.py`

 * *Files identical despite different names*

### Comparing `doppyler-0.0.8/doppyler/model/color.py` & `doppyler-0.0.9/doppyler/model/color.py`

 * *Files identical despite different names*

### Comparing `doppyler-0.0.8/doppyler/model/doppler.py` & `doppyler-0.0.9/doppyler/model/doppler.py`

 * *Files 0% similar despite different names*

```diff
@@ -673,29 +673,35 @@
         self, button_num: int
     ) -> SmartButtonConfiguration:
         """Get the smart button configuration for the device."""
         smart_button_config_dict = await self._call_api(f"hardware/button{button_num}")
         return SmartButtonConfiguration.from_dict(smart_button_config_dict)
 
     async def set_smart_button_configuration(
-        self, button_num: int, url: str | None = None, color: Color | None = None
+        self,
+        button_num: int,
+        url: str | None = None,
+        command: str | None = None,
+        color: Color | None = None,
     ) -> SmartButtonConfiguration:
         """Set the smart button configuration for the device."""
-        if url is None or color is None:
+        if url is None or color is None or command is None:
             smart_button_config = await self.get_smart_button_configuration(button_num)
         else:
-            smart_button_config = SmartButtonConfiguration(
-                "", button_num, "HA", Color(0, 0, 0)
-            )
+            smart_button_config = SmartButtonConfiguration("", "HA", Color(0, 0, 0))
         if url is not None:
             smart_button_config.webhook_url = url
         if color is not None:
             smart_button_config.color = color
+        if command is not None:
+            smart_button_config.command = command
         smart_button_config_dict = await self._call_api(
-            f"hardware/button{button_num}", "PUT", smart_button_config.to_dict()
+            f"hardware/button{button_num}",
+            "PUT",
+            {**smart_button_config.to_dict(), "data": str(button_num)},
         )
         return SmartButtonConfiguration.from_dict(smart_button_config_dict)
 
     async def set_main_display_text(self, mdt: MainDisplayText) -> MainDisplayText:
         """Set Scrolling Text on the main display."""
         data = mdt.to_dict()
         params = await self._call_api("hardware/display-text", "PUT", data)
```

### Comparing `doppyler-0.0.8/doppyler/model/light_bar.py` & `doppyler-0.0.9/doppyler/model/light_bar.py`

 * *Files identical despite different names*

### Comparing `doppyler-0.0.8/doppyler/model/main_display_text.py` & `doppyler-0.0.9/doppyler/model/main_display_text.py`

 * *Files identical despite different names*

### Comparing `doppyler-0.0.8/doppyler/model/mini_display_number.py` & `doppyler-0.0.9/doppyler/model/mini_display_number.py`

 * *Files identical despite different names*

### Comparing `doppyler-0.0.8/doppyler/model/weather.py` & `doppyler-0.0.9/doppyler/model/weather.py`

 * *Files identical despite different names*

### Comparing `doppyler-0.0.8/doppyler/model/wifi.py` & `doppyler-0.0.9/doppyler/model/wifi.py`

 * *Files identical despite different names*

### Comparing `doppyler-0.0.8/doppyler.egg-info/PKG-INFO` & `doppyler-0.0.9/doppyler.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doppyler
-Version: 0.0.8
+Version: 0.0.9
 Summary: A library to interact with the Sandman Doppler Clock API
 Home-page: https://github.com/pa-innovation/doppyler
 Author: Sandman Doppler
 Author-email: hi@paloaltoinnovation.com
 License: UNKNOWN
 Keywords: doppyler
 Platform: UNKNOWN
```

### Comparing `doppyler-0.0.8/doppyler.egg-info/SOURCES.txt` & `doppyler-0.0.9/doppyler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `doppyler-0.0.8/setup.py` & `doppyler-0.0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,10 +26,10 @@
     include_package_data=True,
     keywords="doppyler",
     name="doppyler",
     packages=find_packages(include=["doppyler", "doppyler.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/pa-innovation/doppyler",
-    version="0.0.8",
+    version="0.0.9",
     zip_safe=False,
 )
```

