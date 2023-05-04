# Comparing `tmp/elm-messenger-0.0.1.tar.gz` & `tmp/elm-messenger-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elm-messenger-0.0.1.tar", last modified: Thu May  4 01:51:43 2023, max compression
+gzip compressed data, was "elm-messenger-0.1.0.tar", last modified: Thu May  4 07:32:14 2023, max compression
```

## Comparing `elm-messenger-0.0.1.tar` & `elm-messenger-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-04 01:51:43.547837 elm-messenger-0.0.1/
--rw-r--r--   0 linsy     (1000) linsy     (1000)       18 2023-05-04 01:49:08.000000 elm-messenger-0.0.1/MANIFEST.in
--rw-r--r--   0 linsy     (1000) linsy     (1000)      296 2023-05-04 01:51:43.547837 elm-messenger-0.0.1/PKG-INFO
--rw-r--r--   0 linsy     (1000) linsy     (1000)       31 2023-05-03 14:16:23.000000 elm-messenger-0.0.1/Readme.md
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-04 01:51:43.544504 elm-messenger-0.0.1/elm_messenger.egg-info/
--rw-r--r--   0 linsy     (1000) linsy     (1000)      296 2023-05-04 01:51:43.000000 elm-messenger-0.0.1/elm_messenger.egg-info/PKG-INFO
--rw-r--r--   0 linsy     (1000) linsy     (1000)      344 2023-05-04 01:51:43.000000 elm-messenger-0.0.1/elm_messenger.egg-info/SOURCES.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)        1 2023-05-04 01:51:43.000000 elm-messenger-0.0.1/elm_messenger.egg-info/dependency_links.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)       61 2023-05-04 01:51:43.000000 elm-messenger-0.0.1/elm_messenger.egg-info/entry_points.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)        6 2023-05-04 01:51:43.000000 elm-messenger-0.0.1/elm_messenger.egg-info/requires.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)       13 2023-05-04 01:51:43.000000 elm-messenger-0.0.1/elm_messenger.egg-info/top_level.txt
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-04 01:51:43.547837 elm-messenger-0.0.1/messengercli/
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2022-12-30 03:18:49.000000 elm-messenger-0.0.1/messengercli/__init__.py
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)      120 2023-05-04 01:48:19.000000 elm-messenger-0.0.1/messengercli/command_line.py
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)    10127 2023-05-04 01:35:41.000000 elm-messenger-0.0.1/messengercli/messenger.py
--rw-r--r--   0 linsy     (1000) linsy     (1000)      407 2023-05-04 01:51:43.547837 elm-messenger-0.0.1/setup.cfg
--rw-r--r--   0 linsy     (1000) linsy     (1000)      161 2023-05-04 01:51:13.000000 elm-messenger-0.0.1/setup.py
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-04 07:32:14.221730 elm-messenger-0.1.0/
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       18 2023-05-04 07:31:38.000000 elm-messenger-0.1.0/MANIFEST.in
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      296 2023-05-04 07:32:14.221730 elm-messenger-0.1.0/PKG-INFO
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       31 2023-05-04 07:31:38.000000 elm-messenger-0.1.0/Readme.md
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-04 07:32:14.221730 elm-messenger-0.1.0/elm_messenger.egg-info/
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      296 2023-05-04 07:32:14.000000 elm-messenger-0.1.0/elm_messenger.egg-info/PKG-INFO
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      344 2023-05-04 07:32:14.000000 elm-messenger-0.1.0/elm_messenger.egg-info/SOURCES.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)        1 2023-05-04 07:32:14.000000 elm-messenger-0.1.0/elm_messenger.egg-info/dependency_links.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       61 2023-05-04 07:32:14.000000 elm-messenger-0.1.0/elm_messenger.egg-info/entry_points.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)        6 2023-05-04 07:32:14.000000 elm-messenger-0.1.0/elm_messenger.egg-info/requires.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       13 2023-05-04 07:32:14.000000 elm-messenger-0.1.0/elm_messenger.egg-info/top_level.txt
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-04 07:32:14.221730 elm-messenger-0.1.0/messengercli/
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-04 07:31:38.000000 elm-messenger-0.1.0/messengercli/__init__.py
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)      120 2023-05-04 07:31:38.000000 elm-messenger-0.1.0/messengercli/command_line.py
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)     9533 2023-05-04 07:31:38.000000 elm-messenger-0.1.0/messengercli/messenger.py
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      407 2023-05-04 07:32:14.221730 elm-messenger-0.1.0/setup.cfg
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      161 2023-05-04 07:31:38.000000 elm-messenger-0.1.0/setup.py
```

### Comparing `elm-messenger-0.0.1/messengercli/messenger.py` & `elm-messenger-0.1.0/messengercli/messenger.py`

 * *Files 3% similar despite different names*

```diff
@@ -222,61 +222,49 @@
                 ",\n".join(
                     [
                         f"""( "{l}"
           , let
                 x =
                     {l}.layer
             in
-            {l}G.getLayerCT {{ x | data = {l}.layer.init t NullLayerMsg initCommonData }}
+            {l}G.getLayerT {{ x | data = {l}.layer.init t NullLayerMsg initCommonData }}
           )"""
                         for l in layers
                     ]
                 ),
             )
 
 
 @app.command()
 def init(
     name: str,
-    use_full: bool = typer.Option(
-        True,
-        prompt="""Thanks for using Messenger.
-There are currently two main versions you can use.
-The core version only has the basic framework. There are no core engine support. Use this version if you want to create your own game engine.
-The full version includes a core engine template which has a basic 2D physics engine and high-performance game component support. It enables you to create a level quickly.
-See more instructions on https://github.com/linsyking/Messenger.git
-Do you want to install the full version of Messerger?""",
-    ),
 ):
-    if use_full:
-        version = "full"
-        print("The full version is not supported yet...")
-        exit(0)
-    else:
-        version = "core"
     input(
-        f"""Here is my plan:
+        f"""Thanks for using Messenger.
+See https://github.com/linsyking/Messenger.git for more information.
+Here is my plan:
 - Create a directory named {name}
-- Use the {version} Messenger version
-- Elm install the packages needed
+- Install the core Messenger liberary
+- Install the elm packages needed
 Press Enter to continue
 """
     )
     os.makedirs(name, exist_ok=True)
     os.chdir(name)
     os.system(
-        f"git clone https://github.com/linsyking/Messenger.git .messenger --depth=1"
+        f"git clone -b templates https://github.com/linsyking/Messenger.git .messenger --depth=1"
     )
     shutil.copytree(".messenger/Templates/core/", "./src")
     shutil.copytree(".messenger/Templates/public/", "./public")
     shutil.copy(".messenger/Templates/.gitignore", "./.gitignore")
     shutil.copy(".messenger/Templates/Makefile", "./Makefile")
     shutil.copy(".messenger/Templates/elm.json", "./elm.json")
 
     os.makedirs("src/Scenes", exist_ok=True)
+    os.makedirs("assets", exist_ok=True)
     os.makedirs("src/Components", exist_ok=True)
 
     print("Creating elm.json...")
     initObject = {
         "scenes": {},
         "components": {},
         "gamecomponents": {},
```

