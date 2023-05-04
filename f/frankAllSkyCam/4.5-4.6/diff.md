# Comparing `tmp/frankAllSkyCam-4.5.tar.gz` & `tmp/frankAllSkyCam-4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frankAllSkyCam-4.5.tar", last modified: Sun Apr 30 22:01:46 2023, max compression
+gzip compressed data, was "frankAllSkyCam-4.6.tar", last modified: Thu May  4 18:36:25 2023, max compression
```

## Comparing `frankAllSkyCam-4.5.tar` & `frankAllSkyCam-4.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-30 22:01:46.890419 frankAllSkyCam-4.5/
--rw-r--r--   0 pi        (1000) pi        (1000)      899 2023-04-30 22:01:46.890419 frankAllSkyCam-4.5/PKG-INFO
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-30 22:01:46.886419 frankAllSkyCam-4.5/frankAllSkyCam/
--rwxrw-rw-   0 pi        (1000) pi        (1000)       71 2023-04-30 21:24:46.397862 frankAllSkyCam-4.5/frankAllSkyCam/__init__.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     3041 2023-04-30 21:35:10.315263 frankAllSkyCam-4.5/frankAllSkyCam/__main__.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)      722 2023-04-30 21:24:46.397862 frankAllSkyCam-4.5/frankAllSkyCam/allskycamdelete.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     3400 2023-04-30 21:24:46.397862 frankAllSkyCam-4.5/frankAllSkyCam/crontab.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     1331 2023-04-30 21:24:46.397862 frankAllSkyCam-4.5/frankAllSkyCam/drawtext.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     2318 2023-04-30 21:24:46.397862 frankAllSkyCam-4.5/frankAllSkyCam/fileManager.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-30 22:01:46.886419 frankAllSkyCam-4.5/frankAllSkyCam/helper/
--rwxrw-rw-   0 pi        (1000) pi        (1000)     3081 2023-04-30 21:47:13.522558 frankAllSkyCam-4.5/frankAllSkyCam/helper/config.txt
--rwxr-xr-x   0 pi        (1000) pi        (1000)      503 2023-04-30 21:24:45.893867 frankAllSkyCam-4.5/frankAllSkyCam/helper/index.html
--rwxrw-rw-   0 pi        (1000) pi        (1000)    17690 2023-04-30 21:24:46.397862 frankAllSkyCam-4.5/frankAllSkyCam/imageHeader.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     2818 2023-04-30 21:24:46.397862 frankAllSkyCam-4.5/frankAllSkyCam/startrail.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     6939 2023-04-30 21:24:46.401862 frankAllSkyCam-4.5/frankAllSkyCam/suncalc2.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)      941 2023-04-30 21:24:46.401862 frankAllSkyCam-4.5/frankAllSkyCam/test_sqm.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     2263 2023-04-30 21:24:46.401862 frankAllSkyCam-4.5/frankAllSkyCam/test_suncalc.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     4172 2023-04-30 21:24:46.401862 frankAllSkyCam-4.5/frankAllSkyCam/timelapse.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     1293 2023-04-30 21:24:46.401862 frankAllSkyCam-4.5/frankAllSkyCam/watchDog.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)       65 2023-04-26 18:08:27.179909 frankAllSkyCam-4.5/setup.cfg
--rwxrwxrw-   0 pi        (1000) pi        (1000)     2552 2023-04-30 21:58:43.695128 frankAllSkyCam-4.5/setup.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-30 22:01:46.886419 frankAllSkyCam-4.5/test/
--rwxrw-rw-   0 pi        (1000) pi        (1000)      941 2023-04-16 16:51:13.326836 frankAllSkyCam-4.5/test/test_sqm.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     2263 2023-04-05 15:29:11.227398 frankAllSkyCam-4.5/test/test_suncalc.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-04 18:36:25.909125 frankAllSkyCam-4.6/
+-rw-r--r--   0 pi        (1000) pi        (1000)      899 2023-05-04 18:36:25.909125 frankAllSkyCam-4.6/PKG-INFO
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-04 18:36:25.909125 frankAllSkyCam-4.6/frankAllSkyCam/
+-rwxrw-rw-   0 pi        (1000) pi        (1000)       71 2023-05-04 18:35:53.641444 frankAllSkyCam-4.6/frankAllSkyCam/__init__.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     3047 2023-05-04 18:27:02.206678 frankAllSkyCam-4.6/frankAllSkyCam/__main__.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)      722 2023-04-30 21:24:46.397862 frankAllSkyCam-4.6/frankAllSkyCam/allskycamdelete.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     3400 2023-04-30 21:24:46.397862 frankAllSkyCam-4.6/frankAllSkyCam/crontab.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     1331 2023-04-30 21:24:46.397862 frankAllSkyCam-4.6/frankAllSkyCam/drawtext.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     2318 2023-04-30 21:24:46.397862 frankAllSkyCam-4.6/frankAllSkyCam/fileManager.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-04 18:36:25.909125 frankAllSkyCam-4.6/frankAllSkyCam/helper/
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     3081 2023-04-30 21:47:13.522558 frankAllSkyCam-4.6/frankAllSkyCam/helper/config.txt
+-rwxr-xr-x   0 pi        (1000) pi        (1000)      503 2023-04-30 21:24:45.893867 frankAllSkyCam-4.6/frankAllSkyCam/helper/index.html
+-rwxrw-rw-   0 pi        (1000) pi        (1000)    17690 2023-04-30 21:24:46.397862 frankAllSkyCam-4.6/frankAllSkyCam/imageHeader.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     2818 2023-04-30 21:24:46.397862 frankAllSkyCam-4.6/frankAllSkyCam/startrail.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     6939 2023-04-30 21:24:46.401862 frankAllSkyCam-4.6/frankAllSkyCam/suncalc2.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)      941 2023-04-30 21:24:46.401862 frankAllSkyCam-4.6/frankAllSkyCam/test_sqm.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     2263 2023-04-30 21:24:46.401862 frankAllSkyCam-4.6/frankAllSkyCam/test_suncalc.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     4172 2023-04-30 21:24:46.401862 frankAllSkyCam-4.6/frankAllSkyCam/timelapse.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     1293 2023-04-30 21:24:46.401862 frankAllSkyCam-4.6/frankAllSkyCam/watchDog.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)       65 2023-04-26 18:08:27.179909 frankAllSkyCam-4.6/setup.cfg
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     2598 2023-05-04 18:34:51.466059 frankAllSkyCam-4.6/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-04 18:36:25.909125 frankAllSkyCam-4.6/test/
+-rwxrw-rw-   0 pi        (1000) pi        (1000)      941 2023-04-16 16:51:13.326836 frankAllSkyCam-4.6/test/test_sqm.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     2263 2023-04-05 15:29:11.227398 frankAllSkyCam-4.6/test/test_suncalc.py
```

### Comparing `frankAllSkyCam-4.5/PKG-INFO` & `frankAllSkyCam-4.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: frankAllSkyCam
-Version: 4.5
+Version: 4.6
 Summary: AllSkyCamera with Raspberry Pi and Pi HQ Camera 
 Home-page: https://github.com/sferlix/frankAllSkyCam
 Author: Francesco Sferlazza
 Author-email: sferlazza@gmail.com
 License: MIT
-Download-URL: https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/4.4.tar.gz
+Download-URL: https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/4.6.tar.gz
 Description: UNKNOWN
 Keywords: AllSkyCamera,Astronomy,AllSky
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `frankAllSkyCam-4.5/frankAllSkyCam/__main__.py` & `frankAllSkyCam-4.6/frankAllSkyCam/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     nomefile = fileManager.getOutputFileName(outputFolder, x) + TL + ".jpg"
     print("executing capture:")
 
     comando = "libcamera-still -o " + nomefile
     comando += " -n --width " + str(horiz) + " --height "+ str(vert) + " --immediate "
 
     if esposiz >0:
-       comando +=" --gain 18 --awbgains 2.2,2.2 --shutter " + str(int(esposiz))
+       comando +=" --gain 18 --awbgains 2.2,2.2 --shutter " + str(int(esposiz)) + " "
        comando += additional_params
     else:
        comando += " --metering average "
 
     try:
        # ensure no libcamera is operating
        killcmd = "ps -ef|grep libcamera-still| grep -v color|awk '{print $2}'|xargs kill -9 1> /dev/null 2>&1"
```

### Comparing `frankAllSkyCam-4.5/frankAllSkyCam/allskycamdelete.py` & `frankAllSkyCam-4.6/frankAllSkyCam/allskycamdelete.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-4.5/frankAllSkyCam/crontab.py` & `frankAllSkyCam-4.6/frankAllSkyCam/crontab.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-4.5/frankAllSkyCam/drawtext.py` & `frankAllSkyCam-4.6/frankAllSkyCam/drawtext.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-4.5/frankAllSkyCam/fileManager.py` & `frankAllSkyCam-4.6/frankAllSkyCam/fileManager.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-4.5/frankAllSkyCam/helper/config.txt` & `frankAllSkyCam-4.6/frankAllSkyCam/helper/config.txt`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-4.5/frankAllSkyCam/imageHeader.py` & `frankAllSkyCam-4.6/frankAllSkyCam/imageHeader.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-4.5/frankAllSkyCam/startrail.py` & `frankAllSkyCam-4.6/frankAllSkyCam/startrail.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-4.5/frankAllSkyCam/suncalc2.py` & `frankAllSkyCam-4.6/frankAllSkyCam/suncalc2.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-4.5/frankAllSkyCam/test_sqm.py` & `frankAllSkyCam-4.6/frankAllSkyCam/test_sqm.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-4.5/frankAllSkyCam/test_suncalc.py` & `frankAllSkyCam-4.6/frankAllSkyCam/test_suncalc.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-4.5/frankAllSkyCam/timelapse.py` & `frankAllSkyCam-4.6/frankAllSkyCam/timelapse.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-4.5/frankAllSkyCam/watchDog.py` & `frankAllSkyCam-4.6/frankAllSkyCam/watchDog.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-4.5/setup.py` & `frankAllSkyCam-4.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import os
 import shutil
 from distutils.core import setup
 
-homepath = os.path.expanduser("~")
 setup(
   name = 'frankAllSkyCam',         # How you named your package folder (MyLib)
   packages = ['frankAllSkyCam'],   # Chose the same as "name"
-  version = '4.5',      # Start with a small number and increase it with every change you make
+  version = '4.6',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'AllSkyCamera with Raspberry Pi and Pi HQ Camera ',   # Give a short description about your library
   author = 'Francesco Sferlazza',                   # Type in your name
   author_email = 'sferlazza@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/sferlix/frankAllSkyCam',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/4.4.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/4.6.tar.gz',    # I explain this later on
   keywords = ['AllSkyCamera', 'Astronomy', 'AllSky'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'pytz',
           'numpy',
       ],
   classifiers=[
     'Development Status :: 4 - Beta',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
@@ -28,14 +27,16 @@
     'Programming Language :: Python :: 3.5',
     'Programming Language :: Python :: 3.6',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.9',
   ],
 )
 
+homepath = os.path.expanduser("~")
+print("your homedir is: " + homepath + "\n")
 if os.path.exists(homepath+"/frankAllSkyCam") == False:
     os.mkdir(homepath+"/frankAllSkyCam")
 
 if os.path.exists(homepath+"/frankAllSkyCam/img") == False:
     os.mkdir(homepath+"/frankAllSkyCam/img")
 
 if os.path.exists(homepath+"/frankAllSkyCam/log") == False:
```

### Comparing `frankAllSkyCam-4.5/test/test_sqm.py` & `frankAllSkyCam-4.6/test/test_sqm.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-4.5/test/test_suncalc.py` & `frankAllSkyCam-4.6/test/test_suncalc.py`

 * *Files identical despite different names*

