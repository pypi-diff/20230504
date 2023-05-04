# Comparing `tmp/elm-messenger-0.1.1.tar.gz` & `tmp/elm-messenger-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elm-messenger-0.1.1.tar", last modified: Thu May  4 07:37:36 2023, max compression
+gzip compressed data, was "elm-messenger-0.1.2.tar", last modified: Thu May  4 12:39:55 2023, max compression
```

## Comparing `elm-messenger-0.1.1.tar` & `elm-messenger-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-04 07:37:36.726777 elm-messenger-0.1.1/
--rw-r--r--   0 linsy     (1000) linsy     (1000)       18 2023-05-04 07:37:03.000000 elm-messenger-0.1.1/MANIFEST.in
--rw-r--r--   0 linsy     (1000) linsy     (1000)      296 2023-05-04 07:37:36.726777 elm-messenger-0.1.1/PKG-INFO
--rw-r--r--   0 linsy     (1000) linsy     (1000)       31 2023-05-04 07:37:03.000000 elm-messenger-0.1.1/Readme.md
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-04 07:37:36.726777 elm-messenger-0.1.1/elm_messenger.egg-info/
--rw-r--r--   0 linsy     (1000) linsy     (1000)      296 2023-05-04 07:37:36.000000 elm-messenger-0.1.1/elm_messenger.egg-info/PKG-INFO
--rw-r--r--   0 linsy     (1000) linsy     (1000)      344 2023-05-04 07:37:36.000000 elm-messenger-0.1.1/elm_messenger.egg-info/SOURCES.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)        1 2023-05-04 07:37:36.000000 elm-messenger-0.1.1/elm_messenger.egg-info/dependency_links.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)       61 2023-05-04 07:37:36.000000 elm-messenger-0.1.1/elm_messenger.egg-info/entry_points.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)        6 2023-05-04 07:37:36.000000 elm-messenger-0.1.1/elm_messenger.egg-info/requires.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)       13 2023-05-04 07:37:36.000000 elm-messenger-0.1.1/elm_messenger.egg-info/top_level.txt
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-04 07:37:36.726777 elm-messenger-0.1.1/messengercli/
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-04 07:37:03.000000 elm-messenger-0.1.1/messengercli/__init__.py
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)      120 2023-05-04 07:37:03.000000 elm-messenger-0.1.1/messengercli/command_line.py
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)     9476 2023-05-04 07:37:03.000000 elm-messenger-0.1.1/messengercli/messenger.py
--rw-r--r--   0 linsy     (1000) linsy     (1000)      407 2023-05-04 07:37:36.726777 elm-messenger-0.1.1/setup.cfg
--rw-r--r--   0 linsy     (1000) linsy     (1000)      161 2023-05-04 07:37:03.000000 elm-messenger-0.1.1/setup.py
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-04 12:39:55.466770 elm-messenger-0.1.2/
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       18 2023-05-04 10:50:53.000000 elm-messenger-0.1.2/MANIFEST.in
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      387 2023-05-04 12:39:55.466770 elm-messenger-0.1.2/PKG-INFO
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      122 2023-05-04 10:50:53.000000 elm-messenger-0.1.2/Readme.md
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-04 12:39:55.466770 elm-messenger-0.1.2/elm_messenger.egg-info/
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      387 2023-05-04 12:39:55.000000 elm-messenger-0.1.2/elm_messenger.egg-info/PKG-INFO
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      344 2023-05-04 12:39:55.000000 elm-messenger-0.1.2/elm_messenger.egg-info/SOURCES.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)        1 2023-05-04 12:39:55.000000 elm-messenger-0.1.2/elm_messenger.egg-info/dependency_links.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       61 2023-05-04 12:39:55.000000 elm-messenger-0.1.2/elm_messenger.egg-info/entry_points.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)        6 2023-05-04 12:39:55.000000 elm-messenger-0.1.2/elm_messenger.egg-info/requires.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       13 2023-05-04 12:39:55.000000 elm-messenger-0.1.2/elm_messenger.egg-info/top_level.txt
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-04 12:39:55.466770 elm-messenger-0.1.2/messengercli/
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-04 10:50:53.000000 elm-messenger-0.1.2/messengercli/__init__.py
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)      120 2023-05-04 10:50:53.000000 elm-messenger-0.1.2/messengercli/command_line.py
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)     9159 2023-05-04 10:54:19.000000 elm-messenger-0.1.2/messengercli/messenger.py
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      407 2023-05-04 12:39:55.466770 elm-messenger-0.1.2/setup.cfg
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      161 2023-05-04 10:50:53.000000 elm-messenger-0.1.2/setup.py
```

### Comparing `elm-messenger-0.1.1/messengercli/messenger.py` & `elm-messenger-0.1.2/messengercli/messenger.py`

 * *Files 23% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         os.mkdir(f"src/Scenes/{name}")
 
     def update_scenes(self):
         """
         Update scene settings (AllScenes and SceneSettings)
         """
         scenes = [x for x in self.config["scenes"]]
-        with open(".messenger/Templates/scene/Scenes/AllScenes.elm", "r") as f:
+        with open(".messenger/scene/AllScenes.elm", "r") as f:
             content = f.read()
         dol0 = "\n".join(
             [
                 f"import Scenes.{l}.Export as {l}\nimport Scenes.{l}.Global as {l}G"
                 for l in scenes
             ]
         )
@@ -57,15 +57,15 @@
         # Write
         with open("src/Scenes/AllScenes.elm", "w") as f:
             f.write(content)
 
         dol0 = "\n".join([f"import Scenes.{l}.Export as {l}" for l in scenes])
 
         dol1 = "\n    | ".join([f"{l}DataT {l}.Data" for l in scenes])
-        with open(".messenger/Templates/scene/Scenes/SceneSettings.elm", "r") as f:
+        with open(".messenger/scene/SceneSettings.elm", "r") as f:
             content = f.read()
         content = content.replace("$0", dol0).replace("$1", dol1)
         # Write
         with open("src/Scenes/SceneSettings.elm", "w") as f:
             f.write(content)
 
     def update_rep(self, file_proto, file_output, dollar, rep):
@@ -86,21 +86,21 @@
 
     def add_component(self, name: str):
         """
         Add a component
         """
         os.mkdir(f"src/Components/{name}")
         self.update_rep(
-            ".messenger/Templates/component/Components/Sample/Sample.elm",
+            ".messenger/component/Sample/Sample.elm",
             f"src/Components/{name}/{name}.elm",
             0,
             name,
         )
         self.update_rep(
-            ".messenger/Templates/component/Components/Sample/Export.elm",
+            ".messenger/component/Sample/Export.elm",
             f"src/Components/{name}/Export.elm",
             0,
             name,
         )
 
     def format(self):
         os.system("elm-format src/ --yes")
@@ -111,85 +111,85 @@
         """
         if scene not in self.config["scenes"]:
             raise Exception("Scene doesn't exist.")
         self.config["scenes"][scene].append(layer)
         self.dump_config()
         os.mkdir(f"src/Scenes/{scene}/{layer}")
         self.update_rep(
-            ".messenger/Templates/layer/Sample/Model.elm",
+            ".messenger/layer/Model.elm",
             f"src/Scenes/{scene}/{layer}/Model.elm",
             0,
             scene,
         )
         self.update_rep_next(
             f"src/Scenes/{scene}/{layer}/Model.elm",
             1,
             layer,
         )
         self.update_rep(
-            ".messenger/Templates/layer/Sample/Global.elm",
+            ".messenger/layer/Global.elm",
             f"src/Scenes/{scene}/{layer}/Global.elm",
             0,
             scene,
         )
         self.update_rep_next(
             f"src/Scenes/{scene}/{layer}/Global.elm",
             1,
             layer,
         )
         self.update_rep(
-            ".messenger/Templates/layer/Sample/Export.elm",
+            ".messenger/layer/Export.elm",
             f"src/Scenes/{scene}/{layer}/Export.elm",
             0,
             scene,
         )
         self.update_rep_next(
             f"src/Scenes/{scene}/{layer}/Export.elm",
             1,
             layer,
         )
         self.update_rep(
-            ".messenger/Templates/layer/Sample/Common.elm",
+            ".messenger/layer/Common.elm",
             f"src/Scenes/{scene}/{layer}/Common.elm",
             0,
             f"{scene}.{layer}",
         )
 
     def update_layers(self):
         """
         Update layer settings.
         """
         for scene in self.config["scenes"]:
             layers = self.config["scenes"][scene]
             self.update_rep(
-                ".messenger/Templates/scene/Scenes/Sample/Common.elm",
+                ".messenger/scene/Sample/Common.elm",
                 f"src/Scenes/{scene}/Common.elm",
                 0,
                 scene,
             )
             self.update_rep(
-                ".messenger/Templates/scene/Scenes/Sample/Export.elm",
+                ".messenger/scene/Sample/Export.elm",
                 f"src/Scenes/{scene}/Export.elm",
                 0,
                 scene,
             )
             self.update_rep(
-                ".messenger/Templates/scene/Scenes/Sample/Global.elm",
+                ".messenger/scene/Sample/Global.elm",
                 f"src/Scenes/{scene}/Global.elm",
                 0,
                 scene,
             )
             self.update_rep(
-                ".messenger/Templates/scene/Scenes/Sample/LayerBase.elm",
+                ".messenger/scene/Sample/LayerBase.elm",
                 f"src/Scenes/{scene}/LayerBase.elm",
                 0,
                 scene,
             )
             self.update_rep(
-                ".messenger/Templates/scene/Scenes/Sample/LayerSettings.elm",
+                ".messenger/scene/Sample/LayerSettings.elm",
                 f"src/Scenes/{scene}/LayerSettings.elm",
                 0,
                 scene,
             )
             self.update_rep_next(
                 f"src/Scenes/{scene}/LayerSettings.elm",
                 1,
@@ -197,15 +197,15 @@
             )
             self.update_rep_next(
                 f"src/Scenes/{scene}/LayerSettings.elm",
                 2,
                 "\n    | ".join([f"{l}Data {l}.Data" for l in layers]),
             )
             self.update_rep(
-                ".messenger/Templates/scene/Scenes/Sample/Model.elm",
+                ".messenger/scene/Sample/Model.elm",
                 f"src/Scenes/{scene}/Model.elm",
                 0,
                 scene,
             )
             self.update_rep_next(
                 f"src/Scenes/{scene}/Model.elm",
                 1,
@@ -247,30 +247,28 @@
 - Install the elm packages needed
 Press Enter to continue
 """
     )
     os.makedirs(name, exist_ok=True)
     os.chdir(name)
     os.system(
-        f"git clone -b templates https://github.com/linsyking/Messenger.git .messenger --depth=1"
+        f"git clone https://github.com/linsyking/messenger-templates .messenger --depth=1"
     )
-    shutil.copytree(".messenger/Templates/core/", "./src")
-    shutil.copytree(".messenger/Templates/public/", "./public")
-    shutil.copy(".messenger/Templates/.gitignore", "./.gitignore")
-    shutil.copy(".messenger/Templates/Makefile", "./Makefile")
-    shutil.copy(".messenger/Templates/elm.json", "./elm.json")
+    shutil.copytree(".messenger/core/", "./src")
+    shutil.copytree(".messenger/public/", "./public")
+    shutil.copy(".messenger/.gitignore", "./.gitignore")
+    shutil.copy(".messenger/Makefile", "./Makefile")
+    shutil.copy(".messenger/elm.json", "./elm.json")
 
     os.makedirs("src/Scenes", exist_ok=True)
     os.makedirs("assets", exist_ok=True)
     os.makedirs("src/Components", exist_ok=True)
 
     print("Creating elm.json...")
-    initObject = {
-        "scenes": {}
-    }
+    initObject = {"scenes": {}}
     with open("messenger.json", "w") as f:
         json.dump(initObject, f, indent=4, ensure_ascii=False)
     print("Installing dependencies...")
     os.system("elm make")
     print("Done!")
     print(f"Now please go to {name} and add scenes and components.")
```

