# Comparing `tmp/syncmaster-1.0.4.tar.gz` & `tmp/syncmaster-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syncmaster-1.0.4.tar", last modified: Wed May  3 14:34:04 2023, max compression
+gzip compressed data, was "syncmaster-1.0.5.tar", last modified: Thu May  4 10:44:50 2023, max compression
```

## Comparing `syncmaster-1.0.4.tar` & `syncmaster-1.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 conor     (1000) conor     (1000)        0 2023-05-03 14:34:04.945097 syncmaster-1.0.4/
--rw-rw-r--   0 conor     (1000) conor     (1000)    11337 2023-01-20 02:50:04.000000 syncmaster-1.0.4/LICENSE
--rw-rw-r--   0 conor     (1000) conor     (1000)      111 2023-01-20 02:50:04.000000 syncmaster-1.0.4/MANIFEST.in
--rw-rw-r--   0 conor     (1000) conor     (1000)     3560 2023-05-03 14:34:04.945097 syncmaster-1.0.4/PKG-INFO
--rw-rw-r--   0 conor     (1000) conor     (1000)     2708 2023-05-03 14:33:34.000000 syncmaster-1.0.4/README.md
--rw-rw-r--   0 conor     (1000) conor     (1000)      929 2023-05-03 14:24:28.000000 syncmaster-1.0.4/settings.ini
--rw-rw-r--   0 conor     (1000) conor     (1000)       38 2023-05-03 14:34:04.945097 syncmaster-1.0.4/setup.cfg
--rw-rw-r--   0 conor     (1000) conor     (1000)     2560 2023-01-20 02:50:04.000000 syncmaster-1.0.4/setup.py
-drwxrwxr-x   0 conor     (1000) conor     (1000)        0 2023-05-03 14:34:04.941097 syncmaster-1.0.4/syncmaster/
--rw-rw-r--   0 conor     (1000) conor     (1000)      235 2023-05-03 14:33:31.000000 syncmaster-1.0.4/syncmaster/__init__.py
--rw-rw-r--   0 conor     (1000) conor     (1000)     2057 2023-05-03 14:33:31.000000 syncmaster-1.0.4/syncmaster/_modidx.py
--rw-rw-r--   0 conor     (1000) conor     (1000)     2816 2023-05-03 14:33:31.000000 syncmaster-1.0.4/syncmaster/analysis.py
--rw-rw-r--   0 conor     (1000) conor     (1000)     3674 2023-05-03 14:33:31.000000 syncmaster-1.0.4/syncmaster/device.py
-drwxrwxr-x   0 conor     (1000) conor     (1000)        0 2023-05-03 14:34:04.945097 syncmaster-1.0.4/syncmaster.egg-info/
--rw-rw-r--   0 conor     (1000) conor     (1000)     3560 2023-05-03 14:34:04.000000 syncmaster-1.0.4/syncmaster.egg-info/PKG-INFO
--rw-rw-r--   0 conor     (1000) conor     (1000)      379 2023-05-03 14:34:04.000000 syncmaster-1.0.4/syncmaster.egg-info/SOURCES.txt
--rw-rw-r--   0 conor     (1000) conor     (1000)        1 2023-05-03 14:34:04.000000 syncmaster-1.0.4/syncmaster.egg-info/dependency_links.txt
--rw-rw-r--   0 conor     (1000) conor     (1000)       42 2023-05-03 14:34:04.000000 syncmaster-1.0.4/syncmaster.egg-info/entry_points.txt
--rw-rw-r--   0 conor     (1000) conor     (1000)        1 2023-04-17 10:19:07.000000 syncmaster-1.0.4/syncmaster.egg-info/not-zip-safe
--rw-rw-r--   0 conor     (1000) conor     (1000)       41 2023-05-03 14:34:04.000000 syncmaster-1.0.4/syncmaster.egg-info/requires.txt
--rw-rw-r--   0 conor     (1000) conor     (1000)       11 2023-05-03 14:34:04.000000 syncmaster-1.0.4/syncmaster.egg-info/top_level.txt
+drwxrwxr-x   0 conor     (1000) conor     (1000)        0 2023-05-04 10:44:50.962335 syncmaster-1.0.5/
+-rw-rw-r--   0 conor     (1000) conor     (1000)    11337 2023-01-20 02:50:04.000000 syncmaster-1.0.5/LICENSE
+-rw-rw-r--   0 conor     (1000) conor     (1000)      111 2023-01-20 02:50:04.000000 syncmaster-1.0.5/MANIFEST.in
+-rw-rw-r--   0 conor     (1000) conor     (1000)     3560 2023-05-04 10:44:50.962335 syncmaster-1.0.5/PKG-INFO
+-rw-rw-r--   0 conor     (1000) conor     (1000)     2708 2023-05-03 14:33:34.000000 syncmaster-1.0.5/README.md
+-rw-rw-r--   0 conor     (1000) conor     (1000)      929 2023-05-04 10:39:57.000000 syncmaster-1.0.5/settings.ini
+-rw-rw-r--   0 conor     (1000) conor     (1000)       38 2023-05-04 10:44:50.962335 syncmaster-1.0.5/setup.cfg
+-rw-rw-r--   0 conor     (1000) conor     (1000)     2560 2023-01-20 02:50:04.000000 syncmaster-1.0.5/setup.py
+drwxrwxr-x   0 conor     (1000) conor     (1000)        0 2023-05-04 10:44:50.962335 syncmaster-1.0.5/syncmaster/
+-rw-rw-r--   0 conor     (1000) conor     (1000)      235 2023-05-04 10:40:09.000000 syncmaster-1.0.5/syncmaster/__init__.py
+-rw-rw-r--   0 conor     (1000) conor     (1000)     2057 2023-05-04 10:40:09.000000 syncmaster-1.0.5/syncmaster/_modidx.py
+-rw-rw-r--   0 conor     (1000) conor     (1000)     2816 2023-05-04 10:40:09.000000 syncmaster-1.0.5/syncmaster/analysis.py
+-rw-rw-r--   0 conor     (1000) conor     (1000)     3667 2023-05-04 10:40:09.000000 syncmaster-1.0.5/syncmaster/device.py
+drwxrwxr-x   0 conor     (1000) conor     (1000)        0 2023-05-04 10:44:50.962335 syncmaster-1.0.5/syncmaster.egg-info/
+-rw-rw-r--   0 conor     (1000) conor     (1000)     3560 2023-05-04 10:44:50.000000 syncmaster-1.0.5/syncmaster.egg-info/PKG-INFO
+-rw-rw-r--   0 conor     (1000) conor     (1000)      379 2023-05-04 10:44:50.000000 syncmaster-1.0.5/syncmaster.egg-info/SOURCES.txt
+-rw-rw-r--   0 conor     (1000) conor     (1000)        1 2023-05-04 10:44:50.000000 syncmaster-1.0.5/syncmaster.egg-info/dependency_links.txt
+-rw-rw-r--   0 conor     (1000) conor     (1000)       42 2023-05-04 10:44:50.000000 syncmaster-1.0.5/syncmaster.egg-info/entry_points.txt
+-rw-rw-r--   0 conor     (1000) conor     (1000)        1 2023-04-17 10:19:07.000000 syncmaster-1.0.5/syncmaster.egg-info/not-zip-safe
+-rw-rw-r--   0 conor     (1000) conor     (1000)       41 2023-05-04 10:44:50.000000 syncmaster-1.0.5/syncmaster.egg-info/requires.txt
+-rw-rw-r--   0 conor     (1000) conor     (1000)       11 2023-05-04 10:44:50.000000 syncmaster-1.0.5/syncmaster.egg-info/top_level.txt
```

### Comparing `syncmaster-1.0.4/LICENSE` & `syncmaster-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `syncmaster-1.0.4/PKG-INFO` & `syncmaster-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncmaster
-Version: 1.0.4
+Version: 1.0.5
 Summary: Device and drivers for generating trigger signals to synchronise recorded signals with behavioural data
 Home-page: https://github.com/conorkeogh/syncmaster
 Author: Conor Keogh
 Author-email: conor.keogh@nds.ox.ac.uk
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `syncmaster-1.0.4/README.md` & `syncmaster-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `syncmaster-1.0.4/settings.ini` & `syncmaster-1.0.5/settings.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = syncmaster
 lib_name = syncmaster
-version = 1.0.4
+version = 1.0.5
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = syncmaster
 nbs_path = nbs
 recursive = True
```

### Comparing `syncmaster-1.0.4/setup.py` & `syncmaster-1.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `syncmaster-1.0.4/syncmaster/_modidx.py` & `syncmaster-1.0.5/syncmaster/_modidx.py`

 * *Files identical despite different names*

### Comparing `syncmaster-1.0.4/syncmaster/analysis.py` & `syncmaster-1.0.5/syncmaster/analysis.py`

 * *Files identical despite different names*

### Comparing `syncmaster-1.0.4/syncmaster/device.py` & `syncmaster-1.0.5/syncmaster/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         '''
 
         '''
         Define constants for device configuration
         '''
         # Define messages
         self.GREETING = b'<best wishes>'
-        self.RESPONSE = b'warmest regards'
+        self.RESPONSE = 'warmest regards'
         self.startMarker = '<'
         self.endMarker = '>'
     
         # Define trigger pulse widths (val*10, milliseconds)
         self.STARTPULSE = 5 # 50ms
         self.ENDPULSE = 10 # 100ms
         self.EVENT1PULSE = 15 # 150ms
@@ -58,15 +58,15 @@
         for port in ports:
             try:
                 # Connect to serial port
                 self.ser = serial.Serial(port.device, self.BAUDRATE, timeout=1, write_timeout=1)
 
                 # Send test message and read response; repeat 3 times and keep third
                 for _ in range(3):
-                    self.sendMessage(self.HOST_MESSAGE)
+                    self.ser.write(self.GREETING)
                     response = self.ser.readline()
 
                 # Check if response is appropriate
                 if response.decode().strip() == self.RESPONSE:
                     self.target_port = port.device
                     port_found = True
 
@@ -80,15 +80,15 @@
         # If port found: connect to port
         if port_found:
             self.ser = serial.Serial(self.target_port, self.BAUDRATE, timeout=5)
 
         # If port not found: raise error
         else:
             raise Exception("Device not found")
-#            print("Device not found")
+            #print("Device not found")
 
     ''' Send required messages over serial '''
 
     def start(self):
         ''' Send start signal '''
         self.sendMessage(self.STARTMARKER)
```

### Comparing `syncmaster-1.0.4/syncmaster.egg-info/PKG-INFO` & `syncmaster-1.0.5/syncmaster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncmaster
-Version: 1.0.4
+Version: 1.0.5
 Summary: Device and drivers for generating trigger signals to synchronise recorded signals with behavioural data
 Home-page: https://github.com/conorkeogh/syncmaster
 Author: Conor Keogh
 Author-email: conor.keogh@nds.ox.ac.uk
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

