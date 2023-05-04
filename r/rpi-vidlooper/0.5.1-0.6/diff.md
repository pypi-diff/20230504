# Comparing `tmp/rpi_vidlooper-0.5.1.tar.gz` & `tmp/rpi_vidlooper-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rpi_vidlooper-0.5.1.tar", last modified: Sun May 30 17:19:19 2021, max compression
+gzip compressed data, was "rpi_vidlooper-0.6.tar", last modified: Thu May  4 09:07:45 2023, max compression
```

## Comparing `rpi_vidlooper-0.5.1.tar` & `rpi_vidlooper-0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-05-30 17:19:19.000000 rpi_vidlooper-0.5.1/
--rw-rw-r--   0 travis    (2000) travis    (2000)       56 2021-05-30 17:19:00.000000 rpi_vidlooper-0.5.1/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)    68611 2021-05-30 17:19:00.000000 rpi_vidlooper-0.5.1/versioneer.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-05-30 17:19:19.000000 rpi_vidlooper-0.5.1/rpi_vidlooper.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3237 2021-05-30 17:19:19.000000 rpi_vidlooper-0.5.1/rpi_vidlooper.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-05-30 17:19:19.000000 rpi_vidlooper-0.5.1/rpi_vidlooper.egg-info/zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-05-30 17:19:19.000000 rpi_vidlooper-0.5.1/rpi_vidlooper.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       14 2021-05-30 17:19:19.000000 rpi_vidlooper-0.5.1/rpi_vidlooper.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      397 2021-05-30 17:19:19.000000 rpi_vidlooper-0.5.1/rpi_vidlooper.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2021-05-30 17:19:19.000000 rpi_vidlooper-0.5.1/rpi_vidlooper.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       60 2021-05-30 17:19:19.000000 rpi_vidlooper-0.5.1/rpi_vidlooper.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     3237 2021-05-30 17:19:19.000000 rpi_vidlooper-0.5.1/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2954 2021-05-30 17:19:00.000000 rpi_vidlooper-0.5.1/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      219 2021-05-30 17:19:19.000000 rpi_vidlooper-0.5.1/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1069 2021-05-30 17:19:00.000000 rpi_vidlooper-0.5.1/LICENSE
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-05-30 17:19:19.000000 rpi_vidlooper-0.5.1/rpi_vidlooper/
--rw-rw-r--   0 travis    (2000) travis    (2000)      497 2021-05-30 17:19:19.000000 rpi_vidlooper-0.5.1/rpi_vidlooper/_version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      151 2021-05-30 17:19:00.000000 rpi_vidlooper-0.5.1/rpi_vidlooper/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10574 2021-05-30 17:19:00.000000 rpi_vidlooper-0.5.1/rpi_vidlooper/vidlooper.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      871 2021-05-30 17:19:00.000000 rpi_vidlooper-0.5.1/setup.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-04 09:07:45.794668 rpi_vidlooper-0.6/
+-rw-r--r--   0 alex       (501) staff       (20)     1069 2019-01-21 01:11:52.000000 rpi_vidlooper-0.6/LICENSE
+-rw-r--r--   0 alex       (501) staff       (20)       56 2019-01-21 04:54:21.000000 rpi_vidlooper-0.6/MANIFEST.in
+-rw-r--r--   0 alex       (501) staff       (20)     3179 2023-05-04 09:07:45.794722 rpi_vidlooper-0.6/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)     2954 2020-06-06 19:50:16.000000 rpi_vidlooper-0.6/README.md
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-04 09:07:45.795034 rpi_vidlooper-0.6/rpi_vidlooper/
+-rw-r--r--   0 alex       (501) staff       (20)      151 2019-01-21 04:54:21.000000 rpi_vidlooper-0.6/rpi_vidlooper/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)      495 2023-05-04 09:07:45.795061 rpi_vidlooper-0.6/rpi_vidlooper/_version.py
+-rw-r--r--   0 alex       (501) staff       (20)    11237 2023-04-29 21:50:51.000000 rpi_vidlooper-0.6/rpi_vidlooper/vidlooper.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-04 09:07:45.794446 rpi_vidlooper-0.6/rpi_vidlooper.egg-info/
+-rw-r--r--   0 alex       (501) staff       (20)     3179 2023-05-04 09:07:45.000000 rpi_vidlooper-0.6/rpi_vidlooper.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)      397 2023-05-04 09:07:45.000000 rpi_vidlooper-0.6/rpi_vidlooper.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2023-05-04 09:07:45.000000 rpi_vidlooper-0.6/rpi_vidlooper.egg-info/dependency_links.txt
+-rw-r--r--   0 alex       (501) staff       (20)       59 2023-05-04 09:07:45.000000 rpi_vidlooper-0.6/rpi_vidlooper.egg-info/entry_points.txt
+-rw-r--r--   0 alex       (501) staff       (20)        9 2023-05-04 09:07:45.000000 rpi_vidlooper-0.6/rpi_vidlooper.egg-info/requires.txt
+-rw-r--r--   0 alex       (501) staff       (20)       14 2023-05-04 09:07:45.000000 rpi_vidlooper-0.6/rpi_vidlooper.egg-info/top_level.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2019-01-21 03:57:35.000000 rpi_vidlooper-0.6/rpi_vidlooper.egg-info/zip-safe
+-rw-r--r--   0 alex       (501) staff       (20)      219 2023-05-04 09:07:45.794914 rpi_vidlooper-0.6/setup.cfg
+-rw-r--r--   0 alex       (501) staff       (20)      871 2021-02-16 04:10:26.000000 rpi_vidlooper-0.6/setup.py
+-rw-r--r--   0 alex       (501) staff       (20)    68611 2019-01-21 04:54:21.000000 rpi_vidlooper-0.6/versioneer.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `rpi_vidlooper-0.5.1/versioneer.py` & `rpi_vidlooper-0.6/versioneer.py`

 * *Files identical despite different names*

### Comparing `rpi_vidlooper-0.5.1/rpi_vidlooper.egg-info/PKG-INFO` & `rpi_vidlooper-0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 Metadata-Version: 2.1
-Name: rpi-vidlooper
-Version: 0.5.1
+Name: rpi_vidlooper
+Version: 0.6
 Summary: Raspberry Pi GPIO-controlled video looper
-Home-page: UNKNOWN
 Author: Alex Lubbock
 Author-email: code@alexlubbock.com
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # rpi-vidlooper
 
 A video looper for the Raspberry Pi, controlled by GPIO pins. Designed to
 run an unattended video display, where users can select the active video
@@ -91,9 +88,7 @@
 
 ## Further reading
 
 * [Raspberry Pi Video Player Hardware tutorial](https://alexlubbock.com/raspberry-pi-video-player-hardware)
 * [Raspberry Pi Video Player Software tutorial](https://alexlubbock.com/raspberry-pi-video-player-software)
 * [Python on the Raspberry Pi](https://www.raspberrypi.org/documentation/linux/software/python.md)
 * [OMXPlayer, a hardware-accelerated video player for Raspberry Pi](https://www.raspberrypi.org/documentation/raspbian/applications/omxplayer.md)
-
-
```

### Comparing `rpi_vidlooper-0.5.1/PKG-INFO` & `rpi_vidlooper-0.6/rpi_vidlooper.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 Metadata-Version: 2.1
-Name: rpi_vidlooper
-Version: 0.5.1
+Name: rpi-vidlooper
+Version: 0.6
 Summary: Raspberry Pi GPIO-controlled video looper
-Home-page: UNKNOWN
 Author: Alex Lubbock
 Author-email: code@alexlubbock.com
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # rpi-vidlooper
 
 A video looper for the Raspberry Pi, controlled by GPIO pins. Designed to
 run an unattended video display, where users can select the active video
@@ -91,9 +88,7 @@
 
 ## Further reading
 
 * [Raspberry Pi Video Player Hardware tutorial](https://alexlubbock.com/raspberry-pi-video-player-hardware)
 * [Raspberry Pi Video Player Software tutorial](https://alexlubbock.com/raspberry-pi-video-player-software)
 * [Python on the Raspberry Pi](https://www.raspberrypi.org/documentation/linux/software/python.md)
 * [OMXPlayer, a hardware-accelerated video player for Raspberry Pi](https://www.raspberrypi.org/documentation/raspbian/applications/omxplayer.md)
-
-
```

### Comparing `rpi_vidlooper-0.5.1/README.md` & `rpi_vidlooper-0.6/README.md`

 * *Files identical despite different names*

### Comparing `rpi_vidlooper-0.5.1/LICENSE` & `rpi_vidlooper-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rpi_vidlooper-0.5.1/rpi_vidlooper/vidlooper.py` & `rpi_vidlooper-0.6/rpi_vidlooper/vidlooper.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,20 +63,23 @@
     _active_vid = None
 
     # The process of the active video player
     _p = None
 
     def __init__(self, audio='hdmi', autostart=True, restart_on_press=False,
                  video_dir=os.getcwd(), videos=None, gpio_pins=None, loop=True,
-                 no_osd=False, splash=None, debug=False):
+                 no_osd=False, shutdown_pin=None, splash=None, debug=False):
         # Use default GPIO pins, if needed
         if gpio_pins is None:
             gpio_pins = self._GPIO_PIN_DEFAULT.copy()
         self.gpio_pins = gpio_pins
 
+        # Add shutdown pin
+        self.shutdown_pin = shutdown_pin
+
         # Assemble the list of videos to play, if needed
         if videos:
             self.videos = videos
             for video in videos:
                 if not os.path.exists(video):
                     raise FileNotFoundError('Video "{}" not found'.format(video))
         else:
@@ -154,14 +157,22 @@
         GPIO.setmode(GPIO.BCM)
         for in_pin, out_pin in self.gpio_pins.items():
             GPIO.setup(in_pin, GPIO.IN, pull_up_down=GPIO.PUD_UP)
             if out_pin is not None:
                 GPIO.setup(out_pin, GPIO.OUT)
                 GPIO.output(out_pin, GPIO.LOW)
 
+        # Set up the shutdown pin
+        if self.shutdown_pin:
+            GPIO.setup(self.shutdown_pin, GPIO.IN, pull_up_down=GPIO.PUD_UP)
+            GPIO.add_event_detect(self.shutdown_pin,
+                                  GPIO.FALLING,
+                                  callback=lambda _: call(['shutdown', '-h', 'now'], shell=False),
+                                  bouncetime=self._GPIO_BOUNCE_TIME)
+
         if self.autostart:
             if self.splash is not None:
                 self._splashproc = Popen(['fbi', '--noverbose', '-a',
                                           self.splash])
             else:
                 # Start playing first video
                 self.switch_vid(self.in_pins[0])
@@ -212,30 +223,30 @@
     parser = argparse.ArgumentParser(
         formatter_class=argparse.RawDescriptionHelpFormatter,
         description="""Raspberry Pi video player controlled by GPIO pins
 
 This program is designed to power a looping video display, where the active
 video can be changed by pressing a button (i.e. by shorting a GPIO pin).
 The active video can optionally be indicated by an LED (one output for each
-input pin; works well with switches with built-in LEDs, but separate LEDs work 
+input pin; works well with switches with built-in LEDs, but separate LEDs work
 too).
 
 This video player uses omxplayer, a hardware-accelerated video player for the
-Raspberry Pi, which must be installed separately.        
+Raspberry Pi, which must be installed separately.
 """
     )
     parser.add_argument('--audio', default='hdmi',
                         choices=('hdmi', 'local', 'both'),
                         help='Output audio over HDMI, local (headphone jack),'
-                             'or both.')
+                             'or both')
     parser.add_argument('--no-autostart', action='store_false',
                         dest='autostart', default=True,
                         help='Don\'t start playing a video on startup')
     parser.add_argument('--no-loop', action='store_false', default=True,
-                        dest='loop', help='Loop the active video indefinitely.')
+                        dest='loop', help='Don\'t loop the active video')
     parser.add_argument(
         '--restart-on-press', action='store_true', default=False,
         help='If True, restart the current video if the button for the active '
              'video is pressed. If False, pressing the button for the active '
              'video will be ignored.')
     vidmode = parser.add_mutually_exclusive_group()
     vidmode.add_argument(
@@ -247,22 +258,25 @@
     parser.add_argument('--gpio-pins', default=VidLooper._GPIO_PIN_DEFAULT,
                         action=_GpioParser,
                         help='List of GPIO pins. Either INPUT:OUTPUT pairs, or '
                              'just INPUT pins (no output), separated by '
                              'commas.')
     parser.add_argument('--debug', action='store_true', default=False,
                         help='Debug mode (don\'t clear screen or suppress '
-                             'terminal output.')
+                             'terminal output)')
     parser.add_argument('--countdown', type=int, default=0,
                         help='Add a countdown before start (time in seconds)')
     parser.add_argument('--splash', type=str, default=None,
                         help='Splash screen image to show when no video is '
                              'playing')
     parser.add_argument('--no-osd', action='store_true', default=False,
-                        help='Don\'t show on-screen display when changing videos')
+                        help='Don\'t show on-screen display when changing '
+                             'videos')
+    parser.add_argument('--shutdown-pin', type=int, default=None,
+                        help='GPIO pin to trigger system shutdown (default None)')
 
     # Invoke the videoplayer
     args = parser.parse_args()
 
     # Apply any countdown
     countdown = args.countdown
```

### Comparing `rpi_vidlooper-0.5.1/setup.py` & `rpi_vidlooper-0.6/setup.py`

 * *Files identical despite different names*

