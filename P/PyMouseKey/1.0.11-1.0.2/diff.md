# Comparing `tmp/PyMouseKey-1.0.11.tar.gz` & `tmp/PyMouseKey-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyMouseKey-1.0.11.tar", last modified: Wed May  3 22:48:35 2023, max compression
+gzip compressed data, was "PyMouseKey-1.0.2.tar", last modified: Thu May  4 00:46:14 2023, max compression
```

## Comparing `PyMouseKey-1.0.11.tar` & `PyMouseKey-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 22:48:35.742239 PyMouseKey-1.0.11/
--rw-rw-rw-   0        0        0      376 2023-05-03 22:48:35.736951 PyMouseKey-1.0.11/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-03 22:48:35.731488 PyMouseKey-1.0.11/PyMouseKey.egg-info/
--rw-rw-rw-   0        0        0      376 2023-05-03 22:48:35.000000 PyMouseKey-1.0.11/PyMouseKey.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2023-05-03 22:48:35.000000 PyMouseKey-1.0.11/PyMouseKey.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 22:48:35.000000 PyMouseKey-1.0.11/PyMouseKey.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-03 22:48:35.000000 PyMouseKey-1.0.11/PyMouseKey.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-03 22:48:35.732978 PyMouseKey-1.0.11/pymousekey/
--rw-rw-rw-   0        0        0    17226 2023-05-03 22:37:50.000000 PyMouseKey-1.0.11/pymousekey/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-03 22:48:35.742239 PyMouseKey-1.0.11/setup.cfg
--rw-rw-rw-   0        0        0      544 2023-05-03 22:47:41.000000 PyMouseKey-1.0.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 00:46:14.208606 PyMouseKey-1.0.2/
+-rw-rw-rw-   0        0        0      434 2023-05-04 00:46:14.202652 PyMouseKey-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-04 00:46:14.196206 PyMouseKey-1.0.2/PyMouseKey.egg-info/
+-rw-rw-rw-   0        0        0      434 2023-05-04 00:46:14.000000 PyMouseKey-1.0.2/PyMouseKey.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2023-05-04 00:46:14.000000 PyMouseKey-1.0.2/PyMouseKey.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 00:46:14.000000 PyMouseKey-1.0.2/PyMouseKey.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-04 00:46:14.000000 PyMouseKey-1.0.2/PyMouseKey.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 00:46:14.198190 PyMouseKey-1.0.2/pymousekey/
+-rw-rw-rw-   0        0        0    17498 2023-05-04 00:44:56.000000 PyMouseKey-1.0.2/pymousekey/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-04 00:46:14.208606 PyMouseKey-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      602 2023-05-04 00:29:46.000000 PyMouseKey-1.0.2/setup.py
```

### Comparing `PyMouseKey-1.0.11/pymousekey/__init__.py` & `PyMouseKey-1.0.2/pymousekey/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -317,14 +317,15 @@
                 ("mi", MouseInput),
                 ("hi", HardwareInput)]
 
 class Input(ctypes.Structure):
     _fields_ = [("type", ctypes.c_ulong),
                 ("ii", Input_I)]
 
+
 def getPos():
     cursor = POINT()
     ctypes.windll.user32.GetCursorPos(ctypes.byref(cursor))
     return cursor.x, cursor.y
 
 
 def dragTo(x=None, y=None, duration=0.0, _pause=True):
@@ -332,16 +333,14 @@
     Performs a drag (mouse movement with mouse button down) to coordinates on screen\n
     
     x,y(int): are the coordinates your going to drag to from your current cursor position\n
     
     Duration(int/float): is the time inbetween each mouse movement towards the new x & y coordinates, if 0 it moves instantly
     """
 
-    # cursor = POINT()
-    # ctypes.windll.user32.GetCursorPos(ctypes.byref(cursor))
     start_x, start_y = getPos()
     duration = duration / 100
 
     distance = math.hypot(x - start_x, y - start_y)
 
     ii_ = Input_I()
     ii_.mi = MouseInput(0, 0, 0, MOUSEEVENTF_LEFTDOWN, 0, ctypes.pointer(ctypes.c_ulong(0)))
@@ -366,32 +365,33 @@
     if _pause:
         time.sleep(PAUSE)
 
 
 def moveTo(x=None, y=None, _pause=True):
     """
     Moves the mouse to the specified x and y coordinates\n
-    x,y(int): are the coordinates your going to move to\n
+    x,y(int): x,y(int): The coordinates your going to move to\n
     _pause is the sleep after every keypress _pause=False to disable the pause
     
     """
     ii_ = Input_I()
     ii_.mi = MouseInput(int(65535 * x / screen_width), int(65535 * y / screen_height), 0, MOUSEEVENTF_MOVE | MOUSEEVENTF_ABSOLUTE, 0, ctypes.pointer(ctypes.c_ulong(0)))
     xx = Input(ctypes.c_ulong(0), ii_)
     ctypes.windll.user32.SendInput(1, ctypes.pointer(xx), ctypes.sizeof(xx))
     if _pause:
         time.sleep(PAUSE)
 
+
 def click(x=None, y=None, interval=0.0, clicks=1, button=LEFT, _pause=True):
     """
     Performs a mouse click at the specified x and y coordinates\n
     If no x and y coordinates are specified perform a mouse click at your mouse location\n
-    x,y(int): are the coordinates your going to move to\n
+    x,y(int): The coordinates your going to move to\n
     interval(float): The sleep after the mouse key has been pressed so you can set your own intervals per call\n
-    clicks(int): the amount of clicks you want to perform
+    clicks(int): The amount of clicks you want to perform
 
     """
     if x and y:
         moveTo(x,y)
 
     if button == LEFT:
         event = MOUSEEVENTF_LEFTCLICK
@@ -409,14 +409,15 @@
         xx = Input(ctypes.c_ulong(0), ii_)
         ctypes.windll.user32.SendInput(1, ctypes.pointer(xx), ctypes.sizeof(xx))
         time.sleep(interval)
 
     if _pause:
         time.sleep(PAUSE)
 
+
 def doubleClick(x=None, y=None, interval=0.0, button=LEFT, _pause=True):
     click(x, y, interval, 2, button, _pause)
 
 def tripleClick(x=None, y=None, interval=0.0, button=LEFT, _pause=True):
     click(x, y, interval, 3, button, _pause)
 
 
@@ -433,18 +434,18 @@
     ii_.mi = MouseInput(0,0, scrollAmount*120, MOUSEEVENTF_WHEEL, 0, ctypes.pointer(ctypes.c_ulong(0)))
     xx = Input(ctypes.c_ulong(0), ii_)
     ctypes.windll.user32.SendInput(1, ctypes.pointer(xx), ctypes.sizeof(xx))
 
 
 def press(key, interval=0.0, _pause=True):
     """
-    Performs a keypress or side mouse button press\n
-    Key(string)\n
+    Performs a keypress, also supports side mouse buttons (xbutton1 and xbutton2)\n
+    Key(string): The key/mouse button expected to be pressed\n
     interval(float): The sleep after the key has been pressed so you can set your own intervals per call\n
-    mouse_functions.KEYS for the dict of keys
+    pymousekey.KEYS for the dict of keys
 
     """
     if not key.lower() in KEYS or KEYS[key.lower()] is None:
         return
     ii_ = Input_I()
     
     if key == ('xbutton1' or 'xbutton2'):
@@ -454,35 +455,50 @@
         return
     
     if str(key).isupper():
         ii_.ki = KeyBdInput(0, KEYS['shift'], KEYEVENTF_SCANCODE, 0, ctypes.pointer(ctypes.c_ulong(0)))
         x = Input(ctypes.c_ulong(1), ii_)
         ctypes.windll.user32.SendInput(1, ctypes.pointer(x), ctypes.sizeof(x))
     
-    ii_.ki = KeyBdInput(0, KEYS[str(key).lower()], KEYEVENTF_SCANCODE, 0, ctypes.pointer(ctypes.c_ulong(0)))
-    x = Input(ctypes.c_ulong(1), ii_)
-    ctypes.windll.user32.SendInput(1, ctypes.pointer(x), ctypes.sizeof(x))
-
-    ii_.ki = KeyBdInput(0, KEYS[str(key).lower()], KEYEVENTF_SCANCODE | KEYEVENTF_KEYUP, 0, ctypes.pointer(ctypes.c_ulong(0)))
-    x = Input(ctypes.c_ulong(1), ii_)
-    ctypes.windll.user32.SendInput(1, ctypes.pointer(x), ctypes.sizeof(x))
+    keyDown(key.lower())
+    keyUp(key.lower())
     
     if str(key).isupper():
         ii_.ki = KeyBdInput(0, KEYS['shift'], KEYEVENTF_SCANCODE | KEYEVENTF_KEYUP, 0, ctypes.pointer(ctypes.c_ulong(0)))
         x = Input(ctypes.c_ulong(1), ii_)
         ctypes.windll.user32.SendInput(1, ctypes.pointer(x), ctypes.sizeof(x))
     
     time.sleep(interval)
     if _pause:
         time.sleep(PAUSE)
 
 
+def keyDown(key):
+    if not key.lower() in KEYS or KEYS[key.lower()] is None:
+        return
+
+    ii_ = Input_I()
+    ii_.ki = KeyBdInput(0, KEYS[key], KEYEVENTF_SCANCODE, 0, ctypes.pointer(ctypes.c_ulong(0)))
+    x = Input(ctypes.c_ulong(1), ii_)
+    ctypes.windll.user32.SendInput(1, ctypes.pointer(x), ctypes.sizeof(x))
+
+
+def keyUp(key):
+    if not key.lower() in KEYS or KEYS[key.lower()] is None:
+        return
+
+    ii_ = Input_I()
+    ii_.ki = KeyBdInput(0, KEYS[key], KEYEVENTF_SCANCODE | KEYEVENTF_KEYUP, 0, ctypes.pointer(ctypes.c_ulong(0)))
+    x = Input(ctypes.c_ulong(1), ii_)
+    ctypes.windll.user32.SendInput(1, ctypes.pointer(x), ctypes.sizeof(x))
+
+
 def typeWrite(message, interval=0.0, _pause=True):
     """
-    Types out a given message, letters can me lowercase or uppercase\n
+    Types out a given message, letters suppors lowercase and uppercase letters\n
     message(str): The message you want typed out\n
     interval(float): The sleep after the key has been pressed so you can set your own intervals per call\n
     _pause(bool): The sleep inbetween each keypress, True for pauses False for no pauses
 
     """
     for i in message:
         if i.isupper():
@@ -491,60 +507,61 @@
             press(i, interval, _pause)
         elif i == ' ':
             press(i, interval, _pause)
 
 
 def getPixelColor(x=None, y=None):
     """
-    Gets the color from the specified x and y coordinates, if no x and y are specified it gets the hex color of the coordinates under your mouse\n
+    Gets the color from the specified x and y coordinates, if no coordinates are specified grab the color at your mouse coordinates\n
+    Returns:
+    ----
+    hexColor & rgbColor
     
-    Returns the hex value and rgb value of the specified pixel
-
     """
     dc = ctypes.windll.user32.GetDC(None)
     if not (x and y):
         x,y = getPos()
-        # cursor = POINT()
-        # ctypes.windll.user32.GetCursorPos(ctypes.byref(cursor))
         color = ctypes.windll.gdi32.GetPixel(dc, x, y)
     else:
         color = ctypes.windll.gdi32.GetPixel(dc, x, y)
 
     red = color & 0xff
     green = (color >> 8) & 0xff
     blue = (color >> 16) & 0xff
     ctypes.windll.user32.ReleaseDC(None,dc)
     hexColor = '#{:02x}{:02x}{:02x}'.format(red,green,blue)
-    rgb = red, green, blue
-    return hexColor, rgb
+    rgbColor = red, green, blue
+    return hexColor, rgbColor
 
 
 def controlSend(key=None, className=None, windowTitle=None, lparam=None):
     """
     Sends software keyboard inputs to any inactive window/control by sending the WM_ACTIVATE msg and WA_ACTIVE wParam then sending the WH_CHAR message with the key you specified\n
-    key(string)\n
+    key(string): The key is being sent using ord() so only 1 length strings are allowed such as "a" or ";"\n
+    
     Note:
     -------
     Some games/windows only take the hardware inputs as an option so if you dont see any results this is why
 
     """
     handle = ctypes.windll.user32.FindWindowW(className, windowTitle)
 
-    # Might need to give a lparam other than zero depending on the circumstances
+    # Might need to give a lparam other than zero depending on the circumstances (im unsure)
     ctypes.windll.user32.PostMessageW(handle, WM_ACTIVATE, WA_ACTIVE, 0)
     ctypes.windll.user32.PostMessageW(handle, WM_CHAR, ord(key), lparam)
 
 
 def controlClick(x=None, y=None, className=None, windowTitle=None, button='left'):
     """
     Sends software mouse inputs to any inactive window/control by sending the WM_ACTIVATE msg and WA_ACTIVE wParam then sending WM_LBUTTONDOWN and WM_LBUTTONUP messages\n
+    
     Note:
     -------
     Some games/windows only take the hardware inputs as an option\n
-    In addition to this some games Example: BloonsTD6 dont care that you gave the x and y coordinates and instead will send the mouse event to wherever your current mouse location is
+    In addition to this some games Example: BloonsTD6 dont care that you gave the x and y coordinates and instead sends the mouse event to wherever your current mouse location is
 
     """
 
     handle = ctypes.windll.user32.FindWindowW(className, windowTitle)
     lparam = ctypes.c_long((y << 16) | (x & 0xFFFF)).value
 
     ctypes.windll.user32.PostMessageW(handle, WM_ACTIVATE, WA_ACTIVE, 0)
@@ -558,8 +575,10 @@
         ctypes.windll.user32.PostMessageW(handle, WM_NCHITTEST, 0, lparam)
         ctypes.windll.user32.PostMessageW(handle, WM_RBUTTONDOWN, MK_RBUTTON, lparam)
         ctypes.windll.user32.PostMessageW(handle, WM_RBUTTONUP, MK_RBUTTON, lparam)
 
     elif button == 'middle':
         ctypes.windll.user32.PostMessageW(handle, WM_NCHITTEST, 0, lparam)
         ctypes.windll.user32.PostMessageW(handle, WM_MBUTTONDOWN, MK_MBUTTON, lparam)
-        ctypes.windll.user32.PostMessageW(handle, WM_MBUTTONUP, MK_MBUTTON, lparam)
+        ctypes.windll.user32.PostMessageW(handle, WM_MBUTTONUP, MK_MBUTTON, lparam)
+
+
```

