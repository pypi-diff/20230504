# Comparing `tmp/aioruckus-0.23.tar.gz` & `tmp/aioruckus-0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioruckus-0.23.tar", last modified: Sat Apr  1 05:14:59 2023, max compression
+gzip compressed data, was "aioruckus-0.24.tar", last modified: Thu May  4 07:13:57 2023, max compression
```

## Comparing `aioruckus-0.23.tar` & `aioruckus-0.24.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 tony      (1000) tony      (1000)        0 2023-04-01 05:14:59.976438 aioruckus-0.23/
--rw-r--r--   0 tony      (1000) tony      (1000)      681 2023-03-23 10:24:18.000000 aioruckus-0.23/LICENSE
--rw-r--r--   0 tony      (1000) tony      (1000)     2543 2023-04-01 05:14:59.976438 aioruckus-0.23/PKG-INFO
--rw-r--r--   0 tony      (1000) tony      (1000)     2065 2023-03-24 02:14:00.000000 aioruckus-0.23/README.md
-drwxr-xr-x   0 tony      (1000) tony      (1000)        0 2023-04-01 05:14:59.976438 aioruckus-0.23/aioruckus/
--rw-r--r--   0 tony      (1000) tony      (1000)      114 2023-03-23 10:24:18.000000 aioruckus-0.23/aioruckus/__init__.py
--rw-r--r--   0 tony      (1000) tony      (1000)     6344 2023-03-27 00:18:32.000000 aioruckus-0.23/aioruckus/ajaxsession.py
--rw-r--r--   0 tony      (1000) tony      (1000)     1117 2023-04-01 05:10:33.000000 aioruckus-0.23/aioruckus/const.py
--rw-r--r--   0 tony      (1000) tony      (1000)      110 2023-03-23 13:22:20.000000 aioruckus-0.23/aioruckus/exceptions.py
--rw-r--r--   0 tony      (1000) tony      (1000)    10442 2023-03-23 13:47:42.000000 aioruckus-0.23/aioruckus/ruckusapi.py
-drwxr-xr-x   0 tony      (1000) tony      (1000)        0 2023-04-01 05:14:59.976438 aioruckus-0.23/aioruckus.egg-info/
--rw-r--r--   0 tony      (1000) tony      (1000)     2543 2023-04-01 05:14:59.000000 aioruckus-0.23/aioruckus.egg-info/PKG-INFO
--rw-r--r--   0 tony      (1000) tony      (1000)      349 2023-04-01 05:14:59.000000 aioruckus-0.23/aioruckus.egg-info/SOURCES.txt
--rw-r--r--   0 tony      (1000) tony      (1000)        1 2023-04-01 05:14:59.000000 aioruckus-0.23/aioruckus.egg-info/dependency_links.txt
--rw-r--r--   0 tony      (1000) tony      (1000)       16 2023-04-01 05:14:59.000000 aioruckus-0.23/aioruckus.egg-info/top_level.txt
--rw-r--r--   0 tony      (1000) tony      (1000)       96 2023-03-31 09:47:25.000000 aioruckus-0.23/pyproject.toml
--rw-r--r--   0 tony      (1000) tony      (1000)      568 2023-04-01 05:14:59.976438 aioruckus-0.23/setup.cfg
-drwxr-xr-x   0 tony      (1000) tony      (1000)        0 2023-04-01 05:14:59.976438 aioruckus-0.23/tests/
--rw-r--r--   0 tony      (1000) tony      (1000)      373 2023-03-23 13:15:00.000000 aioruckus-0.23/tests/__init__.py
--rw-r--r--   0 tony      (1000) tony      (1000)      755 2023-03-23 10:24:18.000000 aioruckus-0.23/tests/test_connection.py
--rw-r--r--   0 tony      (1000) tony      (1000)     1399 2023-03-23 10:24:18.000000 aioruckus-0.23/tests/test_data.py
+drwxr-xr-x   0 tony      (1000) tony      (1000)        0 2023-05-04 07:13:57.161026 aioruckus-0.24/
+-rw-r--r--   0 tony      (1000) tony      (1000)      681 2023-04-22 10:29:47.000000 aioruckus-0.24/LICENSE
+-rw-r--r--   0 tony      (1000) tony      (1000)     3760 2023-05-04 07:13:57.161026 aioruckus-0.24/PKG-INFO
+-rw-r--r--   0 tony      (1000) tony      (1000)     3281 2023-05-04 04:16:11.000000 aioruckus-0.24/README.md
+drwxr-xr-x   0 tony      (1000) tony      (1000)        0 2023-05-04 07:13:57.161026 aioruckus-0.24/aioruckus/
+-rw-r--r--   0 tony      (1000) tony      (1000)      166 2023-04-23 12:21:01.000000 aioruckus-0.24/aioruckus/__init__.py
+-rw-r--r--   0 tony      (1000) tony      (1000)     6400 2023-04-24 13:31:05.000000 aioruckus-0.24/aioruckus/ajaxsession.py
+-rw-r--r--   0 tony      (1000) tony      (1000)     1598 2023-05-04 04:08:16.000000 aioruckus-0.24/aioruckus/const.py
+-rw-r--r--   0 tony      (1000) tony      (1000)      110 2023-04-22 10:29:47.000000 aioruckus-0.24/aioruckus/exceptions.py
+-rw-r--r--   0 tony      (1000) tony      (1000)    21469 2023-05-04 04:11:53.000000 aioruckus-0.24/aioruckus/ruckusapi.py
+drwxr-xr-x   0 tony      (1000) tony      (1000)        0 2023-05-04 07:13:57.161026 aioruckus-0.24/aioruckus.egg-info/
+-rw-r--r--   0 tony      (1000) tony      (1000)     3760 2023-05-04 07:13:57.000000 aioruckus-0.24/aioruckus.egg-info/PKG-INFO
+-rw-r--r--   0 tony      (1000) tony      (1000)      349 2023-05-04 07:13:57.000000 aioruckus-0.24/aioruckus.egg-info/SOURCES.txt
+-rw-r--r--   0 tony      (1000) tony      (1000)        1 2023-05-04 07:13:57.000000 aioruckus-0.24/aioruckus.egg-info/dependency_links.txt
+-rw-r--r--   0 tony      (1000) tony      (1000)       16 2023-05-04 07:13:57.000000 aioruckus-0.24/aioruckus.egg-info/top_level.txt
+-rw-r--r--   0 tony      (1000) tony      (1000)       96 2023-05-04 07:12:00.000000 aioruckus-0.24/pyproject.toml
+-rw-r--r--   0 tony      (1000) tony      (1000)      568 2023-05-04 07:13:57.161026 aioruckus-0.24/setup.cfg
+drwxr-xr-x   0 tony      (1000) tony      (1000)        0 2023-05-04 07:13:57.161026 aioruckus-0.24/tests/
+-rw-r--r--   0 tony      (1000) tony      (1000)      373 2023-04-22 10:29:47.000000 aioruckus-0.24/tests/__init__.py
+-rw-r--r--   0 tony      (1000) tony      (1000)      755 2023-04-22 10:29:47.000000 aioruckus-0.24/tests/test_connection.py
+-rw-r--r--   0 tony      (1000) tony      (1000)     1399 2023-04-22 10:29:47.000000 aioruckus-0.24/tests/test_data.py
```

### Comparing `aioruckus-0.23/LICENSE` & `aioruckus-0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `aioruckus-0.23/PKG-INFO` & `aioruckus-0.24/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,72 +1,89 @@
 Metadata-Version: 2.1
 Name: aioruckus
-Version: 0.23
+Version: 0.24
 Summary: Python API to interact with Ruckus Unleashed and ZoneDirector devices.
 Home-page: https://github.com/ms264556/aioruckus
 Author: ms264556
 Author-email: bsd0@patterni.city
 License: BSD0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # aioruckus
 
-A Python API which interacts with Ruckus Unleashed and ZoneDirector devices.
+A Python API which interacts with Ruckus Unleashed and ZoneDirector devices via their AJAX Web Service interface.
 
 Compatible with all Ruckus Unleashed versions, and Ruckus ZoneDirector versions 9.10 onwards.
 
 ## How to install
 
 ```bash
 pip install aioruckus
 ```
 
 ## Usage
 
-Functions are defined within an [async](https://docs.python.org/3/library/asyncio.html) [context manager](https://docs.python.org/3/reference/datamodel.html#context-managers), so you will have to create an event loop instead of calling the functions directly in a shell.
+Functions are defined within an [async](https://docs.python.org/3/library/asyncio.html) [context manager](https://docs.python.org/3/reference/datamodel.html#context-managers), so you will have to use [asyncio](https://docs.python.org/3/library/asyncio.html) rather than calling the functions directly in a shell.
 
 ```python
 from aioruckus import AjaxSession, SystemStat
 import asyncio
 
 async def test_aioruckus():
     
     async with AjaxSession.async_create("<ruckus ip>", "<ruckus user>", "<ruckus password>") as session:
         ruckus = session.api
 
         wlans = await ruckus.get_wlans()
-        wlan_groups = await ruckus.get_wlan_groups()
+        wlan_groups = await ruckus.get_wlan_groups() # WLAN Groups are CLI-only on Unleashed
         aps = await ruckus.get_aps()
         ap_groups = await ruckus.get_ap_groups()
         mesh = await ruckus.get_mesh_info()
         default_system_info = await ruckus.get_system_info()
         all_system_info = await ruckus.get_system_info(SystemStat.ALL)
         active_clients = await ruckus.get_active_clients()
-        inactive_clients = await ruckus.get_inactive_clients() # empty on Unleashed
+        inactive_clients = await ruckus.get_inactive_clients() # always empty on Unleashed
         blocked = await ruckus.get_blocked_client_macs()
-        syslog = await api.get_syslog()
+        syslog = await ruckus.get_syslog()
 
         await ruckus.do_block_client("60:ab:de:ad:be:ef")
         await ruckus.do_unblock_client("60:ab:de:ad:be:ef")
 
         await ruckus.do_disable_wlan("my ssid")
         await ruckus.do_enable_wlan("my ssid")
 
         await ruckus.do_set_wlan_password("my ssid", "blah>blah<")
 
+        await ruckus.do_add_wlan_group("new empty wlangroup", "empty group added by aioruckus")
+        await ruckus.do_add_wlan_group("new full wlangroup", "group added by aioruckus", wlans)
+
+        wlan_group_template = next((wlang for wlang in wlan_groups if wlang["name"] == "Default"), None)
+        await ruckus.do_clone_wlan_group(wlan_group_template, "Copy of Default")
+
+        await ruckus.do_delete_wlan_group("Copy of Default")
+
+        await ruckus.do_add_wlan("my new sid", passphrase="mypassphrase" )
+        await ruckus.do_edit_wlan("my new sid", {"ofdm-rate-only": True})
+
+        template_wlan = next((wlan for wlan in wlans if wlan["name"] == "my ssid"), None)
+        await ruckus.do_clone_wlan(template_wlan, "my newer sid")
+        await ruckus.do_delete_wlan("my newer sid")
+
         await ruckus.do_hide_ap_leds("24:79:de:ad:be:ef")
         await ruckus.do_show_ap_leds("24:79:de:ad:be:ef")
         
-        await api.do_restart_ap("24:79:de:ad:be:ef")
-
+        await ruckus.do_restart_ap("24:79:de:ad:be:ef")
 
 asyncio.run(test_aioruckus())
 ```
 
 ### Other Python APIs for Ruckus Unleashed
 
 This project was originally a fork of [pyuckus](https://github.com/gabe565/pyruckus), which provides similar query functionality by controlling an SSH CLI session.
+
+There is also [scrapli](https://github.com/carlmontanari/scrapli) support for the Ruckus Unleashed SSH CLI via [scrapli community](https://github.com/scrapli/scrapli_community).  
+Authentication and privilege levels are implemented, but no templates are implemented as of April 2023.
```

### Comparing `aioruckus-0.23/README.md` & `aioruckus-0.24/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,74 @@
 # aioruckus
 
-A Python API which interacts with Ruckus Unleashed and ZoneDirector devices.
+A Python API which interacts with Ruckus Unleashed and ZoneDirector devices via their AJAX Web Service interface.
 
 Compatible with all Ruckus Unleashed versions, and Ruckus ZoneDirector versions 9.10 onwards.
 
 ## How to install
 
 ```bash
 pip install aioruckus
 ```
 
 ## Usage
 
-Functions are defined within an [async](https://docs.python.org/3/library/asyncio.html) [context manager](https://docs.python.org/3/reference/datamodel.html#context-managers), so you will have to create an event loop instead of calling the functions directly in a shell.
+Functions are defined within an [async](https://docs.python.org/3/library/asyncio.html) [context manager](https://docs.python.org/3/reference/datamodel.html#context-managers), so you will have to use [asyncio](https://docs.python.org/3/library/asyncio.html) rather than calling the functions directly in a shell.
 
 ```python
 from aioruckus import AjaxSession, SystemStat
 import asyncio
 
 async def test_aioruckus():
     
     async with AjaxSession.async_create("<ruckus ip>", "<ruckus user>", "<ruckus password>") as session:
         ruckus = session.api
 
         wlans = await ruckus.get_wlans()
-        wlan_groups = await ruckus.get_wlan_groups()
+        wlan_groups = await ruckus.get_wlan_groups() # WLAN Groups are CLI-only on Unleashed
         aps = await ruckus.get_aps()
         ap_groups = await ruckus.get_ap_groups()
         mesh = await ruckus.get_mesh_info()
         default_system_info = await ruckus.get_system_info()
         all_system_info = await ruckus.get_system_info(SystemStat.ALL)
         active_clients = await ruckus.get_active_clients()
-        inactive_clients = await ruckus.get_inactive_clients() # empty on Unleashed
+        inactive_clients = await ruckus.get_inactive_clients() # always empty on Unleashed
         blocked = await ruckus.get_blocked_client_macs()
-        syslog = await api.get_syslog()
+        syslog = await ruckus.get_syslog()
 
         await ruckus.do_block_client("60:ab:de:ad:be:ef")
         await ruckus.do_unblock_client("60:ab:de:ad:be:ef")
 
         await ruckus.do_disable_wlan("my ssid")
         await ruckus.do_enable_wlan("my ssid")
 
         await ruckus.do_set_wlan_password("my ssid", "blah>blah<")
 
+        await ruckus.do_add_wlan_group("new empty wlangroup", "empty group added by aioruckus")
+        await ruckus.do_add_wlan_group("new full wlangroup", "group added by aioruckus", wlans)
+
+        wlan_group_template = next((wlang for wlang in wlan_groups if wlang["name"] == "Default"), None)
+        await ruckus.do_clone_wlan_group(wlan_group_template, "Copy of Default")
+
+        await ruckus.do_delete_wlan_group("Copy of Default")
+
+        await ruckus.do_add_wlan("my new sid", passphrase="mypassphrase" )
+        await ruckus.do_edit_wlan("my new sid", {"ofdm-rate-only": True})
+
+        template_wlan = next((wlan for wlan in wlans if wlan["name"] == "my ssid"), None)
+        await ruckus.do_clone_wlan(template_wlan, "my newer sid")
+        await ruckus.do_delete_wlan("my newer sid")
+
         await ruckus.do_hide_ap_leds("24:79:de:ad:be:ef")
         await ruckus.do_show_ap_leds("24:79:de:ad:be:ef")
         
-        await api.do_restart_ap("24:79:de:ad:be:ef")
-
+        await ruckus.do_restart_ap("24:79:de:ad:be:ef")
 
 asyncio.run(test_aioruckus())
 ```
 
 ### Other Python APIs for Ruckus Unleashed
 
 This project was originally a fork of [pyuckus](https://github.com/gabe565/pyruckus), which provides similar query functionality by controlling an SSH CLI session.
+
+There is also [scrapli](https://github.com/carlmontanari/scrapli) support for the Ruckus Unleashed SSH CLI via [scrapli community](https://github.com/scrapli/scrapli_community).  
+Authentication and privilege levels are implemented, but no templates are implemented as of April 2023.
```

### Comparing `aioruckus-0.23/aioruckus/ajaxsession.py` & `aioruckus-0.24/aioruckus/ajaxsession.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     async def login(self) -> None:
         """Create HTTPS AJAX session."""
         # locate the admin pages: /admin/* for Unleashed and ZD 9.x, /admin10/* for ZD 10.x
         try:
             async with self.websession.head(f"https://{self.host}", timeout=3, allow_redirects=False) as head:
                 self.__login_url = head.headers["Location"]
                 self.base_url, login_page = self.__login_url.rsplit("/", 1)
-                if login_page == "index.html": # maybe temporary Unleashed Rebuilding placeholder page is showing
+                if login_page == "index.html" or login_page == "wizard.jsp": # Unleashed Rebuilding or Setup Wizard
                     raise ConnectionRefusedError(CONNECT_ERROR_TEMPORARY)
                 self.cmdstat_url = self.base_url + "/_cmdstat.jsp"
                 self.conf_url = self.base_url + "/_conf.jsp"
         except aiohttp.client_exceptions.ClientConnectorError as cerr:
             raise ConnectionError(CONNECT_ERROR_EOF) from cerr
         except asyncio.exceptions.TimeoutError as terr:
             raise ConnectionError(CONNECT_ERROR_TIMEOUT) from terr
@@ -102,22 +102,22 @@
                 timeout=3,
                 allow_redirects=False,
             ):
                 pass
             if self.__auto_cleanup_websession:
                 await self.websession.close()
 
-    async def request(self, cmd: str, data: str, retrying: bool = False) -> str:
+    async def request(self, cmd: str, data: str, timeout: int | None = None, retrying: bool = False) -> str:
         """Request data"""
-        async with self.websession.post(cmd, data=data, headers={"Content-Type": "text/xml"}, allow_redirects=False) as response:
+        async with self.websession.post(cmd, data=data, headers={"Content-Type": "text/xml"}, timeout=timeout, allow_redirects=False) as response:
             if response.status == 302:  # if the session is dead then we're redirected to the login page
                 if retrying:  # we tried logging in again, but the redirect still happens - maybe password changed?
                     raise PermissionError(AJAX_POST_REDIRECTED_ERROR)
                 await self.login()  # try logging in again, then retry post
-                return await self.request(cmd, data, retrying=True)
+                return await self.request(cmd, data, timeout, retrying=True)
             result_text = await response.text()
             if not result_text or result_text == "\n":  # if the ajax request payload wasn't understood then we get an empty page back
                 raise RuntimeError(AJAX_POST_NORESULT_ERROR)
             return result_text
 
     @property
     def api(self):
```

### Comparing `aioruckus-0.23/aioruckus.egg-info/PKG-INFO` & `aioruckus-0.24/aioruckus.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,72 +1,89 @@
 Metadata-Version: 2.1
 Name: aioruckus
-Version: 0.23
+Version: 0.24
 Summary: Python API to interact with Ruckus Unleashed and ZoneDirector devices.
 Home-page: https://github.com/ms264556/aioruckus
 Author: ms264556
 Author-email: bsd0@patterni.city
 License: BSD0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # aioruckus
 
-A Python API which interacts with Ruckus Unleashed and ZoneDirector devices.
+A Python API which interacts with Ruckus Unleashed and ZoneDirector devices via their AJAX Web Service interface.
 
 Compatible with all Ruckus Unleashed versions, and Ruckus ZoneDirector versions 9.10 onwards.
 
 ## How to install
 
 ```bash
 pip install aioruckus
 ```
 
 ## Usage
 
-Functions are defined within an [async](https://docs.python.org/3/library/asyncio.html) [context manager](https://docs.python.org/3/reference/datamodel.html#context-managers), so you will have to create an event loop instead of calling the functions directly in a shell.
+Functions are defined within an [async](https://docs.python.org/3/library/asyncio.html) [context manager](https://docs.python.org/3/reference/datamodel.html#context-managers), so you will have to use [asyncio](https://docs.python.org/3/library/asyncio.html) rather than calling the functions directly in a shell.
 
 ```python
 from aioruckus import AjaxSession, SystemStat
 import asyncio
 
 async def test_aioruckus():
     
     async with AjaxSession.async_create("<ruckus ip>", "<ruckus user>", "<ruckus password>") as session:
         ruckus = session.api
 
         wlans = await ruckus.get_wlans()
-        wlan_groups = await ruckus.get_wlan_groups()
+        wlan_groups = await ruckus.get_wlan_groups() # WLAN Groups are CLI-only on Unleashed
         aps = await ruckus.get_aps()
         ap_groups = await ruckus.get_ap_groups()
         mesh = await ruckus.get_mesh_info()
         default_system_info = await ruckus.get_system_info()
         all_system_info = await ruckus.get_system_info(SystemStat.ALL)
         active_clients = await ruckus.get_active_clients()
-        inactive_clients = await ruckus.get_inactive_clients() # empty on Unleashed
+        inactive_clients = await ruckus.get_inactive_clients() # always empty on Unleashed
         blocked = await ruckus.get_blocked_client_macs()
-        syslog = await api.get_syslog()
+        syslog = await ruckus.get_syslog()
 
         await ruckus.do_block_client("60:ab:de:ad:be:ef")
         await ruckus.do_unblock_client("60:ab:de:ad:be:ef")
 
         await ruckus.do_disable_wlan("my ssid")
         await ruckus.do_enable_wlan("my ssid")
 
         await ruckus.do_set_wlan_password("my ssid", "blah>blah<")
 
+        await ruckus.do_add_wlan_group("new empty wlangroup", "empty group added by aioruckus")
+        await ruckus.do_add_wlan_group("new full wlangroup", "group added by aioruckus", wlans)
+
+        wlan_group_template = next((wlang for wlang in wlan_groups if wlang["name"] == "Default"), None)
+        await ruckus.do_clone_wlan_group(wlan_group_template, "Copy of Default")
+
+        await ruckus.do_delete_wlan_group("Copy of Default")
+
+        await ruckus.do_add_wlan("my new sid", passphrase="mypassphrase" )
+        await ruckus.do_edit_wlan("my new sid", {"ofdm-rate-only": True})
+
+        template_wlan = next((wlan for wlan in wlans if wlan["name"] == "my ssid"), None)
+        await ruckus.do_clone_wlan(template_wlan, "my newer sid")
+        await ruckus.do_delete_wlan("my newer sid")
+
         await ruckus.do_hide_ap_leds("24:79:de:ad:be:ef")
         await ruckus.do_show_ap_leds("24:79:de:ad:be:ef")
         
-        await api.do_restart_ap("24:79:de:ad:be:ef")
-
+        await ruckus.do_restart_ap("24:79:de:ad:be:ef")
 
 asyncio.run(test_aioruckus())
 ```
 
 ### Other Python APIs for Ruckus Unleashed
 
 This project was originally a fork of [pyuckus](https://github.com/gabe565/pyruckus), which provides similar query functionality by controlling an SSH CLI session.
+
+There is also [scrapli](https://github.com/carlmontanari/scrapli) support for the Ruckus Unleashed SSH CLI via [scrapli community](https://github.com/scrapli/scrapli_community).  
+Authentication and privilege levels are implemented, but no templates are implemented as of April 2023.
```

### Comparing `aioruckus-0.23/setup.cfg` & `aioruckus-0.24/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = aioruckus
-version = 0.23
+version = 0.24
 author = ms264556
 author_email = bsd0@patterni.city
 description = Python API to interact with Ruckus Unleashed and ZoneDirector devices.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ms264556/aioruckus
 classifiers =
```

### Comparing `aioruckus-0.23/tests/test_connection.py` & `aioruckus-0.24/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `aioruckus-0.23/tests/test_data.py` & `aioruckus-0.24/tests/test_data.py`

 * *Files identical despite different names*

