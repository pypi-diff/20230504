# Comparing `tmp/dankware-3.3.6.tar.gz` & `tmp/dankware-3.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dankware-3.3.6.tar", last modified: Wed May  3 10:16:02 2023, max compression
+gzip compressed data, was "dankware-3.3.7.tar", last modified: Thu May  4 16:17:41 2023, max compression
```

## Comparing `dankware-3.3.6.tar` & `dankware-3.3.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:16:02.504831 dankware-3.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-03 10:15:48.000000 dankware-3.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13801 2023-05-03 10:16:02.500831 dankware-3.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12862 2023-05-03 10:15:48.000000 dankware-3.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:16:02.500831 dankware-3.3.6/dankware/
--rw-r--r--   0 runner    (1001) docker     (123)    45681 2023-05-03 10:15:48.000000 dankware-3.3.6/dankware/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:16:02.500831 dankware-3.3.6/dankware.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13801 2023-05-03 10:16:02.000000 dankware-3.3.6/dankware.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-03 10:16:02.000000 dankware-3.3.6/dankware.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 10:16:02.000000 dankware-3.3.6/dankware.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-03 10:16:02.000000 dankware-3.3.6/dankware.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-03 10:16:02.000000 dankware-3.3.6/dankware.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 10:16:02.504831 dankware-3.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-03 10:15:48.000000 dankware-3.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:17:41.173611 dankware-3.3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-04 16:17:28.000000 dankware-3.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13801 2023-05-04 16:17:41.173611 dankware-3.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12862 2023-05-04 16:17:28.000000 dankware-3.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:17:41.169611 dankware-3.3.7/dankware/
+-rw-r--r--   0 runner    (1001) docker     (123)    46069 2023-05-04 16:17:28.000000 dankware-3.3.7/dankware/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:17:41.173611 dankware-3.3.7/dankware.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13801 2023-05-04 16:17:41.000000 dankware-3.3.7/dankware.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-04 16:17:41.000000 dankware-3.3.7/dankware.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 16:17:41.000000 dankware-3.3.7/dankware.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-04 16:17:41.000000 dankware-3.3.7/dankware.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-04 16:17:41.000000 dankware-3.3.7/dankware.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 16:17:41.173611 dankware-3.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-04 16:17:28.000000 dankware-3.3.7/setup.py
```

### Comparing `dankware-3.3.6/LICENSE` & `dankware-3.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dankware-3.3.6/PKG-INFO` & `dankware-3.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dankware
-Version: 3.3.6
+Version: 3.3.7
 Summary: Python package with various features!
 Home-page: https://github.com/SirDank/dankware
 Author: SirDank
 Author-email: SirDankenstein@protonmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/SirDank/dankware
 Project-URL: Bug Tracker, https://github.com/SirDank/dankware/issues
```

### Comparing `dankware-3.3.6/README.md` & `dankware-3.3.7/README.md`

 * *Files identical despite different names*

### Comparing `dankware-3.3.6/dankware/__init__.py` & `dankware-3.3.7/dankware/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,25 +21,15 @@
 green = Fore.GREEN + Style.BRIGHT
 magenta = Fore.MAGENTA + Style.BRIGHT
 red = Fore.RED + Style.BRIGHT
 reset = Style.RESET_ALL
 white = Fore.WHITE + Style.BRIGHT
 yellow = Fore.YELLOW + Style.BRIGHT
 
-# dankware variables
-
-chars = ['>','<','.',',','=','-','_','?','!','|','(',')','{','}','/','\\',':','"',"'","%"]
-words_green = ['true', 'True', 'TRUE', 'online', 'Online', 'ONLINE', 'successfully', 'Successfully', 'SUCCESSFULLY', 'successful', 'Successful', 'SUCCESSFUL', 'success', 'Success', 'SUCCESS']
-words_red = ['falsely', 'Falsely', 'FALSELY', 'false', 'False', 'FALSE', 'offline', 'Offline', 'OFFLINE', 'failures', 'Failures', 'FAILURES', 'failure', 'Failure', 'FAILURE', 'failed', 'Failed', 'FAILED', 'fail', 'Fail', 'FAIL']
-colours_to_replace = [Fore.BLACK, Fore.BLUE, Fore.CYAN, Fore.GREEN, Fore.MAGENTA, Fore.RED, Fore.WHITE, Fore.YELLOW, Style.BRIGHT, Style.RESET_ALL]
-colours_alt = ["BBLACKK", "BBLUEE", "CCYANN", "GGREENN", "MMAGENTAA", "RREDD", "WWHITEE", "YYELLOWW", "BBRIGHTT", "RRESETT"]
-bad_colours = ['BLACK', 'WHITE', 'LIGHTBLACK_EX', 'LIGHTWHITE_EX', 'RESET']
-codes = vars(Fore); colours = [codes[colour] for colour in codes if colour not in bad_colours]
-styles = [Style.BRIGHT, Style.DIM, Style.NORMAL]
-available_colours = ['black','red','green','cyan','blue','purple','random','black-v','red-v','green-v','cyan-v','blue-v','purple-v','pink-v']
+# --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 def multithread(function: callable, threads: int = 1, *args, progress_bar: bool = True) -> None:
     
     """
     > Please read the documentation on github before using this function!
     
     ________________________________________________________________________________
@@ -374,62 +364,82 @@
     ___________________________________________
 
     - mode: 4 | to display banners
     - text & spl = random (fixed colour)
     
     """
     
+    chars = ['[',']','>','<','.',',','=','-','_','?','!','|','(',')','{','}','/','\\',':','"',"'","%"]
+    
+    words_green = ['true', 'True', 'TRUE', 'online', 'Online', 'ONLINE', 'successfully', 'Successfully', 'SUCCESSFULLY', 'successful', 'Successful', 'SUCCESSFUL', 'success', 'Success', 'SUCCESS']
+    words_red = ['falsely', 'Falsely', 'FALSELY', 'false', 'False', 'FALSE', 'offline', 'Offline', 'OFFLINE', 'failures', 'Failures', 'FAILURES', 'failure', 'Failure', 'FAILURE', 'failed', 'Failed', 'FAILED', 'fail', 'Fail', 'FAIL']
+    
+    colours_to_replace = [Fore.BLACK, Fore.BLUE, Fore.CYAN, Fore.GREEN, Fore.MAGENTA, Fore.RED, Fore.WHITE, Fore.YELLOW, Style.BRIGHT, Style.RESET_ALL]
+    colours_alt = ["BBLACKK", "BBLUEE", "CCYANN", "GGREENN", "MMAGENTAA", "RREDD", "WWHITEE", "YYELLOWW", "BBRIGHTT", "RRESETT"]
+    
+    bad_colours = ['BLACK', 'WHITE', 'LIGHTBLACK_EX', 'LIGHTWHITE_EX', 'RESET']
+    codes = vars(Fore); colours = [codes[colour] for colour in codes if colour not in bad_colours]
+    styles = [Style.BRIGHT, Style.DIM, Style.NORMAL]
+    
     try:
-        if mode != 3:
+        if mode not in [3, 4]:
             for _ in range(len(colours_to_replace)):
                 text = text.replace(colours_to_replace[_], colours_alt[_])
         else:
             for _ in range(len(colours_to_replace)):
                 text = text.replace(colours_to_replace[_], '')
 
         # default
 
         if mode == 1:
-            text = text.replace("[",f"{colour_two}[{colour_one}").replace("]",f"{colour_two}]{colour_one}")
+            #text = text.replace("[",f"{colour_two}[{colour_one}").replace("]",f"{colour_two}]{colour_one}")
             for char in chars: text = text.replace(char, f"{colour_two}{char}{colour_one}")
             for word in words_green:
                 replacement = green.join(list(word))
                 text = text.replace(word, f"{green}{replacement}{colour_one}")
             for word in words_red:
                 replacement = red.join(list(word))
                 text = text.replace(word, f"{red}{replacement}{colour_one}")
         
         # for error messages
         
         elif mode == 2:
-            text = text.replace("[",f"{white}[{red}").replace("]",f"{white}]{red}")
+            #text = text.replace("[",f"{white}[{red}").replace("]",f"{white}]{red}")
             for char in chars: text = text.replace(char, f"{white}{char}{red}")
-            #for word in words_green: text = text.replace(word, f"{green}{word}{red}")
+            for word in words_green:
+                replacement = green.join(list(word))
+                text = text.replace(word, f"{green}{replacement}{red}")
         
         # random | TRUE, FALSE will not be coloured!
         
-        elif mode == 3 or mode == 4:
+        elif mode in [3, 4]:
+
             text = [char for char in text]
+            
             if mode == 3: colour_spl = True
             else: colour_spl = False
+    
             for _ in range(len(text)):
                 char = text[_]
                 if char != ' ' and char != '\n':
                     if colour_spl:
-                        if char in ( ['[',']'] + chars ): text[_] = white + char
-                        else: text[_] = random.choice(colours) + Style.BRIGHT + char
+                        if char in chars:
+                            text[_] = white + char
+                        else:
+                            text[_] = random.choice(colours) + Style.BRIGHT + char
                     else:
                         text[_] = random.choice(colours) + Style.BRIGHT + char
+
             text = ''.join(text)
 
         else: raise ValueError(f"\n  {white}> {red}Invalid Mode {white}[{red}{mode}{white}] | Valid Modes{white}: {red}1{white},{red}2{white},{red}3{white},{red}4" + reset)
 
-        if mode != 3:
+        if mode not in [3, 4]:
             for _ in range(len(colours_to_replace)):
-                text = str(text).replace(colours_alt[_], colours_to_replace[_])
+                text = text.replace(colours_alt[_], colours_to_replace[_])
 
         if mode == 1: return white + text + reset
         elif mode == 2: return red + text + reset
         elif mode == 3 or mode == 4: return text + reset
     
     except: sys.exit(clr(err(sys.exc_info()),2))
 
@@ -445,24 +455,26 @@
     from shutil import get_terminal_size
 
     width = get_terminal_size().columns; aligned = text
     for colour in vars(Fore).values(): aligned = aligned.replace(colour,'')
     for style in vars(Style).values(): aligned = aligned.replace(style,'')
     text = text.split('\n'); aligned = aligned.split('\n')
     for _ in range(len(aligned)): aligned[_] = aligned[_].center(width).replace(aligned[_],text[_])
-    return str('\n'.join(aligned))
+    return str('\n'.join(aligned) + reset)
 
 # --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 def fade(text: str, colour: str = "purple") -> str:
     
     """
     credits to https://github.com/venaxyt/gratient & https://github.com/venaxyt/fade <3
     - available_colours = black, red, green, cyan, blue, purple, random, black-v, red-v, green-v, cyan-v, blue-v, purple-v, pink-v
     """
+    
+    available_colours = ['black','red','green','cyan','blue','purple','random','black-v','red-v','green-v','cyan-v','blue-v','purple-v','pink-v']
 
     try:
         colour = colour.lower()
         if not colour in available_colours: raise ValueError(clr(f"\n  > Invalid Colour: {colour} | Available Colours: {', '.join(available_colours)}",2))
             
         faded = ""
         if len(text.splitlines()) > 1: multi_line = True
```

### Comparing `dankware-3.3.6/dankware.egg-info/PKG-INFO` & `dankware-3.3.7/dankware.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dankware
-Version: 3.3.6
+Version: 3.3.7
 Summary: Python package with various features!
 Home-page: https://github.com/SirDank/dankware
 Author: SirDank
 Author-email: SirDankenstein@protonmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/SirDank/dankware
 Project-URL: Bug Tracker, https://github.com/SirDank/dankware/issues
```

### Comparing `dankware-3.3.6/setup.py` & `dankware-3.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
 
     license = "MIT",
     name = "dankware",
-    version = "3.3.6",
+    version = "3.3.7",
     author = "SirDank",
     
     author_email = "SirDankenstein@protonmail.com",
     description = "Python package with various features!",
     long_description = open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type = "text/markdown",
     url = "https://github.com/SirDank/dankware",
```

