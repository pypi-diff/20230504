# Comparing `tmp/PySide6_Customized_Window-1.2-py3-none-any.whl.zip` & `tmp/PySide6_Customized_Window-1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 10242 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat    45000 b- defN 23-May-01 13:20 PySide6_Customized_Window.py
--rw-rw-rw-  2.0 fat       10 b- defN 23-May-01 13:48 PySide6_Customized_Window-1.2.dist-info/DESCRIPTION.rst
--rw-rw-rw-  2.0 fat      619 b- defN 23-May-01 13:48 PySide6_Customized_Window-1.2.dist-info/metadata.json
--rw-rw-rw-  2.0 fat        1 b- defN 23-May-01 13:48 PySide6_Customized_Window-1.2.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat       97 b- defN 23-May-01 13:48 PySide6_Customized_Window-1.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat      486 b- defN 23-May-01 13:48 PySide6_Customized_Window-1.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat      672 b- defN 23-May-01 13:48 PySide6_Customized_Window-1.2.dist-info/RECORD
-7 files, 46885 bytes uncompressed, 9032 bytes compressed:  80.7%
+Zip file size: 10713 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat    48100 b- defN 23-May-04 15:07 PySide6_Customized_Window.py
+-rw-rw-rw-  2.0 fat       10 b- defN 23-May-04 15:13 PySide6_Customized_Window-1.3.dist-info/DESCRIPTION.rst
+-rw-rw-rw-  2.0 fat      619 b- defN 23-May-04 15:13 PySide6_Customized_Window-1.3.dist-info/metadata.json
+-rw-rw-rw-  2.0 fat        1 b- defN 23-May-04 15:13 PySide6_Customized_Window-1.3.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat       97 b- defN 23-May-04 15:13 PySide6_Customized_Window-1.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat      486 b- defN 23-May-04 15:13 PySide6_Customized_Window-1.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      672 b- defN 23-May-04 15:13 PySide6_Customized_Window-1.3.dist-info/RECORD
+7 files, 49985 bytes uncompressed, 9503 bytes compressed:  81.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: PySide6_Customized_Window.py
 Comment: 
 
-Filename: PySide6_Customized_Window-1.2.dist-info/DESCRIPTION.rst
+Filename: PySide6_Customized_Window-1.3.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: PySide6_Customized_Window-1.2.dist-info/metadata.json
+Filename: PySide6_Customized_Window-1.3.dist-info/metadata.json
 Comment: 
 
-Filename: PySide6_Customized_Window-1.2.dist-info/top_level.txt
+Filename: PySide6_Customized_Window-1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: PySide6_Customized_Window-1.2.dist-info/WHEEL
+Filename: PySide6_Customized_Window-1.3.dist-info/WHEEL
 Comment: 
 
-Filename: PySide6_Customized_Window-1.2.dist-info/METADATA
+Filename: PySide6_Customized_Window-1.3.dist-info/METADATA
 Comment: 
 
-Filename: PySide6_Customized_Window-1.2.dist-info/RECORD
+Filename: PySide6_Customized_Window-1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## PySide6_Customized_Window.py

```diff
@@ -171,26 +171,55 @@
     try:
         dpi_x = ctypes.c_uint()
         dpi_y = ctypes.c_uint()
         monitor_handle = ctypes.windll.user32.MonitorFromWindow(hwnd, 2)
         ctypes.windll.shcore.GetDpiForMonitor(monitor_handle, 0, ctypes.byref(dpi_x), ctypes.byref(dpi_y))
         dpi = dpi_x.value
     except:
-        try:
+        if hasattr(ctypes.windll.user32, 'IsProcessDPIAware'):
             if ctypes.windll.user32.IsProcessDPIAware():
                 hDC = ctypes.windll.user32.GetDC(None)
                 dpi = ctypes.windll.gdi32.GetDeviceCaps(hDC, 88)
                 ctypes.windll.user32.ReleaseDC(None, hDC)
             else:
                 dpi = 96
-        except:
+        else:
             dpi = 96
     return dpi
 
 
+def getautohidetaskbarposition():
+    SPI_GETWORKAREA = 0x30
+    primaryscreenrect = RECT()
+    primaryscreenwidth = ctypes.windll.user32.GetSystemMetrics(0)
+    primaryscreenheight = ctypes.windll.user32.GetSystemMetrics(1)
+    primaryscreenrect.left = 0
+    primaryscreenrect.top = 0
+    primaryscreenrect.right = primaryscreenwidth
+    primaryscreenrect.bottom = primaryscreenheight
+    if primaryscreenwidth != primaryscreenrect.right - primaryscreenrect.left or primaryscreenheight != primaryscreenrect.bottom - primaryscreenrect.top:
+        return 4
+    taskbar_hwnd = ctypes.windll.user32.FindWindowA(b'Shell_TrayWnd', None)
+    if not taskbar_hwnd:
+        return 4
+    taskbar_rect = RECT()
+    ctypes.windll.user32.GetWindowRect(taskbar_hwnd, ctypes.byref(taskbar_rect))
+    if taskbar_rect.left < primaryscreenrect.left and taskbar_rect.top == primaryscreenrect.top and taskbar_rect.right != primaryscreenrect.right and taskbar_rect.bottom == primaryscreenrect.bottom:
+        return 0
+    elif taskbar_rect.left == primaryscreenrect.left and taskbar_rect.top < primaryscreenrect.top and taskbar_rect.right == primaryscreenrect.right and taskbar_rect.bottom != primaryscreenrect.bottom:
+        return 1
+    elif taskbar_rect.left != primaryscreenrect.left and taskbar_rect.top == primaryscreenrect.top and taskbar_rect.right > primaryscreenrect.right and taskbar_rect.bottom == primaryscreenrect.bottom:
+        return 2
+    elif taskbar_rect.left == primaryscreenrect.left and taskbar_rect.top != primaryscreenrect.top and taskbar_rect.right == primaryscreenrect.right and taskbar_rect.bottom > primaryscreenrect.bottom:
+        return 3
+    else:
+        return 4
+    
+
+
 def getcaptionfont():
     result = NONCLIENTMETRICS()
     result.cbSize = ctypes.sizeof(NONCLIENTMETRICS)
     ctypes.windll.user32.SystemParametersInfoW(0x29, ctypes.sizeof(NONCLIENTMETRICS), ctypes.pointer(result), 0)
     captionfont = result.lfCaptionFont.lfFaceName
     return captionfont
 
@@ -208,22 +237,22 @@
         self.animation2.setDuration(250)
         self.animation2.setStartValue(1.0)
         self.animation2.setEndValue(0.0)
         self.nonclientareasizeinited = False
         self.isblurwindow = isinstance(self, BlurWindow)
         WNDPROC = ctypes.WINFUNCTYPE(ctypes.c_long, ctypes.c_int, ctypes.c_uint, ctypes.c_int, ctypes.c_int)
         BasicMessageHandlerAddress = ctypes.cast(WNDPROC(self.BasicMessageHandler), ctypes.c_void_p).value
-        try:
+        if hasattr(ctypes.windll.user32, 'GetWindowLongPtrW'):
             self.originalBasicMessageHandler = ctypes.windll.user32.GetWindowLongPtrW(self.hwnd, -4)
-        except:
+        else:
             self.originalBasicMessageHandler = ctypes.windll.user32.GetWindowLongW(self.hwnd, -4)
         if ISPYSIDE1:
-            try:
+            if hasattr(ctypes.windll.user32, 'SetWindowLongPtrW'):
                 ctypes.windll.user32.SetWindowLongPtrW(self.hwnd, -4, ctypes.c_int64(BasicMessageHandlerAddress))
-            except:
+            else:
                 ctypes.windll.user32.SetWindowLongW(self.hwnd, -4, BasicMessageHandlerAddress)
         self.setAttribute(Qt.WA_TranslucentBackground, True)
         self.hwnd = gethwnd(self)
         if ISPYSIDE1:
             ctypes.windll.user32.SetWindowLongW(self.hwnd, -16, 0x40000 | 0x20000 | 0x10000)
         else:
             ctypes.windll.user32.SetWindowLongW(self.hwnd, -16, 0xc00000 | 0x40000 | 0x20000 | 0x10000)
@@ -236,22 +265,30 @@
         self.realdpi = getdpiforwindow_winapi(self.hwnd)
         self.highdpiscalingenabled = False
         self.highdpiscalefactorroundingpolicy = 3
         if hasattr(Qt, 'AA_EnableHighDpiScaling'):
             if QApplication.testAttribute(Qt.AA_EnableHighDpiScaling):
                 self.highdpiscalingenabled = True
         if hasattr(Qt, 'HighDpiScaleFactorRoundingPolicy'):
-            self.highdpiscalefactorroundingpolicy = 4
+            policy_dict = {Qt.HighDpiScaleFactorRoundingPolicy.Ceil: 1, Qt.HighDpiScaleFactorRoundingPolicy.Floor: 2, Qt.HighDpiScaleFactorRoundingPolicy.PassThrough: 3, Qt.HighDpiScaleFactorRoundingPolicy.Round: 4, Qt.HighDpiScaleFactorRoundingPolicy.RoundPreferFloor: 5}
+            if hasattr(Qt.HighDpiScaleFactorRoundingPolicy, 'Unset'):
+                if QApplication.highDpiScaleFactorRoundingPolicy() == Qt.HighDpiScaleFactorRoundingPolicy.Unset:
+                    self.highdpiscalefactorroundingpolicy = 3
+                else:
+                    self.highdpiscalefactorroundingpolicy = policy_dict[QApplication.highDpiScaleFactorRoundingPolicy()]
+            else:
+                self.highdpiscalefactorroundingpolicy = policy_dict[QApplication.highDpiScaleFactorRoundingPolicy()]
         self.dpi = self.getdpibyrealdpi(self.realdpi)
         dpi = self.dpi
         self.maximizedwindowborderwidth_list = self.getMaximizedWindowBorderWidth()
         self.themecolour = 0
         self.isdarktheme = isdarktheme()
         self.setMinimumSize(int(220.0 * dpi / 96.0), int(48.0 * dpi / 96.0))
         self.updateconstantsfordpi()
+        self.updateautohidetaskbarwidth()
         self.inminsizebutton = False
         self.inmaxsizebutton = False
         self.inclosebutton = False
         self.intitlebar = False
         self.intopborder = False
         self.inleftborder = False
         self.inbottomborder = False
@@ -319,32 +356,14 @@
             self.isdarktheme = isdarktheme()
         elif themecolour == 1:
             self.isdarktheme = False
         elif themecolour == 2:
             self.isdarktheme = True
         else:
             raise Exception
-    def setHighDpiScaleFactorRoundingPolicy(self, policy):
-        '''policy=Qt.HighDpiScaleFactorRoundingPolicy.Ceil
-policy=Qt.HighDpiScaleFactorRoundingPolicy.Floor
-policy=Qt.HighDpiScaleFactorRoundingPolicy.PassThrough
-policy=Qt.HighDpiScaleFactorRoundingPolicy.Round
-policy=Qt.HighDpiScaleFactorRoundingPolicy.RoundPreferFloor'''
-        try:
-            policy_dict = {Qt.HighDpiScaleFactorRoundingPolicy.Ceil: 1, Qt.HighDpiScaleFactorRoundingPolicy.Floor: 2, Qt.HighDpiScaleFactorRoundingPolicy.PassThrough: 3, Qt.HighDpiScaleFactorRoundingPolicy.Round: 4, Qt.HighDpiScaleFactorRoundingPolicy.RoundPreferFloor: 5}
-        except:
-            raise Exception('setHighDpiScaleFactorRoundingPolicy is only avaliable on PySideX 5.14 and newer.')
-        try:
-            self.highdpiscalefactorroundingpolicy = policy_dict[policy]
-        except:
-            raise ValueError('Argument policy must be Qt.HighDpiScaleFactorRoundingPolicy.Ceil, Qt.HighDpiScaleFactorRoundingPolicy.Floor, Qt.HighDpiScaleFactorRoundingPolicy.PassThrough, Qt.HighDpiScaleFactorRoundingPolicy.Round or Qt.HighDpiScaleFactorRoundingPolicy.RoundPreferFloor.')
-        dpi = self.getdpibyrealdpi(self.realdpi)
-        self.dpi = dpi
-        self.setMinimumSize(int(220.0 * dpi / 96.0), int(48.0 * dpi / 96.0))
-        self.updateconstantsfordpi()
     def setWindowTitle2(self, arg__1):
         self.originalSetWindowTitle(arg__1)
         self.paintTitleBarAndClientArea(self.isActiveWindow())
     def setWindowIcon2(self, icon):
         self.originalSetWindowIcon(icon)
         self.paintTitleBarAndClientArea(self.isActiveWindow())
     def paintTitleBarAndClientArea(self, isactivewindow=0, ismaximized=-1):
@@ -547,14 +566,15 @@
         pass
     def BasicMessageHandler(self, hwnd, message, wParam, lParam):
         '''For PySide1/2/6, you should define MessageHandler instead of BasicMessageHandler.'''
         WM_ACTIVATE = 0x6
         WM_SHOWWINDOW = 0x18
         WM_SETTINGCHANGE = 0x1a
         WM_GETMINMAXINFO = 0x24
+        WM_WINDOWPOSCHANGED = 0x47
         WM_NCCALCSIZE = 0x83
         WM_NCHITTEST = 0x84
         WM_NCLBUTTONDOWN = 0xa1
         WM_NCLBUTTONUP = 0xa2
         WM_LBUTTONUP = 0x2a2
         WM_DPICHANGED = 0x2e0
         WM_SYSCOMMAND = 0x112
@@ -575,15 +595,20 @@
         HTRIGHT = 0xb
         HTTOP = 0xc
         HTTOPLEFT = 0xd
         HTTOPRIGHT = 0xe
         HTBOTTOM = 0xf
         HTBOTTOMLEFT = 0x10
         HTBOTTOMRIGHT = 0x11
-        WVR_REDRAW = 0x300
+        SWP_NOSIZE = 0x1
+        SWP_NOMOVE = 0x2
+        SWP_NOZORDER = 0x4
+        SWP_FRAMECHANGED = 0x20
+        SPI_SETNONCLIENTMETRICS = 0x2a
+        SPI_SETWORKAREA = 0x2f
         try:
             dpi = self.dpi
             realdpi = self.realdpi
             real_border_width = self.real_border_width
             real_title_height = self.real_title_height
             real_menubutton_width = self.real_menubutton_width
             windowmargin_left = self.windowmargin_left
@@ -632,16 +657,15 @@
         self.inclosebutton = inclosebutton
         self.intitlebar = intitlebar
         self.intopborder = intopborder
         self.inleftborder = inleftborder
         self.inbottomborder = inbottomborder
         self.inrightborder = inrightborder
         if message == WM_NCCALCSIZE:
-            if ISPYSIDE1:
-                return self.Handle_WM_NCCALCSIZE_Message(hwnd, message, wParam, lParam)
+            return self.Handle_WM_NCCALCSIZE_Message(hwnd, message, wParam, lParam)
         if message == WM_NCHITTEST:
             VK_LBUTTON = 0x1
             isleftbuttonpressed = ctypes.windll.user32.GetKeyState(VK_LBUTTON) not in [0, 1]
             if not self.isMaximized():
                 if intopborder and inleftborder:
                     WM_NCHITTEST_result = HTTOPLEFT
                 elif intopborder and inrightborder:
@@ -713,19 +737,27 @@
                 self.setGeometry(x, y, width, height)
             dpi = self.getdpibyrealdpi(realdpi)
             self.dpi = dpi
             self.setMinimumSize(int(220.0 * dpi / 96.0), int(48.0 * dpi / 96.0))
             self.updateconstantsfordpi()
             self.paintTitleBarAndClientArea(self.isActiveWindow())
         if message == WM_SETTINGCHANGE:
-            if self.themecolour == 0 and str(ctypes.cast(lParam, ctypes.c_wchar_p).value) == 'ImmersiveColorSet':
+            try:
+                lParam_string = str(ctypes.cast(lParam, ctypes.c_wchar_p).value)
+            except:
+                lParam_string = ''
+            if wParam == SPI_SETWORKAREA:
+                self.updateautohidetaskbarwidth()
+                ctypes.windll.user32.SetWindowPos(hwnd, None, 0, 0, 0, 0, SWP_NOSIZE | SWP_NOMOVE | SWP_NOZORDER | SWP_FRAMECHANGED)
+            if wParam == SPI_SETNONCLIENTMETRICS:
+                self.maximizedwindowborderwidth_list = self.getMaximizedWindowBorderWidth()
+                self.captionfont = getcaptionfont()
+            if self.themecolour == 0 and lParam_string == 'ImmersiveColorSet':
                 self.isdarktheme = isdarktheme()
                 self.paintTitleBarAndClientArea(self.isActiveWindow())
-            if str(ctypes.cast(lParam, ctypes.c_wchar_p).value) == 'WindowMetrics':
-                self.captionfont = getcaptionfont()
         if message == WM_DWMCOMPOSITIONCHANGED:
             self.isaeroenabled = isAeroEnabled()
             if self.isaeroenabled:
                 if self.isblurwindow:
                     self.setBlurEffect()
                 else:
                     self.setDWMShadowEffect()
@@ -741,34 +773,49 @@
         if messagehandlerresult != None:
             return messagehandlerresult
         if ISPYSIDE1:
             return ctypes.windll.user32.CallWindowProcW(self.originalBasicMessageHandler, hwnd, message, wParam, lParam)
     def Handle_WM_NCCALCSIZE_Message(self, hwnd, message, wParam, lParam):
         try:
             nonclientareasizeinited = self.nonclientareasizeinited
+            leftautohidetaskbarwidth = self.leftautohidetaskbarwidth
+            topautohidetaskbarwidth = self.topautohidetaskbarwidth
+            rightautohidetaskbarwidth = self.rightautohidetaskbarwidth
+            bottomautohidetaskbarwidth = self.bottomautohidetaskbarwidth
         except:
             nonclientareasizeinited = False
+            leftautohidetaskbarwidth = 0
+            topautohidetaskbarwidth = 0
+            rightautohidetaskbarwidth = 0
+            bottomautohidetaskbarwidth = 0
         if not nonclientareasizeinited:
             if ISPYSIDE1:
-                ctypes.windll.user32.SetWindowLongW(self.hwnd, -16, ctypes.windll.user32.GetWindowLongW(self.hwnd, -16) | 0xc00000)
+                if hasattr(ctypes.windll.user32, 'GetWindowLongPtrW'):
+                    originalwindowlong = ctypes.windll.user32.GetWindowLongPtrW(self.hwnd, -16)
+                else:
+                    originalwindowlong = ctypes.windll.user32.GetWindowLongW(self.hwnd, -16)
+                if hasattr(ctypes.windll.user32, 'SetWindowLongPtrW'):
+                    ctypes.windll.user32.SetWindowLongPtrW(self.hwnd, -16, originalwindowlong | 0xc00000)
+                else:
+                    ctypes.windll.user32.SetWindowLongW(self.hwnd, -16, originalwindowlong | 0xc00000)
             self.nonclientareasizeinited = True
         if wParam:
             rect = ctypes.cast(lParam, ctypes.POINTER(NCCALCSIZE_PARAMS)).contents.rgrc[0]
         else:
             rect = ctypes.cast(lParam, ctypes.POINTER(RECT)).contents
         ISMAXIMIZED = ctypes.windll.user32.IsZoomed(hwnd)
         try:
             maximizedwindowborderwidth_list = self.maximizedwindowborderwidth_list
         except:
             maximizedwindowborderwidth_list = [0, 0]
         if ISMAXIMIZED:
-            self.windowmargin_left = maximizedwindowborderwidth_list[0]
-            self.windowmargin_right = maximizedwindowborderwidth_list[0]
-            self.windowmargin_top = maximizedwindowborderwidth_list[1]
-            self.windowmargin_bottom = maximizedwindowborderwidth_list[1]
+            self.windowmargin_left = maximizedwindowborderwidth_list[0] + leftautohidetaskbarwidth
+            self.windowmargin_right = maximizedwindowborderwidth_list[0] + rightautohidetaskbarwidth
+            self.windowmargin_top = maximizedwindowborderwidth_list[1] + topautohidetaskbarwidth
+            self.windowmargin_bottom = maximizedwindowborderwidth_list[1] + bottomautohidetaskbarwidth
         else:
             self.windowmargin_left = 0
             self.windowmargin_right = 0
             self.windowmargin_top = 0
             self.windowmargin_bottom = 0
         windowmargin_left = self.windowmargin_left
         windowmargin_right = self.windowmargin_right
@@ -800,32 +847,29 @@
         SC_CLOSE = 0xf060
         ctypes.windll.user32.SendMessageW(self.hwnd, WM_SYSCOMMAND, SC_CLOSE, 0)
     def getMaximizedWindowBorderWidth(self):
         SM_CXSIZEFRAME = 32
         SM_CYSIZEFRAME = 33
         SM_CXPADDEDBORDER = 92
         realdpi = self.realdpi
-        try:
+        if hasattr(ctypes.windll.user32, 'GetSystemMetricsForDpi'):
             borderwidth_x = ctypes.windll.user32.GetSystemMetricsForDpi(SM_CXSIZEFRAME, realdpi) + ctypes.windll.user32.GetSystemMetricsForDpi(SM_CXPADDEDBORDER, realdpi)
             borderwidth_y = ctypes.windll.user32.GetSystemMetricsForDpi(SM_CYSIZEFRAME, realdpi) + ctypes.windll.user32.GetSystemMetricsForDpi(SM_CXPADDEDBORDER, realdpi)
-        except:
+        else:
             borderwidth_x = ctypes.windll.user32.GetSystemMetrics(SM_CXSIZEFRAME) + ctypes.windll.user32.GetSystemMetrics(SM_CXPADDEDBORDER)
             borderwidth_y = ctypes.windll.user32.GetSystemMetrics(SM_CYSIZEFRAME) + ctypes.windll.user32.GetSystemMetrics(SM_CXPADDEDBORDER)
         return [borderwidth_x, borderwidth_y]
     def nativeEvent(self, eventType, msg):
         '''For PySide2/6, you should define MessageHandler instead of nativeEvent.'''
         WM_NCCALCSIZE = 0x83
         msg = MSG.from_address(msg.__int__())
         hwnd = msg.hWnd
         message = msg.message
         wParam = msg.wParam
         lParam = msg.lParam
-        if message == WM_NCCALCSIZE:
-            if not ISPYSIDE1:
-                return True, self.Handle_WM_NCCALCSIZE_Message(hwnd, message, wParam, lParam)
         basicmessagehandlerresult = self.BasicMessageHandler(hwnd, message, wParam, lParam)
         if basicmessagehandlerresult != None:
             return True, basicmessagehandlerresult
         return super(CustomizedWindow, self).nativeEvent(eventType, msg)
     def setBlurEffect(self):
         hwnd = self.hwnd
         try:
@@ -878,37 +922,43 @@
                     scalefactor = int(realscalefactor + 1)
                 else:
                     scalefactor = int(realscalefactor)
             dpi = int(float(realdpi) / scalefactor)
         else:
             dpi = realdpi
         return dpi
+    def updateconstantsfordpi(self):
+        dpi = self.dpi
+        realdpi = self.realdpi
+        self.border_width = int(5.0 * dpi / 96.0)
+        self.title_height = int(30.0 * dpi / 96.0)
+        self.menubutton_width = int(46.0 * dpi / 96.0)
+        self.title_font_size = int(13.0 * dpi / 96.0)
+        self.real_border_width = int(5.0 * realdpi / 96.0)
+        self.real_title_height = int(30.0 * realdpi / 96.0)
+        self.real_menubutton_width = int(46.0 * realdpi / 96.0)
+        self.titleiconlayout_margin = int(7.0 * dpi / 96.0)
+    def updateautohidetaskbarwidth(self):
+        autohidetaskbarposition = getautohidetaskbarposition()
+        self.leftautohidetaskbarwidth = 2 if autohidetaskbarposition == 0 else 0
+        self.topautohidetaskbarwidth = 2 if autohidetaskbarposition == 1 else 0
+        self.rightautohidetaskbarwidth = 2 if autohidetaskbarposition == 2 else 0
+        self.bottomautohidetaskbarwidth = 2 if autohidetaskbarposition == 3 else 0
     def setwin11blur(self, hWnd):
         Win11_21H2_ENTRY = 1029
         Win11_21H2_VALUE = 1
         Win11_22H2_ENTRY = 38
         Win11_22H2_VALUE = 3
         Win11_21H2_COMMAND = ctypes.windll.dwmapi.DwmSetWindowAttribute(hWnd, Win11_21H2_ENTRY,
                                                                         ctypes.byref(ctypes.c_int(Win11_21H2_VALUE)),
                                                                         ctypes.sizeof(ctypes.c_int))
         Win11_22H2_COMMAND = ctypes.windll.dwmapi.DwmSetWindowAttribute(hWnd, Win11_22H2_ENTRY,
                                                                         ctypes.byref(ctypes.c_int(Win11_22H2_VALUE)),
                                                                         ctypes.sizeof(ctypes.c_int))
         return (Win11_21H2_COMMAND, Win11_22H2_COMMAND)
-    def updateconstantsfordpi(self):
-        dpi = self.dpi
-        realdpi = self.realdpi
-        self.border_width = int(5.0 * dpi / 96.0)
-        self.title_height = int(30.0 * dpi / 96.0)
-        self.menubutton_width = int(46.0 * dpi / 96.0)
-        self.title_font_size = int(13.0 * dpi / 96.0)
-        self.real_border_width = int(5.0 * realdpi / 96.0)
-        self.real_title_height = int(30.0 * realdpi / 96.0)
-        self.real_menubutton_width = int(46.0 * realdpi / 96.0)
-        self.titleiconlayout_margin = int(7.0 * dpi / 96.0)
     def GetWindowRect(self):
         lpRect = RECT()
         ctypes.windll.user32.GetWindowRect(self.hwnd, ctypes.byref(lpRect))
         return lpRect
     def screenChangedHandler(self):
         hwnd = gethwnd(self.windowHandle())
         SWP_NOSIZE = 0x1
@@ -931,15 +981,12 @@
         QApplication.setAttribute(Qt.AA_EnableHighDpiScaling, True)
         QApplication.setAttribute(Qt.AA_UseHighDpiPixmaps, True)
     except: pass
     app = QApplication(sys.argv)
     window = BlurWindow()
     window.setWindowTitle('Window')
     window.setDarkTheme(2)
-    try:
-        window.setHighDpiScaleFactorRoundingPolicy(Qt.HighDpiScaleFactorRoundingPolicy.PassThrough)
-    except: pass
     window.resize(int(400.0 * window.dpi / 96.0), int(175.0 * window.dpi / 96.0))
     window.setWindowIcon(QIcon('Icon.ico'))
     button = QPushButton('Button', window.clientArea)
     window.show()
     app.exec_()
```

## Comparing `PySide6_Customized_Window-1.2.dist-info/metadata.json` & `PySide6_Customized_Window-1.3.dist-info/metadata.json`

 * *Files 18% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'version'": "'1.3'"}*

```diff
@@ -27,9 +27,9 @@
         "GUI",
         "PySide"
     ],
     "metadata_version": "2.0",
     "name": "PySide6-Customized-Window",
     "requires_python": ">=2.6",
     "summary": "A customized window based on PySideX.",
-    "version": "1.2"
+    "version": "1.3"
 }
```

## Comparing `PySide6_Customized_Window-1.2.dist-info/RECORD` & `PySide6_Customized_Window-1.3.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-PySide6_Customized_Window.py,sha256=wYuAM7nkOzQTkCOjH4Mr7LRxXJ32o0OIlWtn9JAbSpo,45000
-PySide6_Customized_Window-1.2.dist-info/DESCRIPTION.rst,sha256=OCTuuN6LcWulhHS3d5rfjdsQtW22n7HENFRh6jC6ego,10
-PySide6_Customized_Window-1.2.dist-info/METADATA,sha256=BMVEN0LigwtpVxdDTzHEiyj_H9-WvcfUIFAxNGI4IjI,486
-PySide6_Customized_Window-1.2.dist-info/RECORD,,
-PySide6_Customized_Window-1.2.dist-info/WHEEL,sha256=Vlaj2XNMTTJ893zWX-JvKeZUIs7q5E7d7Gise2Vouzc,97
-PySide6_Customized_Window-1.2.dist-info/metadata.json,sha256=epGarI3fy-UhIYqUY4LFNNm-Sc0ytkFh1ZzVJ1MXjV8,619
-PySide6_Customized_Window-1.2.dist-info/top_level.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+PySide6_Customized_Window.py,sha256=uxUN1YBkk8yiMtnrygzdkNQ3gnhKPA3tb8lqfzSo2Xo,48100
+PySide6_Customized_Window-1.3.dist-info/DESCRIPTION.rst,sha256=OCTuuN6LcWulhHS3d5rfjdsQtW22n7HENFRh6jC6ego,10
+PySide6_Customized_Window-1.3.dist-info/METADATA,sha256=VMeLR5FnIDEsiB-Z91HfBSjMtfJOlxiWYL-l7Fsal9I,486
+PySide6_Customized_Window-1.3.dist-info/RECORD,,
+PySide6_Customized_Window-1.3.dist-info/WHEEL,sha256=Vlaj2XNMTTJ893zWX-JvKeZUIs7q5E7d7Gise2Vouzc,97
+PySide6_Customized_Window-1.3.dist-info/metadata.json,sha256=5ardBWh6Y1CQhfWmN6IY742DWjiixMQdaf9F2FIZOCI,619
+PySide6_Customized_Window-1.3.dist-info/top_level.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
```

