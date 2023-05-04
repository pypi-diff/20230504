# Comparing `tmp/pimgu-5.4.2023.5.tar.gz` & `tmp/pimgu-5.4.2023.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pimgu-5.4.2023.5.tar", last modified: Thu May  4 20:56:37 2023, max compression
+gzip compressed data, was "pimgu-5.4.2023.6.tar", last modified: Thu May  4 20:59:52 2023, max compression
```

## Comparing `pimgu-5.4.2023.5.tar` & `pimgu-5.4.2023.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ianwilkey   (501) staff       (20)        0 2023-05-04 20:56:37.329893 pimgu-5.4.2023.5/
--rw-r--r--   0 ianwilkey   (501) staff       (20)     1067 2023-05-04 17:58:18.000000 pimgu-5.4.2023.5/LICENSE
--rw-r--r--   0 ianwilkey   (501) staff       (20)     4303 2023-05-04 20:56:37.329638 pimgu-5.4.2023.5/PKG-INFO
--rw-r--r--   0 ianwilkey   (501) staff       (20)     3546 2023-05-04 20:41:55.000000 pimgu-5.4.2023.5/README.md
-drwxr-xr-x   0 ianwilkey   (501) staff       (20)        0 2023-05-04 20:56:37.327519 pimgu-5.4.2023.5/pimgu/
--rw-r--r--   0 ianwilkey   (501) staff       (20)      404 2023-05-04 20:56:19.000000 pimgu-5.4.2023.5/pimgu/__init__.py
--rw-r--r--   0 ianwilkey   (501) staff       (20)    10888 2023-05-04 20:56:09.000000 pimgu-5.4.2023.5/pimgu/applet.py
-drwxr-xr-x   0 ianwilkey   (501) staff       (20)        0 2023-05-04 20:56:37.329195 pimgu-5.4.2023.5/pimgu.egg-info/
--rw-r--r--   0 ianwilkey   (501) staff       (20)     4303 2023-05-04 20:56:37.000000 pimgu-5.4.2023.5/pimgu.egg-info/PKG-INFO
--rw-r--r--   0 ianwilkey   (501) staff       (20)      204 2023-05-04 20:56:37.000000 pimgu-5.4.2023.5/pimgu.egg-info/SOURCES.txt
--rw-r--r--   0 ianwilkey   (501) staff       (20)        1 2023-05-04 20:56:37.000000 pimgu-5.4.2023.5/pimgu.egg-info/dependency_links.txt
--rw-r--r--   0 ianwilkey   (501) staff       (20)       28 2023-05-04 20:56:37.000000 pimgu-5.4.2023.5/pimgu.egg-info/requires.txt
--rw-r--r--   0 ianwilkey   (501) staff       (20)        6 2023-05-04 20:56:37.000000 pimgu-5.4.2023.5/pimgu.egg-info/top_level.txt
--rw-r--r--   0 ianwilkey   (501) staff       (20)       38 2023-05-04 20:56:37.330002 pimgu-5.4.2023.5/setup.cfg
--rw-r--r--   0 ianwilkey   (501) staff       (20)     1085 2023-05-04 20:56:24.000000 pimgu-5.4.2023.5/setup.py
+drwxr-xr-x   0 ianwilkey   (501) staff       (20)        0 2023-05-04 20:59:52.117250 pimgu-5.4.2023.6/
+-rw-r--r--   0 ianwilkey   (501) staff       (20)     1067 2023-05-04 17:58:18.000000 pimgu-5.4.2023.6/LICENSE
+-rw-r--r--   0 ianwilkey   (501) staff       (20)     4303 2023-05-04 20:59:52.116934 pimgu-5.4.2023.6/PKG-INFO
+-rw-r--r--   0 ianwilkey   (501) staff       (20)     3546 2023-05-04 20:41:55.000000 pimgu-5.4.2023.6/README.md
+drwxr-xr-x   0 ianwilkey   (501) staff       (20)        0 2023-05-04 20:59:52.114360 pimgu-5.4.2023.6/pimgu/
+-rw-r--r--   0 ianwilkey   (501) staff       (20)      404 2023-05-04 20:56:19.000000 pimgu-5.4.2023.6/pimgu/__init__.py
+-rw-r--r--   0 ianwilkey   (501) staff       (20)    11108 2023-05-04 20:59:27.000000 pimgu-5.4.2023.6/pimgu/applet.py
+drwxr-xr-x   0 ianwilkey   (501) staff       (20)        0 2023-05-04 20:59:52.116438 pimgu-5.4.2023.6/pimgu.egg-info/
+-rw-r--r--   0 ianwilkey   (501) staff       (20)     4303 2023-05-04 20:59:51.000000 pimgu-5.4.2023.6/pimgu.egg-info/PKG-INFO
+-rw-r--r--   0 ianwilkey   (501) staff       (20)      204 2023-05-04 20:59:52.000000 pimgu-5.4.2023.6/pimgu.egg-info/SOURCES.txt
+-rw-r--r--   0 ianwilkey   (501) staff       (20)        1 2023-05-04 20:59:51.000000 pimgu-5.4.2023.6/pimgu.egg-info/dependency_links.txt
+-rw-r--r--   0 ianwilkey   (501) staff       (20)       28 2023-05-04 20:59:51.000000 pimgu-5.4.2023.6/pimgu.egg-info/requires.txt
+-rw-r--r--   0 ianwilkey   (501) staff       (20)        6 2023-05-04 20:59:51.000000 pimgu-5.4.2023.6/pimgu.egg-info/top_level.txt
+-rw-r--r--   0 ianwilkey   (501) staff       (20)       38 2023-05-04 20:59:52.117389 pimgu-5.4.2023.6/setup.cfg
+-rw-r--r--   0 ianwilkey   (501) staff       (20)     1085 2023-05-04 20:59:39.000000 pimgu-5.4.2023.6/setup.py
```

### Comparing `pimgu-5.4.2023.5/LICENSE` & `pimgu-5.4.2023.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pimgu-5.4.2023.5/PKG-INFO` & `pimgu-5.4.2023.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pimgu
-Version: 5.4.2023.5
+Version: 5.4.2023.6
 Summary: A simple framework for creating robust 2D GUI applications using Pygame and ImGui.
 Home-page: https://github.com/iwilkey/pimgu
 Author: Ian Wilkey
 Author-email: iwilkey@mail.bradley.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pimgu-5.4.2023.5/README.md` & `pimgu-5.4.2023.6/README.md`

 * *Files identical despite different names*

### Comparing `pimgu-5.4.2023.5/pimgu/applet.py` & `pimgu-5.4.2023.6/pimgu/applet.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,26 +13,30 @@
 import pygame as engine
 from OpenGL.GL import *
 from OpenGL.GLUT import *
 from OpenGL.GLU import *
 import imgui
 from imgui.integrations.pygame import PygameRenderer
 
-version = "v05.04.2023"
+version = "v05.04.2023.6"
+
+#################################################
+# OpenGL Helper Methods to make our lives easier.
+#################################################
 
 def pygame_surface_to_opengl_texture(surface) -> int:
     """ Helper method that accepts a Pygame Surface object and converts it to an
     OpenGL texture that can be rendered by the Pimgu renderer.
     Args:
         surface (pygame.Surface): The surface to be rendered.
     Returns:
         texture_id: The OpenGL texture ID to be rendered.
     """
     width, height = surface.get_size()
-    texture_data = pygame.image.tostring(surface, "RGBA", 1)
+    texture_data = engine.image.tostring(surface, "RGBA", 1)
     texture_id : int = glGenTextures(1)
     glBindTexture(GL_TEXTURE_2D, texture_id)
     glTexParameteri(GL_TEXTURE_2D, GL_TEXTURE_MIN_FILTER, GL_LINEAR)
     glTexParameteri(GL_TEXTURE_2D, GL_TEXTURE_MAG_FILTER, GL_LINEAR)
     glTexImage2D(GL_TEXTURE_2D, 0, GL_RGBA, width, height, 0, GL_RGBA, GL_UNSIGNED_BYTE, texture_data)
     return texture_id
 
@@ -61,14 +65,18 @@
     glTexCoord2f(1, 0); glVertex3f(x2, y2, 0)
     glTexCoord2f(1, 1); glVertex3f(x3, y3, 0)
     glTexCoord2f(0, 1); glVertex3f(x4, y4, 0)
     glEnd()
 
     glDisable(GL_TEXTURE_2D)
 
+#####################
+# Pimgu Applet class.
+#####################
+
 class Applet:
     """ Core framework for a Pimgu Applet. Supports robust, high-level tools for powerful 2D GUI applications.
     """
     
     def __init__(self, title : str = "Pimgu Application", dimensions : tuple = (1280, 720), icon_path : str = "", **kwargs):
         """ Construct a new Pimgu Applet.\n
         Args:
```

### Comparing `pimgu-5.4.2023.5/pimgu.egg-info/PKG-INFO` & `pimgu-5.4.2023.6/pimgu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pimgu
-Version: 5.4.2023.5
+Version: 5.4.2023.6
 Summary: A simple framework for creating robust 2D GUI applications using Pygame and ImGui.
 Home-page: https://github.com/iwilkey/pimgu
 Author: Ian Wilkey
 Author-email: iwilkey@mail.bradley.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pimgu-5.4.2023.5/setup.py` & `pimgu-5.4.2023.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pimgu',
-    version='v05.04.2023.5',
+    version='v05.04.2023.6',
     description='A simple framework for creating robust 2D GUI applications using Pygame and ImGui.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Ian Wilkey',
     author_email='iwilkey@mail.bradley.edu',
     url='https://github.com/iwilkey/pimgu',
     packages=find_packages(),
```

