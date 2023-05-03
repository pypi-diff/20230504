# Comparing `tmp/desktop-notifier-3.5.1.tar.gz` & `tmp/desktop-notifier-3.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "desktop-notifier-3.5.1.tar", last modified: Mon May  1 19:36:45 2023, max compression
+gzip compressed data, was "desktop-notifier-3.5.2.tar", last modified: Wed May  3 22:25:39 2023, max compression
```

## Comparing `desktop-notifier-3.5.1.tar` & `desktop-notifier-3.5.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:36:45.545543 desktop-notifier-3.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-01 19:36:31.000000 desktop-notifier-3.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-05-01 19:36:45.545543 desktop-notifier-3.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7383 2023-05-01 19:36:31.000000 desktop-notifier-3.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-01 19:36:31.000000 desktop-notifier-3.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 19:36:45.545543 desktop-notifier-3.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:36:45.545543 desktop-notifier-3.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:36:45.545543 desktop-notifier-3.5.1/src/desktop_notifier/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-01 19:36:31.000000 desktop-notifier-3.5.1/src/desktop_notifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10614 2023-05-01 19:36:31.000000 desktop-notifier-3.5.1/src/desktop_notifier/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-05-01 19:36:31.000000 desktop-notifier-3.5.1/src/desktop_notifier/dbus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-01 19:36:31.000000 desktop-notifier-3.5.1/src/desktop_notifier/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)    14980 2023-05-01 19:36:31.000000 desktop-notifier-3.5.1/src/desktop_notifier/macos.py
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-05-01 19:36:31.000000 desktop-notifier-3.5.1/src/desktop_notifier/macos_legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-01 19:36:31.000000 desktop-notifier-3.5.1/src/desktop_notifier/macos_support.py
--rw-r--r--   0 runner    (1001) docker     (123)    12931 2023-05-01 19:36:31.000000 desktop-notifier-3.5.1/src/desktop_notifier/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:36:45.545543 desktop-notifier-3.5.1/src/desktop_notifier/resources/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-01 19:36:31.000000 desktop-notifier-3.5.1/src/desktop_notifier/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-05-01 19:36:31.000000 desktop-notifier-3.5.1/src/desktop_notifier/resources/python.png
--rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-05-01 19:36:31.000000 desktop-notifier-3.5.1/src/desktop_notifier/winrt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:36:45.545543 desktop-notifier-3.5.1/src/desktop_notifier.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-05-01 19:36:45.000000 desktop-notifier-3.5.1/src/desktop_notifier.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-01 19:36:45.000000 desktop-notifier-3.5.1/src/desktop_notifier.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 19:36:45.000000 desktop-notifier-3.5.1/src/desktop_notifier.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-01 19:36:45.000000 desktop-notifier-3.5.1/src/desktop_notifier.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 19:36:45.000000 desktop-notifier-3.5.1/src/desktop_notifier.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:25:39.009713 desktop-notifier-3.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-03 22:25:25.000000 desktop-notifier-3.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-05-03 22:25:39.009713 desktop-notifier-3.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7383 2023-05-03 22:25:25.000000 desktop-notifier-3.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-03 22:25:25.000000 desktop-notifier-3.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 22:25:39.009713 desktop-notifier-3.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:25:39.005712 desktop-notifier-3.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:25:39.009713 desktop-notifier-3.5.2/src/desktop_notifier/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-03 22:25:25.000000 desktop-notifier-3.5.2/src/desktop_notifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10614 2023-05-03 22:25:25.000000 desktop-notifier-3.5.2/src/desktop_notifier/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-05-03 22:25:25.000000 desktop-notifier-3.5.2/src/desktop_notifier/dbus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-03 22:25:25.000000 desktop-notifier-3.5.2/src/desktop_notifier/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14980 2023-05-03 22:25:25.000000 desktop-notifier-3.5.2/src/desktop_notifier/macos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-05-03 22:25:25.000000 desktop-notifier-3.5.2/src/desktop_notifier/macos_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-03 22:25:25.000000 desktop-notifier-3.5.2/src/desktop_notifier/macos_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12931 2023-05-03 22:25:25.000000 desktop-notifier-3.5.2/src/desktop_notifier/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:25:39.009713 desktop-notifier-3.5.2/src/desktop_notifier/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-03 22:25:25.000000 desktop-notifier-3.5.2/src/desktop_notifier/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-05-03 22:25:25.000000 desktop-notifier-3.5.2/src/desktop_notifier/resources/python.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9933 2023-05-03 22:25:25.000000 desktop-notifier-3.5.2/src/desktop_notifier/winrt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:25:39.009713 desktop-notifier-3.5.2/src/desktop_notifier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-05-03 22:25:38.000000 desktop-notifier-3.5.2/src/desktop_notifier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-03 22:25:39.000000 desktop-notifier-3.5.2/src/desktop_notifier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 22:25:38.000000 desktop-notifier-3.5.2/src/desktop_notifier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-03 22:25:38.000000 desktop-notifier-3.5.2/src/desktop_notifier.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-03 22:25:38.000000 desktop-notifier-3.5.2/src/desktop_notifier.egg-info/top_level.txt
```

### Comparing `desktop-notifier-3.5.1/LICENSE` & `desktop-notifier-3.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.5.1/PKG-INFO` & `desktop-notifier-3.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: desktop-notifier
-Version: 3.5.1
+Version: 3.5.2
 Summary: Python library for cross-platform desktop notifications
 Author-email: Sam Schott <sam.schott@outlook.com>
 License: MIT
 Project-URL: Homepage, https://github.com/samschott/desktop-notifier
 Keywords: desktop-notifier
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `desktop-notifier-3.5.1/README.md` & `desktop-notifier-3.5.2/README.md`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.5.1/pyproject.toml` & `desktop-notifier-3.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2", "build"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "desktop-notifier"
-version = "3.5.1"
+version = "3.5.2"
 authors = [{name = "Sam Schott", email = "sam.schott@outlook.com"}]
 license = {text = "MIT"}
 description = "Python library for cross-platform desktop notifications"
 keywords = ["desktop-notifier"]
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Developers",
```

### Comparing `desktop-notifier-3.5.1/src/desktop_notifier/base.py` & `desktop-notifier-3.5.2/src/desktop_notifier/base.py`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.5.1/src/desktop_notifier/dbus.py` & `desktop-notifier-3.5.2/src/desktop_notifier/dbus.py`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.5.1/src/desktop_notifier/dummy.py` & `desktop-notifier-3.5.2/src/desktop_notifier/dummy.py`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.5.1/src/desktop_notifier/macos.py` & `desktop-notifier-3.5.2/src/desktop_notifier/macos.py`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.5.1/src/desktop_notifier/macos_legacy.py` & `desktop-notifier-3.5.2/src/desktop_notifier/macos_legacy.py`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.5.1/src/desktop_notifier/macos_support.py` & `desktop-notifier-3.5.2/src/desktop_notifier/macos_support.py`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.5.1/src/desktop_notifier/main.py` & `desktop-notifier-3.5.2/src/desktop_notifier/main.py`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.5.1/src/desktop_notifier/resources/python.png` & `desktop-notifier-3.5.2/src/desktop_notifier/resources/python.png`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.5.1/src/desktop_notifier/winrt.py` & `desktop-notifier-3.5.2/src/desktop_notifier/winrt.py`

 * *Files 8% similar despite different names*

```diff
@@ -63,14 +63,19 @@
 
     _to_native_urgency = {
         Urgency.Low: ToastNotificationPriority.DEFAULT,
         Urgency.Normal: ToastNotificationPriority.DEFAULT,
         Urgency.Critical: ToastNotificationPriority.HIGH,
     }
 
+    DEFAULT_ACTION = "default"
+    REPLY_ACTION = "action=reply&amp"
+    BUTTON_ACTION_PREFIX = "action=button&amp;id="
+    REPLY_TEXTBOX_NAME = "textBox"
+
     def __init__(
         self,
         app_name: str = "Python",
         notification_limit: int | None = None,
     ) -> None:
         super().__init__(app_name, notification_limit)
         self.manager = ToastNotificationManager.get_default()
@@ -105,32 +110,34 @@
     ) -> str:
         """
         Asynchronously sends a notification.
 
         :param notification: Notification to send.
         :param notification_to_replace: Notification to replace, if any.
         """
-        if not self.notifier:
-            raise RuntimeError("Could not get toast notifier")
-
         if notification_to_replace:
             platform_nid = cast(str, notification_to_replace.identifier)
         else:
             platform_nid = str(uuid.uuid4())
 
         # Create notification XML.
-        toast_xml = Element("toast", {"launch": "default"})
+        toast_xml = Element("toast", {"launch": WinRTDesktopNotifier.DEFAULT_ACTION})
         visual_xml = SubElement(toast_xml, "visual")
         actions_xml = SubElement(toast_xml, "actions")
 
         if notification.thread:
             SubElement(
                 toast_xml,
                 "header",
-                {"id": notification.thread, "title": notification.thread},
+                {
+                    "id": notification.thread,
+                    "title": notification.thread,
+                    "arguments": WinRTDesktopNotifier.DEFAULT_ACTION,
+                    "activationType": "background",
+                },
             )
 
         binding = SubElement(visual_xml, "binding", {"template": "ToastGeneric"})
 
         title_xml = SubElement(binding, "text")
         title_xml.text = notification.title
 
@@ -146,38 +153,44 @@
 
         if notification.attachment:
             SubElement(
                 binding, "image", {"placement": "hero", "src": notification.attachment}
             )
 
         if notification.reply_field:
-            SubElement(actions_xml, "input", {"id": "textBox", "type": "text"})
+            SubElement(
+                actions_xml,
+                "input",
+                {"id": WinRTDesktopNotifier.REPLY_TEXTBOX_NAME, "type": "text"},
+            )
             reply_button_xml = SubElement(
                 actions_xml,
                 "action",
                 {
                     "content": notification.reply_field.button_title,
                     "activationType": "background",
                     "arguments": "action=reply&amp",
                 },
             )
 
             # If there are no other buttons, show the
             # reply buttons next to the text field.
             if not notification.buttons:
-                reply_button_xml.set("hint-inputId", "textBox")
+                reply_button_xml.set(
+                    "hint-inputId", WinRTDesktopNotifier.REPLY_TEXTBOX_NAME
+                )
 
         for n, button in enumerate(notification.buttons):
             SubElement(
                 actions_xml,
                 "action",
                 {
                     "content": button.title,
                     "activationType": "background",
-                    "arguments": str(n),
+                    "arguments": WinRTDesktopNotifier.BUTTON_ACTION_PREFIX + str(n),
                 },
             )
 
         if notification.sound:
             SubElement(
                 toast_xml, "audio", {"src": "ms-winsoundevent:Notification.Default"}
             )
@@ -187,35 +200,33 @@
         xml_document = dom.XmlDocument()
         xml_document.load_xml(tostring(toast_xml, encoding="unicode"))
 
         native = ToastNotification(xml_document)
         native.tag = platform_nid
         native.priority = self._to_native_urgency[notification.urgency]
 
-        if notification.thread:
-            native.group = notification.thread
-        else:
-            native.group = "default"
-
         def on_activated(sender, boxed_activated_args) -> None:  # type:ignore
             activated_args = ToastActivatedEventArgs._from(boxed_activated_args)
             action_id = cast(str, activated_args.arguments)
 
-            if action_id == "default":
+            if action_id == WinRTDesktopNotifier.DEFAULT_ACTION:
                 if notification.on_clicked:
                     notification.on_clicked()
-
-            elif action_id == "action=reply&amp":
+            elif action_id == WinRTDesktopNotifier.REPLY_ACTION:
                 if notification.reply_field and notification.reply_field.on_replied:
-                    boxed_text = activated_args.user_input["textBox"]
+                    boxed_text = activated_args.user_input[
+                        WinRTDesktopNotifier.REPLY_TEXTBOX_NAME
+                    ]
                     text = unbox_winrt(boxed_text)
                     notification.reply_field.on_replied(text)
-
-            elif action_id.isnumeric():
-                action_number = int(action_id)
+            elif action_id.startswith(WinRTDesktopNotifier.BUTTON_ACTION_PREFIX):
+                action_number_str = action_id.replace(
+                    WinRTDesktopNotifier.BUTTON_ACTION_PREFIX, ""
+                )
+                action_number = int(action_number_str)
                 callback = notification.buttons[action_number].on_pressed
                 if callback:
                     callback()
 
         def on_dismissed(sender, dismissed_args) -> None:  # type:ignore
             self._clear_notification_from_cache(notification)
 
@@ -233,19 +244,18 @@
         native.add_failed(on_failed)
 
         self.notifier.show(native)
 
         return platform_nid
 
     async def _clear(self, notification: Notification) -> None:
-        """c
+        """
         Asynchronously removes a notification from the notification center.
         """
-        group = notification.thread or "default"
-        self.manager.history.remove(notification.identifier, group, self.app_id)
+        self.manager.history.remove(notification.identifier)
 
     async def _clear_all(self) -> None:
         """
         Asynchronously clears all notifications from notification center.
         """
         self.manager.history.clear(self.app_id)
```

### Comparing `desktop-notifier-3.5.1/src/desktop_notifier.egg-info/PKG-INFO` & `desktop-notifier-3.5.2/src/desktop_notifier.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: desktop-notifier
-Version: 3.5.1
+Version: 3.5.2
 Summary: Python library for cross-platform desktop notifications
 Author-email: Sam Schott <sam.schott@outlook.com>
 License: MIT
 Project-URL: Homepage, https://github.com/samschott/desktop-notifier
 Keywords: desktop-notifier
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `desktop-notifier-3.5.1/src/desktop_notifier.egg-info/SOURCES.txt` & `desktop-notifier-3.5.2/src/desktop_notifier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

