# Comparing `tmp/panacotta-0.1.tar.gz` & `tmp/panacotta-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/panacotta-0.1.tar", last modified: Mon Nov 12 21:59:41 2018, max compression
+gzip compressed data, was "panacotta-0.2.tar", last modified: Thu May  4 18:08:17 2023, max compression
```

## Comparing `panacotta-0.1.tar` & `panacotta-0.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 noodles   (1000) noodles   (1000)        0 2018-11-12 21:59:41.000000 panacotta-0.1/
--rw-r--r--   0 noodles   (1000) noodles   (1000)     1520 2018-11-12 21:56:25.000000 panacotta-0.1/setup.py
-drwxr-xr-x   0 noodles   (1000) noodles   (1000)        0 2018-11-12 21:59:41.000000 panacotta-0.1/panacotta.egg-info/
--rw-r--r--   0 noodles   (1000) noodles   (1000)      172 2018-11-12 21:59:41.000000 panacotta-0.1/panacotta.egg-info/SOURCES.txt
--rw-r--r--   0 noodles   (1000) noodles   (1000)        1 2018-11-12 21:59:41.000000 panacotta-0.1/panacotta.egg-info/dependency_links.txt
--rw-r--r--   0 noodles   (1000) noodles   (1000)       10 2018-11-12 21:59:41.000000 panacotta-0.1/panacotta.egg-info/top_level.txt
--rw-r--r--   0 noodles   (1000) noodles   (1000)     1785 2018-11-12 21:59:41.000000 panacotta-0.1/panacotta.egg-info/PKG-INFO
--rw-r--r--   0 noodles   (1000) noodles   (1000)       38 2018-11-12 21:59:41.000000 panacotta-0.1/setup.cfg
-drwxr-xr-x   0 noodles   (1000) noodles   (1000)        0 2018-11-12 21:59:41.000000 panacotta-0.1/panacotta/
--rw-r--r--   0 noodles   (1000) noodles   (1000)     4817 2018-11-12 20:40:56.000000 panacotta-0.1/panacotta/__init__.py
--rw-r--r--   0 noodles   (1000) noodles   (1000)     1785 2018-11-12 21:59:41.000000 panacotta-0.1/PKG-INFO
--rw-r--r--   0 noodles   (1000) noodles   (1000)      991 2018-11-12 20:43:06.000000 panacotta-0.1/README.md
+drwxr-xr-x   0 noodles   (1000) noodles   (1000)        0 2023-05-04 18:08:17.434318 panacotta-0.2/
+-rw-r--r--   0 noodles   (1000) noodles   (1000)    35147 2018-11-11 16:10:29.000000 panacotta-0.2/LICENSE
+-rw-r--r--   0 noodles   (1000) noodles   (1000)     1639 2023-05-04 18:08:17.434318 panacotta-0.2/PKG-INFO
+-rw-r--r--   0 noodles   (1000) noodles   (1000)     1087 2023-05-04 18:06:33.000000 panacotta-0.2/README.md
+drwxr-xr-x   0 noodles   (1000) noodles   (1000)        0 2023-05-04 18:08:17.434318 panacotta-0.2/panacotta/
+-rw-r--r--   0 noodles   (1000) noodles   (1000)     6155 2023-05-04 18:06:55.000000 panacotta-0.2/panacotta/__init__.py
+drwxr-xr-x   0 noodles   (1000) noodles   (1000)        0 2023-05-04 18:08:17.434318 panacotta-0.2/panacotta.egg-info/
+-rw-r--r--   0 noodles   (1000) noodles   (1000)     1639 2023-05-04 18:08:17.000000 panacotta-0.2/panacotta.egg-info/PKG-INFO
+-rw-r--r--   0 noodles   (1000) noodles   (1000)      180 2023-05-04 18:08:17.000000 panacotta-0.2/panacotta.egg-info/SOURCES.txt
+-rw-r--r--   0 noodles   (1000) noodles   (1000)        1 2023-05-04 18:08:17.000000 panacotta-0.2/panacotta.egg-info/dependency_links.txt
+-rw-r--r--   0 noodles   (1000) noodles   (1000)       10 2023-05-04 18:08:17.000000 panacotta-0.2/panacotta.egg-info/top_level.txt
+-rw-r--r--   0 noodles   (1000) noodles   (1000)       38 2023-05-04 18:08:17.434318 panacotta-0.2/setup.cfg
+-rw-r--r--   0 noodles   (1000) noodles   (1000)     1520 2023-05-04 18:06:33.000000 panacotta-0.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `panacotta-0.1/setup.py` & `panacotta-0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
         long_description = fh.read()
 
 setuptools.setup(
     name='panacotta',
-    version="0.1",
+    version="0.2",
     author='Jonathan McDowell',
     author_email='noodles@earth.li',
     description='Python API for controlling Panasonic Blu-Ray players',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/u1f35c/python-panacotta',
     packages=setuptools.find_packages(),
```

### Comparing `panacotta-0.1/panacotta.egg-info/PKG-INFO` & `panacotta-0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 Metadata-Version: 2.1
 Name: panacotta
-Version: 0.1
+Version: 0.2
 Summary: Python API for controlling Panasonic Blu-Ray players
 Home-page: https://github.com/u1f35c/python-panacotta
 Author: Jonathan McDowell
 Author-email: noodles@earth.li
-License: UNKNOWN
-Description: Python control for Panasonic Blu-Ray players
-        ============================================
-        
-        This is a simple Python API for controlling Panasonic Blu-Ray players. It has only been tested with the DMP-BDT220, which dates from 2012. All players supported by the [Panasonic Blu-ray Remote 2012 Android app](https://play.google.com/store/apps/details?id=com.panasonic.avc.diga.blurayremote2012) should be supported; i.e. DMP-BDT120, DMP-BDT220, DMP-BDT221, DMP-BDT320, DMP-BDT500 and DMP-BBT01 devices.
-        
-        Example use
-        -----------
-        
-        Connect to a player on 192.168.0.4 and find out the current playing status:
-        
-        ```
-        import panacotta
-        
-        bluray = panacotta.PansonicBD('192.168.0.4')
-        print("Device is currently %s" % bluray.get_play_status()[0])
-        ```
-        
-        Note that the device must be on the same subnet as the host running this API; requests from a different subnet will return a failure.
-        
-        Press the power button:
-        
-        ```
-        import panacotta
-        
-        bluray = panacotta.PansonicBD('192.168.0.4')
-        bluray.send_key('POWER')
-        ```
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+Python control for Panasonic Blu-Ray players
+============================================
+
+This is a simple Python API for controlling Panasonic Blu-Ray players. It has only been tested with the DMP-BDT220, which dates from 2012. All players supported by the [Panasonic Blu-ray Remote 2012 Android app](https://play.google.com/store/apps/details?id=com.panasonic.avc.diga.blurayremote2012) should be supported; i.e. DMP-BDT120, DMP-BDT220, DMP-BDT221, DMP-BDT320, DMP-BDT500 and DMP-BBT01 devices.
+
+Newer players with "UB" prefixes (e.g. the UB-9000) support a (very) limited set of functions.
+
+Example use
+-----------
+
+Connect to a player on 192.168.0.4 and find out the current playing status:
+
+```
+import panacotta
+
+bluray = panacotta.PansonicBD('192.168.0.4')
+print("Device is currently %s" % bluray.get_play_status()[0])
+```
+
+Note that the device must be on the same subnet as the host running this API; requests from a different subnet will return a failure.
+
+Press the power button:
+
+```
+import panacotta
+
+bluray = panacotta.PansonicBD('192.168.0.4')
+bluray.send_key('POWER')
+```
```

### Comparing `panacotta-0.1/panacotta/__init__.py` & `panacotta-0.2/panacotta/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from enum import Enum
+
 import urllib.request
 
 # Must send these headers to not be ignored
 HEADERS = {'User-Agent': 'MEI-LAN-REMOTE-CALL'}
 # Known key commands
 KEYS = ['POWER', 'OP_CL',
         'PLAYBACK', 'PAUSE', 'STOP', 'SKIPFWD', 'SKIPREV', 'REV',
@@ -35,21 +37,28 @@
         'KEYS', 'CUE', 'CHROMA',
         'MNBACK', 'MNSKIP', '2NDARY', 'PICTMD', 'DETAIL', 'RESOLUTN',
         # Playback view?
         'OSDONOFF', 'P_IN_P',
         ]
 
 
+class PlayerVariant(Enum):
+    AUTO = 1
+    BD = 2
+    UB = 3
+
+
 class PanasonicBD:
     """Class to interact with Panasonic Blu-Ray Players."""
 
-    def __init__(self, host):
+    def __init__(self, host, variant=PlayerVariant.AUTO):
         self._host = host
         self._state = None
         self._duration = 0
+        self._variant = variant
 
     def send_cmd(self, url, data):
         req = urllib.request.Request(url, data, HEADERS)
         try:
             response = urllib.request.urlopen(req, timeout=5)
         except OSError:
             # If we can't reach the device, assume it's off
@@ -67,28 +76,58 @@
 
     def send_key(self, key):
         """ Send the supplied keypress to the device """
         # Sanity check it's a valid key
         if key not in KEYS:
             return ['error', None]
 
+        # Check the player supports it
+        if self._variant == PlayerVariant.UB:
+            return ['error', None]
+
         url = 'http://%s/WAN/%s/%s_ctrl.cgi' % (self._host, 'dvdr', 'dvdr')
         data = ('cCMD_RC_%s.x=100&cCMD_RC_%s.y=100' % (key, key)).encode()
 
-        return self.send_cmd(url, data)
+        resp = self.send_cmd(url, data)
+        # If we're auto-detecting player type then assume we're an newer UB
+        # variant if we got an error, and an older BD if it worked
+        if self._variant == PlayerVariant.AUTO:
+            if resp[0] == 'error':
+                self._variant = PlayerVariant.UB
+                return ['error', None]
+            else:
+                self._variant = PlayerVariant.BD
+
+        return resp
 
     def get_status(self):
+        # Check the player supports it, return a dummy response if not
+        if self._variant == PlayerVariant.UB:
+            return ['1', '0', '0', '00000000', '0']
+
         url = 'http://%s/WAN/%s/%s_ctrl.cgi' % (self._host, 'dvdr', 'dvdr')
         data = b'cCMD_GET_STATUS.x=100&cCMD_GET_STATUS.y=100'
 
         resp = self.send_cmd(url, data)
+        if resp[0] == 'error':
+            # If we got an error and we're auto-detecting player type assume
+            # it's a more modern UB
+            if self._variant == PlayerVariant.AUTO:
+                self._variant = PlayerVariant.UB
+                return ['1', '0', '0', '00000000', '0']
+            else:
+                return ['error']
+
+        # If we get here and we're still auto-detecting player type we can
+        # assume an older BD variant.
+        if self._variant == PlayerVariant.AUTO:
+            self._variant = PlayerVariant.BD
+
         if resp[0] == 'off':
             return ['off']
-        elif resp[0] == 'error':
-            return ['error']
 
         # Response is of the form:
         #  2,0,0,248,0,1,8,2,0,00000000
         #
         # 0: 0 == standby, playing or paused / 2 == stopped or menu
         # 3: Playing time
         # 4: Total time
```

### Comparing `panacotta-0.1/PKG-INFO` & `panacotta-0.2/panacotta.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 Metadata-Version: 2.1
 Name: panacotta
-Version: 0.1
+Version: 0.2
 Summary: Python API for controlling Panasonic Blu-Ray players
 Home-page: https://github.com/u1f35c/python-panacotta
 Author: Jonathan McDowell
 Author-email: noodles@earth.li
-License: UNKNOWN
-Description: Python control for Panasonic Blu-Ray players
-        ============================================
-        
-        This is a simple Python API for controlling Panasonic Blu-Ray players. It has only been tested with the DMP-BDT220, which dates from 2012. All players supported by the [Panasonic Blu-ray Remote 2012 Android app](https://play.google.com/store/apps/details?id=com.panasonic.avc.diga.blurayremote2012) should be supported; i.e. DMP-BDT120, DMP-BDT220, DMP-BDT221, DMP-BDT320, DMP-BDT500 and DMP-BBT01 devices.
-        
-        Example use
-        -----------
-        
-        Connect to a player on 192.168.0.4 and find out the current playing status:
-        
-        ```
-        import panacotta
-        
-        bluray = panacotta.PansonicBD('192.168.0.4')
-        print("Device is currently %s" % bluray.get_play_status()[0])
-        ```
-        
-        Note that the device must be on the same subnet as the host running this API; requests from a different subnet will return a failure.
-        
-        Press the power button:
-        
-        ```
-        import panacotta
-        
-        bluray = panacotta.PansonicBD('192.168.0.4')
-        bluray.send_key('POWER')
-        ```
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+Python control for Panasonic Blu-Ray players
+============================================
+
+This is a simple Python API for controlling Panasonic Blu-Ray players. It has only been tested with the DMP-BDT220, which dates from 2012. All players supported by the [Panasonic Blu-ray Remote 2012 Android app](https://play.google.com/store/apps/details?id=com.panasonic.avc.diga.blurayremote2012) should be supported; i.e. DMP-BDT120, DMP-BDT220, DMP-BDT221, DMP-BDT320, DMP-BDT500 and DMP-BBT01 devices.
+
+Newer players with "UB" prefixes (e.g. the UB-9000) support a (very) limited set of functions.
+
+Example use
+-----------
+
+Connect to a player on 192.168.0.4 and find out the current playing status:
+
+```
+import panacotta
+
+bluray = panacotta.PansonicBD('192.168.0.4')
+print("Device is currently %s" % bluray.get_play_status()[0])
+```
+
+Note that the device must be on the same subnet as the host running this API; requests from a different subnet will return a failure.
+
+Press the power button:
+
+```
+import panacotta
+
+bluray = panacotta.PansonicBD('192.168.0.4')
+bluray.send_key('POWER')
+```
```

### Comparing `panacotta-0.1/README.md` & `panacotta-0.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Python control for Panasonic Blu-Ray players
 ============================================
 
 This is a simple Python API for controlling Panasonic Blu-Ray players. It has only been tested with the DMP-BDT220, which dates from 2012. All players supported by the [Panasonic Blu-ray Remote 2012 Android app](https://play.google.com/store/apps/details?id=com.panasonic.avc.diga.blurayremote2012) should be supported; i.e. DMP-BDT120, DMP-BDT220, DMP-BDT221, DMP-BDT320, DMP-BDT500 and DMP-BBT01 devices.
 
+Newer players with "UB" prefixes (e.g. the UB-9000) support a (very) limited set of functions.
+
 Example use
 -----------
 
 Connect to a player on 192.168.0.4 and find out the current playing status:
 
 ```
 import panacotta
```

