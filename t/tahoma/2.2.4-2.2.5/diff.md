# Comparing `tmp/tahoma-2.2.4.tar.gz` & `tmp/tahoma-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tahoma-2.2.4.tar", last modified: Sun Apr 16 07:56:23 2023, max compression
+gzip compressed data, was "tahoma-2.2.5.tar", last modified: Thu May  4 12:16:30 2023, max compression
```

## Comparing `tahoma-2.2.4.tar` & `tahoma-2.2.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-04-16 07:56:23.678277 tahoma-2.2.4/
--rwxrwx---   0 neptune   (1000) neptune   (1000)     1070 2023-02-18 00:22:37.000000 tahoma-2.2.4/LICENSE
--rwxrwx---   0 neptune   (1000) neptune   (1000)      142 2023-02-21 14:35:21.000000 tahoma-2.2.4/MANIFEST.in
--rwxrwx---   0 neptune   (1000) neptune   (1000)     6133 2023-04-16 07:56:23.678441 tahoma-2.2.4/PKG-INFO
--rwxrwx---   0 neptune   (1000) neptune   (1000)     5471 2023-04-05 16:49:55.000000 tahoma-2.2.4/PYPI_README.md
--rwxrwx---   0 neptune   (1000) neptune   (1000)     5471 2023-04-05 16:50:21.000000 tahoma-2.2.4/README.md
--rwxrwx---   0 neptune   (1000) neptune   (1000)     1201 2023-02-21 21:29:00.000000 tahoma-2.2.4/pyproject.toml
--rwxrwx---   0 neptune   (1000) neptune   (1000)       41 2023-02-21 17:24:01.000000 tahoma-2.2.4/requirements.txt
--rwxrwx---   0 neptune   (1000) neptune   (1000)       38 2023-04-16 07:56:23.678954 tahoma-2.2.4/setup.cfg
--rwxrwx---   0 neptune   (1000) neptune   (1000)      125 2023-02-15 20:31:23.000000 tahoma-2.2.4/setup.py
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-04-16 07:56:23.671422 tahoma-2.2.4/tahoma/
--rwxrwx---   0 neptune   (1000) neptune   (1000)      134 2023-02-21 18:24:33.000000 tahoma-2.2.4/tahoma/__init__.py
--rwxrwx---   0 neptune   (1000) neptune   (1000)       22 2023-04-16 07:53:03.000000 tahoma-2.2.4/tahoma/__version__.py
--rwxrwx---   0 neptune   (1000) neptune   (1000)     5469 2023-04-05 15:40:09.000000 tahoma-2.2.4/tahoma/get_devices_url.py
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-04-16 07:56:23.675872 tahoma-2.2.4/tahoma/icons/
--rwxrwx---   0 neptune   (1000) neptune   (1000)        5 2023-02-18 00:33:06.000000 tahoma-2.2.4/tahoma/icons/__init__.py
--rwxrwx---   0 neptune   (1000) neptune   (1000)    21160 2023-02-15 08:39:56.000000 tahoma-2.2.4/tahoma/icons/connected_house.png
--rwxrwx---   0 neptune   (1000) neptune   (1000)    29722 2023-02-15 17:48:11.000000 tahoma-2.2.4/tahoma/icons/water heater.png
--rwxrwx---   0 neptune   (1000) neptune   (1000)      668 2023-02-21 09:02:06.000000 tahoma-2.2.4/tahoma/install_tahoma.py
--rwxrwx---   0 neptune   (1000) neptune   (1000)    35274 2023-04-16 07:49:29.000000 tahoma-2.2.4/tahoma/tahoma.py
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-04-16 07:56:23.676628 tahoma-2.2.4/tahoma/temp/
--rwxrwx---   0 neptune   (1000) neptune   (1000)        5 2023-02-18 00:32:54.000000 tahoma-2.2.4/tahoma/temp/__init__.py
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-04-16 07:56:23.677883 tahoma-2.2.4/tahoma/test/
--rwxrwx---   0 neptune   (1000) neptune   (1000)        5 2023-02-18 00:33:06.000000 tahoma-2.2.4/tahoma/test/__init__.py
--rwxrwx---   0 neptune   (1000) neptune   (1000)       23 2021-07-13 15:25:04.000000 tahoma-2.2.4/tahoma/test/test.py
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-04-16 07:56:23.674321 tahoma-2.2.4/tahoma.egg-info/
--rwxrwx---   0 neptune   (1000) neptune   (1000)     6133 2023-04-16 07:56:23.000000 tahoma-2.2.4/tahoma.egg-info/PKG-INFO
--rwxrwx---   0 neptune   (1000) neptune   (1000)      542 2023-04-16 07:56:23.000000 tahoma-2.2.4/tahoma.egg-info/SOURCES.txt
--rwxrwx---   0 neptune   (1000) neptune   (1000)        1 2023-04-16 07:56:23.000000 tahoma-2.2.4/tahoma.egg-info/dependency_links.txt
--rwxrwx---   0 neptune   (1000) neptune   (1000)       46 2023-04-16 07:56:23.000000 tahoma-2.2.4/tahoma.egg-info/entry_points.txt
--rwxrwx---   0 neptune   (1000) neptune   (1000)       41 2023-04-16 07:56:23.000000 tahoma-2.2.4/tahoma.egg-info/requires.txt
--rwxrwx---   0 neptune   (1000) neptune   (1000)        7 2023-04-16 07:56:23.000000 tahoma-2.2.4/tahoma.egg-info/top_level.txt
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-05-04 12:16:30.318843 tahoma-2.2.5/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     1070 2023-02-18 00:22:37.000000 tahoma-2.2.5/LICENSE
+-rwxrwx---   0 neptune   (1000) neptune   (1000)      142 2023-02-21 14:35:21.000000 tahoma-2.2.5/MANIFEST.in
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     6416 2023-05-04 12:16:30.319178 tahoma-2.2.5/PKG-INFO
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     5754 2023-05-04 11:36:22.000000 tahoma-2.2.5/PYPI_README.md
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     5753 2023-05-04 11:36:20.000000 tahoma-2.2.5/README.md
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     1201 2023-02-21 21:29:00.000000 tahoma-2.2.5/pyproject.toml
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       41 2023-02-21 17:24:01.000000 tahoma-2.2.5/requirements.txt
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       38 2023-05-04 12:16:30.320181 tahoma-2.2.5/setup.cfg
+-rwxrwx---   0 neptune   (1000) neptune   (1000)      125 2023-02-15 20:31:23.000000 tahoma-2.2.5/setup.py
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-05-04 12:16:30.309385 tahoma-2.2.5/tahoma/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)      134 2023-02-21 18:24:33.000000 tahoma-2.2.5/tahoma/__init__.py
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       22 2023-05-04 12:16:06.000000 tahoma-2.2.5/tahoma/__version__.py
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     5469 2023-04-05 15:40:09.000000 tahoma-2.2.5/tahoma/get_devices_url.py
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-05-04 12:16:30.315569 tahoma-2.2.5/tahoma/icons/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)        5 2023-02-18 00:33:06.000000 tahoma-2.2.5/tahoma/icons/__init__.py
+-rwxrwx---   0 neptune   (1000) neptune   (1000)    21160 2023-02-15 08:39:56.000000 tahoma-2.2.5/tahoma/icons/connected_house.png
+-rwxrwx---   0 neptune   (1000) neptune   (1000)    29722 2023-02-15 17:48:11.000000 tahoma-2.2.5/tahoma/icons/water heater.png
+-rwxrwx---   0 neptune   (1000) neptune   (1000)      668 2023-02-21 09:02:06.000000 tahoma-2.2.5/tahoma/install_tahoma.py
+-rwxrwx---   0 neptune   (1000) neptune   (1000)    36253 2023-05-04 11:44:29.000000 tahoma-2.2.5/tahoma/tahoma.py
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-05-04 12:16:30.316598 tahoma-2.2.5/tahoma/temp/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)        5 2023-02-18 00:32:54.000000 tahoma-2.2.5/tahoma/temp/__init__.py
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-05-04 12:16:30.318192 tahoma-2.2.5/tahoma/test/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)        5 2023-02-18 00:33:06.000000 tahoma-2.2.5/tahoma/test/__init__.py
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       23 2021-07-13 15:25:04.000000 tahoma-2.2.5/tahoma/test/test.py
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-05-04 12:16:30.313018 tahoma-2.2.5/tahoma.egg-info/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     6416 2023-05-04 12:16:30.000000 tahoma-2.2.5/tahoma.egg-info/PKG-INFO
+-rwxrwx---   0 neptune   (1000) neptune   (1000)      542 2023-05-04 12:16:30.000000 tahoma-2.2.5/tahoma.egg-info/SOURCES.txt
+-rwxrwx---   0 neptune   (1000) neptune   (1000)        1 2023-05-04 12:16:30.000000 tahoma-2.2.5/tahoma.egg-info/dependency_links.txt
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       46 2023-05-04 12:16:30.000000 tahoma-2.2.5/tahoma.egg-info/entry_points.txt
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       41 2023-05-04 12:16:30.000000 tahoma-2.2.5/tahoma.egg-info/requires.txt
+-rwxrwx---   0 neptune   (1000) neptune   (1000)        7 2023-05-04 12:16:30.000000 tahoma-2.2.5/tahoma.egg-info/top_level.txt
```

### Comparing `tahoma-2.2.4/LICENSE` & `tahoma-2.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tahoma-2.2.4/PKG-INFO` & `tahoma-2.2.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tahoma
-Version: 2.2.4
+Version: 2.2.5
 Summary: This is a very easy API for controlling Somfy Tahoma's devices written in Python3, thanks to the pyoverkiz API. You just need a three-word input to control a device
 Author-email: Pzim-devdata <contact@pzim.fr>
 Project-URL: Homepage, https://github.com/pzim-devdata/tahoma
 Project-URL: Bug Tracker, https://github.com/pzim-devdata/tahoma/issues
 Keywords: tahoma,somfy,api
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -106,17 +106,19 @@
 
 # Usage : 
 `tahoma [ACTION] [CATEGORY] [NAME]`
 
 
 For instance : `tahoma open shutter kitchen` or `tahoma ouvrir volet cuisine`
 
+You can also close a shutter or a sunscreen to a specific level. For example, to close to 25%, you can use the commands : `tahoma 25 shutter kitchen` or `tahoma 25 sunscreen kitchen`. Please note that this feature only works with IO protocols and not with RTS.
+
 You can also run many commands during the same process without restarting tahoma ;
 
-For instance : `tahoma arm alarm garden open shutter kitchen close shutter room6 confort heater dining off plug office`
+For instance : `tahoma arm alarm garden open shutter kitchen close shutter room6 confort heater dining off plug office 25 sunscreen kitchen`
 
 
 # But first you need to retrieve your PERSONALS commands :
 
 
 ## Get a list of all possibles [ACTIONS] for each [CATEGORIES] :
```

### Comparing `tahoma-2.2.4/PYPI_README.md` & `tahoma-2.2.5/PYPI_README.md`

 * *Files 2% similar despite different names*

```diff
@@ -91,17 +91,19 @@
 
 # Usage : 
 `tahoma [ACTION] [CATEGORY] [NAME]`
 
 
 For instance : `tahoma open shutter kitchen` or `tahoma ouvrir volet cuisine`
 
+You can also close a shutter or a sunscreen to a specific level. For example, to close to 25%, you can use the commands : `tahoma 25 shutter kitchen` or `tahoma 25 sunscreen kitchen`. Please note that this feature only works with IO protocols and not with RTS.
+
 You can also run many commands during the same process without restarting tahoma ;
 
-For instance : `tahoma arm alarm garden open shutter kitchen close shutter room6 confort heater dining off plug office`
+For instance : `tahoma arm alarm garden open shutter kitchen close shutter room6 confort heater dining off plug office 25 sunscreen kitchen`
 
 
 # But first you need to retrieve your PERSONALS commands :
 
 
 ## Get a list of all possibles [ACTIONS] for each [CATEGORIES] :
```

### Comparing `tahoma-2.2.4/README.md` & `tahoma-2.2.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -91,18 +91,19 @@
 
 # Usage : 
 `tahoma [ACTION] [CATEGORY] [NAME]`
 
 
 For instance : `tahoma open shutter kitchen` or `tahoma ouvrir volet cuisine`
 
-You can also run many commands during the same process without restarting tahoma ;
+You can also close a shutter or a sunscreen to a specific level. For example, to close to 25%, you can use the commands : `tahoma 25 shutter kitchen` or `tahoma 25 sunscreen kitchen`. Please note that this feature only works with IO protocols and not with RTS.
 
-For instance : `tahoma arm alarm garden open shutter kitchen close shutter room6 confort heater dining off plug office`
+You can also run many commands during the same process without restarting tahoma ;
 
+For instance : `tahoma arm alarm garden open shutter kitchen close shutter room6 confort heater dining off plug office 25 sunscreen kitchen`
 
 # But first you need to retrieve your PERSONALS commands :
 
 
 ## Get a list of all possibles [ACTIONS] for each [CATEGORIES] : 
 
 Open a terminal and type :
```

### Comparing `tahoma-2.2.4/pyproject.toml` & `tahoma-2.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tahoma-2.2.4/tahoma/get_devices_url.py` & `tahoma-2.2.5/tahoma/get_devices_url.py`

 * *Files identical despite different names*

### Comparing `tahoma-2.2.4/tahoma/icons/connected_house.png` & `tahoma-2.2.5/tahoma/icons/connected_house.png`

 * *Files identical despite different names*

### Comparing `tahoma-2.2.4/tahoma/icons/water heater.png` & `tahoma-2.2.5/tahoma/icons/water heater.png`

 * *Files identical despite different names*

### Comparing `tahoma-2.2.4/tahoma/install_tahoma.py` & `tahoma-2.2.5/tahoma/install_tahoma.py`

 * *Files identical despite different names*

### Comparing `tahoma-2.2.4/tahoma/tahoma.py` & `tahoma-2.2.5/tahoma/tahoma.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,16 +40,16 @@
 
     notification_consent = os.path.dirname(os.path.abspath(__file__))+'/temp/consent_notification.txt'
 
     server_choosen =  os.path.dirname(os.path.abspath(__file__))+'/temp/server_choosen.txt'
 
     list_categories = ['shutter','spotalarm','plug','alarm','heater','sunscreen']
     list_categories_french = ['volet','spotalarme','prise','alarme','chauffage','rideau']
-    list_actions = ['[open,close,stop,my]','[on,off]','[on,off]','[arm,disarm,partial,arm_night,arm_away]','[comfort,comfort-1,comfort-2,eco,off]','[open,close,stop,my]']
-    list_actions_french = ['[ouvrir,fermer,stop,my]','[allumer,eteindre]','[allumer,eteindre]','[activer,desactiver,partiel,activer_nuit,activer_parti]','[confort,confort-1,confort-2,eco,eteindre]','[ouvrir,fermer,stop,my]']
+    list_actions = ['[open,close,stop,my,NUMBER]','[on,off]','[on,off]','[arm,disarm,partial,arm_night,arm_away]','[comfort,comfort-1,comfort-2,eco,off]','[open,close,stop,my,NUMBER]']
+    list_actions_french = ['[ouvrir,fermer,stop,my,NOMBRE]','[allumer,eteindre]','[allumer,eteindre]','[activer,desactiver,partiel,activer_nuit,activer_parti]','[confort,confort-1,confort-2,eco,eteindre]','[ouvrir,fermer,stop,my,NOMBRE]']
 
     try :
         f = open(notification_consent, 'r')
         notification = f.read()
         f.close()
     except FileNotFoundError:
         notification = 'n'
@@ -78,15 +78,15 @@
         print( "" )
         print( " - List of possible CATEGORIES : \n "+str(list_categories) )
         print( " - Liste des CATEGORIES possibles : \n "+str(list_categories_french) )
         print( "" )
         print( " - List of available NAMES : tahoma --list-names \n - Liste des NOMS possibles : tahoma --list-names-french \n You must provide a part of the name you have assigned to the device in the Tahoma App. \n It must be a single and unic word, not taken by another device of the same category !\n For instance if you have two devices called <Alarm 1> and <Alarm 2> you will need to choose <2> as device [NAME] for <Alarm 2> and not <Alarm>).\n See tahoma --list or tahoma --help for info")
         print( "" )
         print( "                  You must provide at least 3 arguments" )
-        print( "         For instance : python3 tahoma open shutter kitchen" )
+        print( "         For instance : python3 tahoma open shutter kitchen or python3 tahoma 25 shutter kitchen" )
         print( "" )
         print( " You can also provide, as many as you wish, orders on the same line." ) 
         print( " Tahoma will execute all orders one by one on the same process ;-)" )
         print( " For instance : tahoma open shutter kitchen arm alarm garden on plug room wait train garestation " )
         print( "" )
         print( " FIRST you must configure login and password : sudo tahoma -c " )
         print( " It will be stored there : \n "+passwd_file )
@@ -363,30 +363,35 @@
                 print("There is no match. The <NAME> you gave is not exact. Did you mean : "+str(bad_name)+" ? Choose a UNIQUE part of word from this results as <NAME> argument\nIf you don't find your device in this results try tahoma --getlist\nSee tahoma --list-names for help.")
                 exit()
             if len(url) > 1 :
                 print("There is more than one match. The <NAME> you gave is not exact. Choose a UNIQUE part of word from this results as <NAME> argument : "+str(too_many_urls)+"\nSee tahoma --list-names for help.")
                 exit()
 
             if remove_accent(action).upper() == "OPEN" or remove_accent(action).upper() == "OUVRIR" :
-                fonction = Command(OverkizCommand.OPEN, [0])
+                fonction = Command(OverkizCommand.OPEN)
             elif remove_accent(action).upper() == 'CLOSE' or remove_accent(action).upper() == "FERMER" :
-                fonction = Command(OverkizCommand.CLOSE, [0])
+                fonction = Command(OverkizCommand.CLOSE)
             elif remove_accent(action).upper() == 'STOP' :
-                fonction = Command(OverkizCommand.STOP, [0])
+                print("Be careful! The 'stop' function is only available for IO protocols. It doesn't work with RTS devices, it will use the 'MY'function instead...")
+                fonction = Command(OverkizCommand.STOP)
             elif remove_accent(action).upper() == 'MY' :
-                fonction = Command(OverkizCommand.MY, [0])
+                fonction = Command(OverkizCommand.MY)
+            elif str(action).isnumeric() == True :
+                fonction = Command(OverkizCommand.SET_CLOSURE, [int(action)])
+                print('Will close to '+str(action)+' %')
+                print("Be careful! This function is only available for IO protocols. It doesn't work with RTS devices...")
             else :
                 print( "\n'"+action+"'"+" is not a valide action.\n")
                 print("Please provide one of this argument as action : [open close stop my]")
             str1 = " "
             print("Output action : "+remove_accent(action).upper()+" "+remove_accent(category)+" "+str1.join(good_name)+ " \nwith url : "+str1.join(url))
 
         ##########################SUNSCREEN
         
-        if remove_accent(category) == 'sunscreen' or remove_accent(category) == 'rideau':
+        elif remove_accent(category) == 'sunscreen' or remove_accent(category) == 'rideau':
             f = open(list_of_tahoma_sunscreens, 'r')
             content = f.read()
             f.close()
             try:
                 master_list = content.split("\n")
                 master_list.remove('')
             except ValueError:
@@ -402,21 +407,26 @@
                 print("There is no match. The <NAME> you gave is not exact. Did you mean : "+str(bad_name)+" ? Choose a UNIQUE part of word from this results as <NAME> argument\nIf you don't find your device in this results try tahoma --getlist\nSee tahoma --list-names for help.")
                 exit()
             if len(url) > 1 :
                 print("There is more than one match. The <NAME> you gave is not exact. Choose a UNIQUE part of word from this results as <NAME> argument : "+str(too_many_urls)+"\nSee tahoma --list-names for help.")
                 exit()
 
             if remove_accent(action).upper() == "OPEN" or remove_accent(action).upper() == "OUVRIR" :
-                fonction = Command(OverkizCommand.OPEN, [0])
+                fonction = Command(OverkizCommand.OPEN)
             elif remove_accent(action).upper() == 'CLOSE' or remove_accent(action).upper() == "FERMER" :
-                fonction = Command(OverkizCommand.CLOSE, [0])
+                fonction = Command(OverkizCommand.CLOSE)
             elif remove_accent(action).upper() == 'STOP' :
-                fonction = Command(OverkizCommand.STOP, [0])
+                print("Be careful! The 'stop' function is only available for IO protocols. It doesn't work with RTS devices, it will use the 'MY'function instead...")
+                fonction = Command(OverkizCommand.STOP)
             elif remove_accent(action).upper() == 'MY' :
-                fonction = Command(OverkizCommand.MY, [0])
+                fonction = Command(OverkizCommand.MY)
+            elif str(action).isnumeric() == True :
+                fonction = Command(OverkizCommand.SET_CLOSURE, [int(action)])
+                print('Will close to '+str(action)+' %')
+                print("Be careful! This function is only available for IO protocols. It doesn't work with RTS devices...")
             else :
                 print( "\n'"+action+"'"+" is not a valide action.\n")
                 print("Please provide one of this argument as action : [open close stop my]")
             str1 = " "
             print("Output action : "+remove_accent(action).upper()+" "+remove_accent(category)+" "+str1.join(good_name)+ " \nwith url : "+str1.join(url))
 
         ##########################SPOTALARMS AND PLUGS
```

### Comparing `tahoma-2.2.4/tahoma.egg-info/PKG-INFO` & `tahoma-2.2.5/tahoma.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tahoma
-Version: 2.2.4
+Version: 2.2.5
 Summary: This is a very easy API for controlling Somfy Tahoma's devices written in Python3, thanks to the pyoverkiz API. You just need a three-word input to control a device
 Author-email: Pzim-devdata <contact@pzim.fr>
 Project-URL: Homepage, https://github.com/pzim-devdata/tahoma
 Project-URL: Bug Tracker, https://github.com/pzim-devdata/tahoma/issues
 Keywords: tahoma,somfy,api
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -106,17 +106,19 @@
 
 # Usage : 
 `tahoma [ACTION] [CATEGORY] [NAME]`
 
 
 For instance : `tahoma open shutter kitchen` or `tahoma ouvrir volet cuisine`
 
+You can also close a shutter or a sunscreen to a specific level. For example, to close to 25%, you can use the commands : `tahoma 25 shutter kitchen` or `tahoma 25 sunscreen kitchen`. Please note that this feature only works with IO protocols and not with RTS.
+
 You can also run many commands during the same process without restarting tahoma ;
 
-For instance : `tahoma arm alarm garden open shutter kitchen close shutter room6 confort heater dining off plug office`
+For instance : `tahoma arm alarm garden open shutter kitchen close shutter room6 confort heater dining off plug office 25 sunscreen kitchen`
 
 
 # But first you need to retrieve your PERSONALS commands :
 
 
 ## Get a list of all possibles [ACTIONS] for each [CATEGORIES] :
```

### Comparing `tahoma-2.2.4/tahoma.egg-info/SOURCES.txt` & `tahoma-2.2.5/tahoma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

