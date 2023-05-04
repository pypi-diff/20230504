# Comparing `tmp/pimgu-5.4.2023.2.tar.gz` & `tmp/pimgu-5.4.2023.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pimgu-5.4.2023.2.tar", last modified: Thu May  4 17:55:54 2023, max compression
+gzip compressed data, was "pimgu-5.4.2023.3.tar", last modified: Thu May  4 20:38:47 2023, max compression
```

## Comparing `pimgu-5.4.2023.2.tar` & `pimgu-5.4.2023.3.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 ianwilkey   (501) staff       (20)        0 2023-05-04 17:55:54.738504 pimgu-5.4.2023.2/
--rw-r--r--   0 ianwilkey   (501) staff       (20)     4243 2023-05-04 17:55:54.738250 pimgu-5.4.2023.2/PKG-INFO
--rw-r--r--   0 ianwilkey   (501) staff       (20)     3508 2023-05-04 17:31:36.000000 pimgu-5.4.2023.2/README.md
-drwxr-xr-x   0 ianwilkey   (501) staff       (20)        0 2023-05-04 17:55:54.736118 pimgu-5.4.2023.2/pimgu/
--rw-r--r--   0 ianwilkey   (501) staff       (20)      404 2023-05-04 17:10:13.000000 pimgu-5.4.2023.2/pimgu/__init__.py
--rw-r--r--   0 ianwilkey   (501) staff       (20)     7637 2023-05-04 17:07:14.000000 pimgu-5.4.2023.2/pimgu/applet.py
-drwxr-xr-x   0 ianwilkey   (501) staff       (20)        0 2023-05-04 17:55:54.737827 pimgu-5.4.2023.2/pimgu.egg-info/
--rw-r--r--   0 ianwilkey   (501) staff       (20)     4243 2023-05-04 17:55:54.000000 pimgu-5.4.2023.2/pimgu.egg-info/PKG-INFO
--rw-r--r--   0 ianwilkey   (501) staff       (20)      196 2023-05-04 17:55:54.000000 pimgu-5.4.2023.2/pimgu.egg-info/SOURCES.txt
--rw-r--r--   0 ianwilkey   (501) staff       (20)        1 2023-05-04 17:55:54.000000 pimgu-5.4.2023.2/pimgu.egg-info/dependency_links.txt
--rw-r--r--   0 ianwilkey   (501) staff       (20)       28 2023-05-04 17:55:54.000000 pimgu-5.4.2023.2/pimgu.egg-info/requires.txt
--rw-r--r--   0 ianwilkey   (501) staff       (20)        6 2023-05-04 17:55:54.000000 pimgu-5.4.2023.2/pimgu.egg-info/top_level.txt
--rw-r--r--   0 ianwilkey   (501) staff       (20)       38 2023-05-04 17:55:54.738611 pimgu-5.4.2023.2/setup.cfg
--rw-r--r--   0 ianwilkey   (501) staff       (20)     1085 2023-05-04 17:55:52.000000 pimgu-5.4.2023.2/setup.py
+drwxr-xr-x   0 ianwilkey   (501) staff       (20)        0 2023-05-04 20:38:47.376068 pimgu-5.4.2023.3/
+-rw-r--r--   0 ianwilkey   (501) staff       (20)     1067 2023-05-04 17:58:18.000000 pimgu-5.4.2023.3/LICENSE
+-rw-r--r--   0 ianwilkey   (501) staff       (20)     4265 2023-05-04 20:38:47.375658 pimgu-5.4.2023.3/PKG-INFO
+-rw-r--r--   0 ianwilkey   (501) staff       (20)     3508 2023-05-04 17:31:36.000000 pimgu-5.4.2023.3/README.md
+drwxr-xr-x   0 ianwilkey   (501) staff       (20)        0 2023-05-04 20:38:47.373113 pimgu-5.4.2023.3/pimgu/
+-rw-r--r--   0 ianwilkey   (501) staff       (20)      425 2023-05-04 20:38:00.000000 pimgu-5.4.2023.3/pimgu/__init__.py
+-rw-r--r--   0 ianwilkey   (501) staff       (20)     8989 2023-05-04 20:34:27.000000 pimgu-5.4.2023.3/pimgu/applet.py
+-rw-r--r--   0 ianwilkey   (501) staff       (20)     2479 2023-05-04 20:29:19.000000 pimgu-5.4.2023.3/pimgu/pimgl.py
+drwxr-xr-x   0 ianwilkey   (501) staff       (20)        0 2023-05-04 20:38:47.375027 pimgu-5.4.2023.3/pimgu.egg-info/
+-rw-r--r--   0 ianwilkey   (501) staff       (20)     4265 2023-05-04 20:38:47.000000 pimgu-5.4.2023.3/pimgu.egg-info/PKG-INFO
+-rw-r--r--   0 ianwilkey   (501) staff       (20)      219 2023-05-04 20:38:47.000000 pimgu-5.4.2023.3/pimgu.egg-info/SOURCES.txt
+-rw-r--r--   0 ianwilkey   (501) staff       (20)        1 2023-05-04 20:38:47.000000 pimgu-5.4.2023.3/pimgu.egg-info/dependency_links.txt
+-rw-r--r--   0 ianwilkey   (501) staff       (20)       28 2023-05-04 20:38:47.000000 pimgu-5.4.2023.3/pimgu.egg-info/requires.txt
+-rw-r--r--   0 ianwilkey   (501) staff       (20)        6 2023-05-04 20:38:47.000000 pimgu-5.4.2023.3/pimgu.egg-info/top_level.txt
+-rw-r--r--   0 ianwilkey   (501) staff       (20)       38 2023-05-04 20:38:47.376271 pimgu-5.4.2023.3/setup.cfg
+-rw-r--r--   0 ianwilkey   (501) staff       (20)     1085 2023-05-04 20:36:31.000000 pimgu-5.4.2023.3/setup.py
```

### Comparing `pimgu-5.4.2023.2/PKG-INFO` & `pimgu-5.4.2023.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: pimgu
-Version: 5.4.2023.2
+Version: 5.4.2023.3
 Summary: A simple framework for creating robust 2D GUI applications using Pygame and ImGui.
 Home-page: https://github.com/iwilkey/pimgu
 Author: Ian Wilkey
 Author-email: iwilkey@mail.bradley.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Pimgu
 
 Pimgu is a lightweight framework that combines the power of Pygame and ImGui to create intuitive and responsive 2D GUI applications. This framework provides an easy-to-use interface to build user interfaces while harnessing the capabilities of Pygame and ImGui under the hood.
 
 ## Features
```

### Comparing `pimgu-5.4.2023.2/README.md` & `pimgu-5.4.2023.3/README.md`

 * *Files identical despite different names*

### Comparing `pimgu-5.4.2023.2/pimgu/applet.py` & `pimgu-5.4.2023.3/pimgu/applet.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,22 +3,25 @@
 # Author: Ian Wilkey (iwilkey)
 # Copyright (C) 2023 Ian Wilkey. All Rights Reserved.
 # License: MIT.
 # Version: v05.04.2023
 ###################################################################################
 
 # Python standards.
-import sys
 import os
-from typing import List, Callable
+from typing import List, Callable, Tuple
 # Dependencies.
 import pygame as engine
-import OpenGL.GL as gl
+from OpenGL.GL import *
+from OpenGL.GLUT import *
+from OpenGL.GLU import *
 import imgui
 from imgui.integrations.pygame import PygameRenderer
+# For rendering Pygame surfaces with OpenGL.
+import pimgl
 
 version = "v05.04.2023"
 
 class Applet:
     """ Core framework for a Pimgu Applet. Supports robust, high-level tools for powerful 2D GUI applications.
     """
     
@@ -54,15 +57,23 @@
             # Load the icon image.
             icon = engine.image.load(self.__icon_path)
             # Set the icon of the window.
             engine.display.set_icon(icon)
         
         # Set up the screen.
         self.__screen : engine.Surface = engine.display.set_mode(self.__dimensions, engine.OPENGL | engine.DOUBLEBUF)
-    
+
+        # Set up OpenGL context.
+        glViewport(0, 0, self.__dimensions[0], self.__dimensions[1])
+        glMatrixMode(GL_PROJECTION)
+        glLoadIdentity()
+        gluOrtho2D(0, self.__dimensions[0], self.__dimensions[1], 0)
+        glMatrixMode(GL_MODELVIEW)
+        glLoadIdentity()
+        
         # Clear color.
         self.__cls_color : tuple = (0.1, 0.1, 0.1, 1)
 
         # Get clock object.
         self.__clock : engine.time.Clock = engine.time.Clock()
 
         #################
@@ -79,23 +90,25 @@
         self.__imgui_io.backend_flags |= imgui.BACKEND_HAS_MOUSE_CURSORS
         # Set up ImGui renderer.
         self.__imgui_renderer : PygameRenderer = PygameRenderer()
         
         #############
         # CALLBACKS #
         #############
-        
+
         # Callbacks during input processing stage.
         self.__input_callbacks : List[Callable] = []
         # Callbacks during GUI processing state.
         self.__imgui_callbacks : List[Callable] = []
         # Callbacks during render time (for Pygame).
-        self.__render_callbacks : List[Callable] = []
+        self.__render_callbacks : List[Callable[..., Tuple[engine.Surface, int, int]]] = []
         # Callbacks during tick time (before any rendering).
         self.__tick_callbacks : List[Callable] = []
+        # Called when the Pimgu application is closed.
+        self.__on_end_callback : Callable = None
         
         # Run the application.
         self.__running : bool = False
         
     def run(self):
         """ Runs the main loop of the application.
         """
@@ -112,18 +125,18 @@
             for callback in self.__tick_callbacks:
                 callback()
             # Clear the screen.
             self.__cls()
             # Render.
             self.__render()
             
+        self.__on_end_callback()
         self.__imgui_renderer.shutdown()
         engine.quit()
-        sys.exit()
-            
+        
     def __sync(self):
         """ Sync the engine to the target frame rate.
         """
         self.__clock.tick(self.__target_fps)
         
     def __process_events(self):
         """ Handle input for Pygame and ImGui.
@@ -146,26 +159,36 @@
         for callback in self.__imgui_callbacks:
             callback()
         imgui.end_frame()
         
     def __cls(self):
         """ Clear the GL color buffer.
         """
-        gl.glClearColor(self.__cls_color[0], self.__cls_color[1], self.__cls_color[2], self.__cls_color[3])
-        gl.glClear(gl.GL_COLOR_BUFFER_BIT)
+        glClearColor(self.__cls_color[0], self.__cls_color[1], self.__cls_color[2], self.__cls_color[3])
+        glClear(GL_COLOR_BUFFER_BIT | GL_DEPTH_BUFFER_BIT)
         
     def __render(self):
         """ Render the current state of the applet.
         """
+        
+        # Custom Pygame Surface render callbacks.
+        for callback in self.__render_callbacks:
+            try:
+                surface, cx, cy = callback()
+            except TypeError:
+                raise Exception("[PIMGU] When it is desired to draw a pygame surface to the screen, your callback must return: surface, center_x, center_y! See Pimgu examples on GitHub: https://github.com/iwilkey/pimgu.")
+            # Surface dimensions.
+            width, height = surface.get_size()
+            texture_id : int = pimgl.pygame_surface_to_opengl_texture(surface)
+            pimgl.draw_texture(texture_id, width, height, cx, cy)
+        
         # Draw ImGui data to renderer.
         imgui.render()
         self.__imgui_renderer.render(imgui.get_draw_data())
-        # Custom Pygame render callbacks.
-        for callback in self.__render_callbacks:
-            callback(screen = self.__screen)
+        
         # Flip the display color buffers to render.
         engine.display.flip()
         
     #############
     # REGISTERS #
     #############
             
@@ -175,23 +198,27 @@
         self.__input_callbacks.append(callback)
         
     def register_imgui_callback(self, callback : Callable):
         """ Register a callback to be called during Applet GUI processing.
         """
         self.__imgui_callbacks.append(callback)
 
-    def register_pygame_render_callback(self, callback : Callable):
+    def register_pygame_render_callback(self, callback : Callable[..., Tuple[engine.Surface, int, int]]):
         """ Register a callback to be called during Pygame render time.
         """
         self.__render_callbacks.append(callback)
         
     def register_tick_callback(self, callback : Callable):
         """ Regsiter a callback to be called during the Applet's tick stage (before rendering, after input.)
         """
         self.__tick_callbacks.append(callback)
+    def register_on_end_callback(self, callback : Callable):
+        """ Register a callback to occur when the application is terminated (running = False after running).
+        """
+        self.__on_end_callback = callback
     
     #######################
     # GETTERS AND SETTERS #
     #######################
     
     def get_title(self) -> str:
         return self.__title
```

### Comparing `pimgu-5.4.2023.2/pimgu.egg-info/PKG-INFO` & `pimgu-5.4.2023.3/pimgu.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: pimgu
-Version: 5.4.2023.2
+Version: 5.4.2023.3
 Summary: A simple framework for creating robust 2D GUI applications using Pygame and ImGui.
 Home-page: https://github.com/iwilkey/pimgu
 Author: Ian Wilkey
 Author-email: iwilkey@mail.bradley.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Pimgu
 
 Pimgu is a lightweight framework that combines the power of Pygame and ImGui to create intuitive and responsive 2D GUI applications. This framework provides an easy-to-use interface to build user interfaces while harnessing the capabilities of Pygame and ImGui under the hood.
 
 ## Features
```

### Comparing `pimgu-5.4.2023.2/setup.py` & `pimgu-5.4.2023.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pimgu',
-    version='v05.04.2023.2',
+    version='v05.04.2023.3',
     description='A simple framework for creating robust 2D GUI applications using Pygame and ImGui.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Ian Wilkey',
     author_email='iwilkey@mail.bradley.edu',
     url='https://github.com/iwilkey/pimgu',
     packages=find_packages(),
```

