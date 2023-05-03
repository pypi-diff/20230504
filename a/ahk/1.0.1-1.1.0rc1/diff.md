# Comparing `tmp/ahk-1.0.1.tar.gz` & `tmp/ahk-1.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ahk-1.0.1.tar", last modified: Tue May  2 23:45:45 2023, max compression
+gzip compressed data, was "ahk-1.1.0rc1.tar", last modified: Wed May  3 23:02:32 2023, max compression
```

## Comparing `ahk-1.0.1.tar` & `ahk-1.1.0rc1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:45:45.257030 ahk-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-02 23:45:34.000000 ahk-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    18230 2023-05-02 23:45:45.257030 ahk-1.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:45:45.253030 ahk-1.0.1/ahk/
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-02 23:45:34.000000 ahk-1.0.1/ahk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:45:45.257030 ahk-1.0.1/ahk/_async/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-02 23:45:34.000000 ahk-1.0.1/ahk/_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   178319 2023-05-02 23:45:34.000000 ahk-1.0.1/ahk/_async/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    42426 2023-05-02 23:45:34.000000 ahk-1.0.1/ahk/_async/transport.py
--rw-r--r--   0 runner    (1001) docker     (123)    28809 2023-05-02 23:45:34.000000 ahk-1.0.1/ahk/_async/window.py
--rw-r--r--   0 runner    (1001) docker     (123)    82888 2023-05-02 23:45:34.000000 ahk-1.0.1/ahk/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13992 2023-05-02 23:45:34.000000 ahk-1.0.1/ahk/_hotkey.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:45:45.257030 ahk-1.0.1/ahk/_sync/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-02 23:45:34.000000 ahk-1.0.1/ahk/_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   172602 2023-05-02 23:45:34.000000 ahk-1.0.1/ahk/_sync/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    38263 2023-05-02 23:45:34.000000 ahk-1.0.1/ahk/_sync/transport.py
--rw-r--r--   0 runner    (1001) docker     (123)    26252 2023-05-02 23:45:34.000000 ahk-1.0.1/ahk/_sync/window.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-02 23:45:34.000000 ahk-1.0.1/ahk/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-05-02 23:45:34.000000 ahk-1.0.1/ahk/directives.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-02 23:45:34.000000 ahk-1.0.1/ahk/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-05-02 23:45:34.000000 ahk-1.0.1/ahk/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)    11435 2023-05-02 23:45:34.000000 ahk-1.0.1/ahk/message.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 23:45:34.000000 ahk-1.0.1/ahk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:45:45.257030 ahk-1.0.1/ahk/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    78237 2023-05-02 23:45:34.000000 ahk-1.0.1/ahk/templates/daemon.ahk
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-05-02 23:45:34.000000 ahk-1.0.1/ahk/templates/hotkeys.ahk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:45:45.257030 ahk-1.0.1/ahk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18230 2023-05-02 23:45:45.000000 ahk-1.0.1/ahk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-02 23:45:45.000000 ahk-1.0.1/ahk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 23:45:45.000000 ahk-1.0.1/ahk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-02 23:45:45.000000 ahk-1.0.1/ahk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-02 23:45:45.000000 ahk-1.0.1/ahk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-02 23:45:34.000000 ahk-1.0.1/buildunasync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:45:45.257030 ahk-1.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    17347 2023-05-02 23:45:34.000000 ahk-1.0.1/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-02 23:45:34.000000 ahk-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-02 23:45:45.257030 ahk-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 23:45:34.000000 ahk-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:02:32.551648 ahk-1.1.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-03 23:02:21.000000 ahk-1.1.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18814 2023-05-03 23:02:32.551648 ahk-1.1.0rc1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:02:32.547648 ahk-1.1.0rc1/ahk/
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-03 23:02:21.000000 ahk-1.1.0rc1/ahk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:02:32.551648 ahk-1.1.0rc1/ahk/_async/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-03 23:02:21.000000 ahk-1.1.0rc1/ahk/_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   179907 2023-05-03 23:02:21.000000 ahk-1.1.0rc1/ahk/_async/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43081 2023-05-03 23:02:21.000000 ahk-1.1.0rc1/ahk/_async/transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28809 2023-05-03 23:02:21.000000 ahk-1.1.0rc1/ahk/_async/window.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83313 2023-05-03 23:02:21.000000 ahk-1.1.0rc1/ahk/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13992 2023-05-03 23:02:21.000000 ahk-1.1.0rc1/ahk/_hotkey.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:02:32.551648 ahk-1.1.0rc1/ahk/_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-03 23:02:21.000000 ahk-1.1.0rc1/ahk/_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   174154 2023-05-03 23:02:21.000000 ahk-1.1.0rc1/ahk/_sync/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38885 2023-05-03 23:02:21.000000 ahk-1.1.0rc1/ahk/_sync/transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26252 2023-05-03 23:02:21.000000 ahk-1.1.0rc1/ahk/_sync/window.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-03 23:02:21.000000 ahk-1.1.0rc1/ahk/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-05-03 23:02:21.000000 ahk-1.1.0rc1/ahk/directives.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-03 23:02:21.000000 ahk-1.1.0rc1/ahk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-05-03 23:02:21.000000 ahk-1.1.0rc1/ahk/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11435 2023-05-03 23:02:21.000000 ahk-1.1.0rc1/ahk/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 23:02:21.000000 ahk-1.1.0rc1/ahk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:02:32.551648 ahk-1.1.0rc1/ahk/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    78662 2023-05-03 23:02:21.000000 ahk-1.1.0rc1/ahk/templates/daemon.ahk
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-05-03 23:02:21.000000 ahk-1.1.0rc1/ahk/templates/hotkeys.ahk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:02:32.551648 ahk-1.1.0rc1/ahk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18814 2023-05-03 23:02:32.000000 ahk-1.1.0rc1/ahk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-03 23:02:32.000000 ahk-1.1.0rc1/ahk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 23:02:32.000000 ahk-1.1.0rc1/ahk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-03 23:02:32.000000 ahk-1.1.0rc1/ahk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-03 23:02:32.000000 ahk-1.1.0rc1/ahk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-03 23:02:21.000000 ahk-1.1.0rc1/buildunasync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:02:32.551648 ahk-1.1.0rc1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    17928 2023-05-03 23:02:21.000000 ahk-1.1.0rc1/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-03 23:02:21.000000 ahk-1.1.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-03 23:02:32.551648 ahk-1.1.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 23:02:21.000000 ahk-1.1.0rc1/setup.py
```

### Comparing `ahk-1.0.1/PKG-INFO` & `ahk-1.1.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahk
-Version: 1.0.1
+Version: 1.1.0rc1
 Summary: A Python wrapper for AHK
 Home-page: https://github.com/spyoungtech/ahk
 Author: Spencer Young
 Author-email: spencer.young@spyoung.com
 Keywords: ahk,autohotkey,windows,mouse,keyboard,automation,pyautogui
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Desktop Environment
@@ -341,14 +341,36 @@
 from ahk.directives import NoTrayIcon
 
 ahk = AHK(directives=[NoTrayIcon])
 ```
 
 By default, some directives are automatically added to ensure functionality and are merged with any user-provided directives.
 
+## Menu tray icon
+
+As discussed above, you can hide the tray icon if you wish. Additionally, there are some methods available for
+customizing the tray icon.
+
+
+```python
+from ahk import AHK
+ahk = AHK()
+
+# change the tray icon (in this case, using a builtin system icon)
+ahk.menu_tray_icon('Shell32.dll', 174)
+# revert it back to the original:
+ahk.menu_tray_icon()
+
+# change the tooltip that shows up when hovering the mouse over the tray icon
+ahk.menu_tray_tooltip('My Program Name')
+
+# Show the tray icon that was previously hidden by ``NoTrayIcon``
+ahk.menu_tray_icon_show()
+```
+
 ## Registry methods
 
 You can read/write/delete registry keys:
 
 ```python
 from ahk import AHK
 ahk = AHK()
```

### Comparing `ahk-1.0.1/ahk/__init__.py` & `ahk-1.1.0rc1/ahk/__init__.py`

 * *Files identical despite different names*

### Comparing `ahk-1.0.1/ahk/_async/engine.py` & `ahk-1.1.0rc1/ahk/_async/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -1363,14 +1363,51 @@
         else:
             args.append('')
         await self._transport.function_call('AHKShowToolTip', args)
 
     async def hide_tooltip(self, which: int = 1) -> None:
         await self.show_tooltip(which=which)
 
+    async def menu_tray_tooltip(self, value: str) -> None:
+        """
+        Change the menu tray icon tooltip that appears when hovering the mouse over the tray icon.
+        Does not affect tray icon for AHK processes started with :py:meth:`run_script` or ``blocking=False``
+
+        Uses the `Tip subcommand <https://www.autohotkey.com/docs/v1/lib/Menu.htm#Tip>`_
+        """
+
+        args = [value]
+        await self._transport.function_call('AHKMenuTrayTip', args)
+        return None
+
+    async def menu_tray_icon(self, filename: str = '*', icon_number: int = 1, freeze: Optional[bool] = None) -> None:
+        """
+        Change the tray icon menu.
+        Does not affect tray icon for AHK processes started with :py:meth:`run_script` or ``blocking=False``
+
+        Uses the `Icon subcommand <https://www.autohotkey.com/docs/v1/lib/Menu.htm#Icon>`_
+
+        If called with no parameters, the tray icon will be reset to the original default.
+        """
+        args = [filename, str(icon_number)]
+        if freeze is True:
+            args.append('1')
+        elif freeze is False:
+            args.append('0')
+        await self._transport.function_call('AHKMenuTrayIcon', args)
+        return None
+
+    async def menu_tray_icon_show(self) -> None:
+        """
+        Show ('unhide') the tray icon previously hidden by :py:class:`~ahk.directives.NoTrayIcon` directive.
+        Does not affect tray icon for AHK processes started with :py:meth:`run_script` or ``blocking=False``
+        """
+        await self._transport.function_call('AHKMenuTrayShow')
+        return None
+
     # fmt: off
     @overload
     async def sound_beep(self, frequency: int = 523, duration: int = 150) -> None: ...
     @overload
     async def sound_beep(self, frequency: int = 523, duration: int = 150, *, blocking: Literal[False]) -> AsyncFutureResult[None]: ...
     @overload
     async def sound_beep(self, frequency: int = 523, duration: int = 150, *, blocking: Literal[True]) -> None: ...
```

### Comparing `ahk-1.0.1/ahk/_async/transport.py` & `ahk-1.1.0rc1/ahk/_async/transport.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,14 +91,17 @@
     'AHKGetSendLevel',
     'AHKGetTitleMatchMode',
     'AHKGetTitleMatchSpeed',
     'AHKGetVolume',
     'AHKImageSearch',
     'AHKKeyState',
     'AHKKeyWait',
+    'AHKMenuTrayIcon',
+    'AHKMenuTrayShow',
+    'AHKMenuTrayTip',
     'AHKMouseClickDrag',
     'AHKMouseGetPos',
     'AHKMouseMove',
     'AHKPixelGetColor',
     'AHKPixelSearch',
     'AHKRegRead',
     'AHKRegWrite',
@@ -561,14 +564,20 @@
     async def function_call(self, function_name: Literal['AHKWinWaitClose'], args: Optional[List[str]] = None, *, blocking: bool = True, engine: Optional[AsyncAHK] = None) -> Union[None, AsyncFutureResult[None]]: ...
     @overload
     async def function_call(self, function_name: Literal['AHKRegRead'], args: Optional[List[str]] = None, *, blocking: bool = True) -> Union[str, AsyncFutureResult[str]]: ...
     @overload
     async def function_call(self, function_name: Literal['AHKRegWrite'], args: Optional[List[str]] = None, *, blocking: bool = True) -> Union[None, AsyncFutureResult[None]]: ...
     @overload
     async def function_call(self, function_name: Literal['AHKRegDelete'], args: Optional[List[str]] = None, *, blocking: bool = True) -> Union[None, AsyncFutureResult[None]]: ...
+    @overload
+    async def function_call(self, function_name: Literal['AHKMenuTrayTip'], args: Optional[List[str]] = None, *, blocking: bool = True) -> Union[None, AsyncFutureResult[None]]: ...
+    @overload
+    async def function_call(self, function_name: Literal['AHKMenuTrayIcon'], args: Optional[List[str]] = None, *, blocking: bool = True) -> Union[None, AsyncFutureResult[None]]: ...
+    @overload
+    async def function_call(self, function_name: Literal['AHKMenuTrayShow'], args: Optional[List[str]] = None, *, blocking: bool = True) -> Union[None, AsyncFutureResult[None]]: ...
 
     # fmt: on
 
     async def function_call(
         self,
         function_name: FunctionName,
         args: Optional[List[str]] = None,
```

### Comparing `ahk-1.0.1/ahk/_async/window.py` & `ahk-1.1.0rc1/ahk/_async/window.py`

 * *Files identical despite different names*

### Comparing `ahk-1.0.1/ahk/_constants.py` & `ahk-1.1.0rc1/ahk/_constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -2599,14 +2599,33 @@
 
 AHKBlockInput(ByRef command) {
     value := command[2]
     BlockInput, %value%
     return FormatNoValueResponse()
 }
 
+AHKMenuTrayTip(ByRef command) {
+    value := command[2]
+    Menu, Tray, Tip, %value%
+    return FormatNoValueResponse()
+}
+
+AHKMenuTrayShow(ByRef command) {
+    Menu, Tray, Icon
+    return FormatNoValueResponse()
+}
+
+AHKMenuTrayIcon(ByRef command) {
+    filename := command[2]
+    icon_number := command[3]
+    freeze := command[4]
+    Menu, Tray, Icon, %filename%, %icon_number%,%freeze%
+    return FormatNoValueResponse()
+}
+
 b64decode(ByRef pszString) {
     ; TODO load DLL globally for performance
     ; REF: https://docs.microsoft.com/en-us/windows/win32/api/wincrypt/nf-wincrypt-cryptstringtobinaryw
     ;  [in]      LPCSTR pszString,  A pointer to a string that contains the formatted string to be converted.
     ;  [in]      DWORD  cchString,  The number of characters of the formatted string to be converted, not including the terminating NULL character. If this parameter is zero, pszString is considered to be a null-terminated string.
     ;  [in]      DWORD  dwFlags,    Indicates the format of the string to be converted. (see table in link above)
     ;  [in]      BYTE   *pbBinary,  A pointer to a buffer that receives the returned sequence of bytes. If this parameter is NULL, the function calculates the length of the buffer needed and returns the size, in bytes, of required memory in the DWORD pointed to by pcbBinary.
```

### Comparing `ahk-1.0.1/ahk/_hotkey.py` & `ahk-1.1.0rc1/ahk/_hotkey.py`

 * *Files identical despite different names*

### Comparing `ahk-1.0.1/ahk/_sync/engine.py` & `ahk-1.1.0rc1/ahk/_sync/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -1352,14 +1352,51 @@
         else:
             args.append('')
         self._transport.function_call('AHKShowToolTip', args)
 
     def hide_tooltip(self, which: int = 1) -> None:
         self.show_tooltip(which=which)
 
+    def menu_tray_tooltip(self, value: str) -> None:
+        """
+        Change the menu tray icon tooltip that appears when hovering the mouse over the tray icon.
+        Does not affect tray icon for AHK processes started with :py:meth:`run_script` or ``blocking=False``
+
+        Uses the `Tip subcommand <https://www.autohotkey.com/docs/v1/lib/Menu.htm#Tip>`_
+        """
+
+        args = [value]
+        self._transport.function_call('AHKMenuTrayTip', args)
+        return None
+
+    def menu_tray_icon(self, filename: str = '*', icon_number: int = 1, freeze: Optional[bool] = None) -> None:
+        """
+        Change the tray icon menu.
+        Does not affect tray icon for AHK processes started with :py:meth:`run_script` or ``blocking=False``
+
+        Uses the `Icon subcommand <https://www.autohotkey.com/docs/v1/lib/Menu.htm#Icon>`_
+
+        If called with no parameters, the tray icon will be reset to the original default.
+        """
+        args = [filename, str(icon_number)]
+        if freeze is True:
+            args.append('1')
+        elif freeze is False:
+            args.append('0')
+        self._transport.function_call('AHKMenuTrayIcon', args)
+        return None
+
+    def menu_tray_icon_show(self) -> None:
+        """
+        Show ('unhide') the tray icon previously hidden by :py:class:`~ahk.directives.NoTrayIcon` directive.
+        Does not affect tray icon for AHK processes started with :py:meth:`run_script` or ``blocking=False``
+        """
+        self._transport.function_call('AHKMenuTrayShow')
+        return None
+
     # fmt: off
     @overload
     def sound_beep(self, frequency: int = 523, duration: int = 150) -> None: ...
     @overload
     def sound_beep(self, frequency: int = 523, duration: int = 150, *, blocking: Literal[False]) -> FutureResult[None]: ...
     @overload
     def sound_beep(self, frequency: int = 523, duration: int = 150, *, blocking: Literal[True]) -> None: ...
```

### Comparing `ahk-1.0.1/ahk/_sync/transport.py` & `ahk-1.1.0rc1/ahk/_sync/transport.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,14 +83,17 @@
     'AHKGetSendLevel',
     'AHKGetTitleMatchMode',
     'AHKGetTitleMatchSpeed',
     'AHKGetVolume',
     'AHKImageSearch',
     'AHKKeyState',
     'AHKKeyWait',
+    'AHKMenuTrayIcon',
+    'AHKMenuTrayShow',
+    'AHKMenuTrayTip',
     'AHKMouseClickDrag',
     'AHKMouseGetPos',
     'AHKMouseMove',
     'AHKPixelGetColor',
     'AHKPixelSearch',
     'AHKRegRead',
     'AHKRegWrite',
@@ -542,14 +545,20 @@
     def function_call(self, function_name: Literal['AHKWinWaitClose'], args: Optional[List[str]] = None, *, blocking: bool = True, engine: Optional[AHK] = None) -> Union[None, FutureResult[None]]: ...
     @overload
     def function_call(self, function_name: Literal['AHKRegRead'], args: Optional[List[str]] = None, *, blocking: bool = True) -> Union[str, FutureResult[str]]: ...
     @overload
     def function_call(self, function_name: Literal['AHKRegWrite'], args: Optional[List[str]] = None, *, blocking: bool = True) -> Union[None, FutureResult[None]]: ...
     @overload
     def function_call(self, function_name: Literal['AHKRegDelete'], args: Optional[List[str]] = None, *, blocking: bool = True) -> Union[None, FutureResult[None]]: ...
+    @overload
+    def function_call(self, function_name: Literal['AHKMenuTrayTip'], args: Optional[List[str]] = None, *, blocking: bool = True) -> Union[None, FutureResult[None]]: ...
+    @overload
+    def function_call(self, function_name: Literal['AHKMenuTrayIcon'], args: Optional[List[str]] = None, *, blocking: bool = True) -> Union[None, FutureResult[None]]: ...
+    @overload
+    def function_call(self, function_name: Literal['AHKMenuTrayShow'], args: Optional[List[str]] = None, *, blocking: bool = True) -> Union[None, FutureResult[None]]: ...
 
     # fmt: on
 
     def function_call(
         self,
         function_name: FunctionName,
         args: Optional[List[str]] = None,
```

### Comparing `ahk-1.0.1/ahk/_sync/window.py` & `ahk-1.1.0rc1/ahk/_sync/window.py`

 * *Files identical despite different names*

### Comparing `ahk-1.0.1/ahk/_utils.py` & `ahk-1.1.0rc1/ahk/_utils.py`

 * *Files identical despite different names*

### Comparing `ahk-1.0.1/ahk/directives.py` & `ahk-1.1.0rc1/ahk/directives.py`

 * *Files identical despite different names*

### Comparing `ahk-1.0.1/ahk/keys.py` & `ahk-1.1.0rc1/ahk/keys.py`

 * *Files identical despite different names*

### Comparing `ahk-1.0.1/ahk/message.py` & `ahk-1.1.0rc1/ahk/message.py`

 * *Files identical despite different names*

### Comparing `ahk-1.0.1/ahk/templates/daemon.ahk` & `ahk-1.1.0rc1/ahk/templates/daemon.ahk`

 * *Files 0% similar despite different names*

```diff
@@ -2596,14 +2596,33 @@
 
 AHKBlockInput(ByRef command) {
     value := command[2]
     BlockInput, %value%
     return FormatNoValueResponse()
 }
 
+AHKMenuTrayTip(ByRef command) {
+    value := command[2]
+    Menu, Tray, Tip, %value%
+    return FormatNoValueResponse()
+}
+
+AHKMenuTrayShow(ByRef command) {
+    Menu, Tray, Icon
+    return FormatNoValueResponse()
+}
+
+AHKMenuTrayIcon(ByRef command) {
+    filename := command[2]
+    icon_number := command[3]
+    freeze := command[4]
+    Menu, Tray, Icon, %filename%, %icon_number%,%freeze%
+    return FormatNoValueResponse()
+}
+
 b64decode(ByRef pszString) {
     ; TODO load DLL globally for performance
     ; REF: https://docs.microsoft.com/en-us/windows/win32/api/wincrypt/nf-wincrypt-cryptstringtobinaryw
     ;  [in]      LPCSTR pszString,  A pointer to a string that contains the formatted string to be converted.
     ;  [in]      DWORD  cchString,  The number of characters of the formatted string to be converted, not including the terminating NULL character. If this parameter is zero, pszString is considered to be a null-terminated string.
     ;  [in]      DWORD  dwFlags,    Indicates the format of the string to be converted. (see table in link above)
     ;  [in]      BYTE   *pbBinary,  A pointer to a buffer that receives the returned sequence of bytes. If this parameter is NULL, the function calculates the length of the buffer needed and returns the size, in bytes, of required memory in the DWORD pointed to by pcbBinary.
```

### Comparing `ahk-1.0.1/ahk/templates/hotkeys.ahk` & `ahk-1.1.0rc1/ahk/templates/hotkeys.ahk`

 * *Files identical despite different names*

### Comparing `ahk-1.0.1/ahk.egg-info/PKG-INFO` & `ahk-1.1.0rc1/ahk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahk
-Version: 1.0.1
+Version: 1.1.0rc1
 Summary: A Python wrapper for AHK
 Home-page: https://github.com/spyoungtech/ahk
 Author: Spencer Young
 Author-email: spencer.young@spyoung.com
 Keywords: ahk,autohotkey,windows,mouse,keyboard,automation,pyautogui
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Desktop Environment
@@ -341,14 +341,36 @@
 from ahk.directives import NoTrayIcon
 
 ahk = AHK(directives=[NoTrayIcon])
 ```
 
 By default, some directives are automatically added to ensure functionality and are merged with any user-provided directives.
 
+## Menu tray icon
+
+As discussed above, you can hide the tray icon if you wish. Additionally, there are some methods available for
+customizing the tray icon.
+
+
+```python
+from ahk import AHK
+ahk = AHK()
+
+# change the tray icon (in this case, using a builtin system icon)
+ahk.menu_tray_icon('Shell32.dll', 174)
+# revert it back to the original:
+ahk.menu_tray_icon()
+
+# change the tooltip that shows up when hovering the mouse over the tray icon
+ahk.menu_tray_tooltip('My Program Name')
+
+# Show the tray icon that was previously hidden by ``NoTrayIcon``
+ahk.menu_tray_icon_show()
+```
+
 ## Registry methods
 
 You can read/write/delete registry keys:
 
 ```python
 from ahk import AHK
 ahk = AHK()
```

### Comparing `ahk-1.0.1/ahk.egg-info/SOURCES.txt` & `ahk-1.1.0rc1/ahk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ahk-1.0.1/buildunasync.py` & `ahk-1.1.0rc1/buildunasync.py`

 * *Files identical despite different names*

### Comparing `ahk-1.0.1/docs/README.md` & `ahk-1.1.0rc1/docs/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -318,14 +318,36 @@
 from ahk.directives import NoTrayIcon
 
 ahk = AHK(directives=[NoTrayIcon])
 ```
 
 By default, some directives are automatically added to ensure functionality and are merged with any user-provided directives.
 
+## Menu tray icon
+
+As discussed above, you can hide the tray icon if you wish. Additionally, there are some methods available for
+customizing the tray icon.
+
+
+```python
+from ahk import AHK
+ahk = AHK()
+
+# change the tray icon (in this case, using a builtin system icon)
+ahk.menu_tray_icon('Shell32.dll', 174)
+# revert it back to the original:
+ahk.menu_tray_icon()
+
+# change the tooltip that shows up when hovering the mouse over the tray icon
+ahk.menu_tray_tooltip('My Program Name')
+
+# Show the tray icon that was previously hidden by ``NoTrayIcon``
+ahk.menu_tray_icon_show()
+```
+
 ## Registry methods
 
 You can read/write/delete registry keys:
 
 ```python
 from ahk import AHK
 ahk = AHK()
```

### Comparing `ahk-1.0.1/setup.cfg` & `ahk-1.1.0rc1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ahk
-version = 1.0.1
+version = 1.1.0rc1
 author_email = spencer.young@spyoung.com
 author = Spencer Young
 description = A Python wrapper for AHK
 long_description = file: docs/README.md
 long_description_content_type = text/markdown
 url = https://github.com/spyoungtech/ahk
 keywords =
```

