# Comparing `tmp/tortuemobile-0.5.tar.gz` & `tmp/tortuemobile-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tortuemobile-0.5.tar", last modified: Fri Apr 14 14:41:59 2023, max compression
+gzip compressed data, was "tortuemobile-0.5.1.tar", last modified: Thu May  4 13:55:09 2023, max compression
```

## Comparing `tortuemobile-0.5.tar` & `tortuemobile-0.5.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 14:41:59.139223 tortuemobile-0.5/
--rw-rw-rw-   0        0        0     1579 2023-04-14 12:52:47.000000 tortuemobile-0.5/LICENSE
--rw-rw-rw-   0        0        0       71 2023-04-14 13:42:33.000000 tortuemobile-0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     2491 2023-04-14 14:41:59.139223 tortuemobile-0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1852 2023-04-14 13:42:36.000000 tortuemobile-0.5/README.md
--rw-rw-rw-   0        0        0       74 2023-04-14 14:41:59.141226 tortuemobile-0.5/setup.cfg
--rw-rw-rw-   0        0        0      930 2023-04-14 14:41:24.000000 tortuemobile-0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:41:59.113224 tortuemobile-0.5/tortuemobile/
--rw-rw-rw-   0        0        0     6169 2023-04-14 14:31:15.000000 tortuemobile-0.5/tortuemobile/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:41:59.137250 tortuemobile-0.5/tortuemobile/tortuemobilejs/
--rw-rw-rw-   0        0        0   344396 2023-04-14 12:52:47.000000 tortuemobile-0.5/tortuemobile/tortuemobilejs/paper.js
--rw-rw-rw-   0        0        0    13299 2023-04-14 14:00:57.000000 tortuemobile-0.5/tortuemobile/tortuemobilejs/turtlewidget.js
-drwxrwxrwx   0        0        0        0 2023-04-14 14:41:59.131224 tortuemobile-0.5/tortuemobile.egg-info/
--rw-rw-rw-   0        0        0     2491 2023-04-14 14:41:59.000000 tortuemobile-0.5/tortuemobile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      333 2023-04-14 14:41:59.000000 tortuemobile-0.5/tortuemobile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 14:41:59.000000 tortuemobile-0.5/tortuemobile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-04-14 14:41:59.000000 tortuemobile-0.5/tortuemobile.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-14 14:41:59.000000 tortuemobile-0.5/tortuemobile.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 13:55:09.154471 tortuemobile-0.5.1/
+-rw-rw-rw-   0        0        0     1579 2023-04-14 12:52:47.000000 tortuemobile-0.5.1/LICENSE
+-rw-rw-rw-   0        0        0       71 2023-04-14 13:42:33.000000 tortuemobile-0.5.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2497 2023-05-04 13:55:09.154471 tortuemobile-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1856 2023-05-04 13:34:25.000000 tortuemobile-0.5.1/README.md
+-rw-rw-rw-   0        0        0       74 2023-05-04 13:55:09.156476 tortuemobile-0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0      932 2023-05-04 13:53:47.000000 tortuemobile-0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 13:55:09.137472 tortuemobile-0.5.1/tortuemobile/
+-rw-rw-rw-   0        0        0     6107 2023-05-04 13:37:03.000000 tortuemobile-0.5.1/tortuemobile/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 13:55:09.152472 tortuemobile-0.5.1/tortuemobile/tortuemobilejs/
+-rw-rw-rw-   0        0        0   344396 2023-04-14 12:52:47.000000 tortuemobile-0.5.1/tortuemobile/tortuemobilejs/paper.js
+-rw-rw-rw-   0        0        0    13306 2023-05-04 13:44:39.000000 tortuemobile-0.5.1/tortuemobile/tortuemobilejs/turtlewidget.js
+drwxrwxrwx   0        0        0        0 2023-05-04 13:55:09.148474 tortuemobile-0.5.1/tortuemobile.egg-info/
+-rw-rw-rw-   0        0        0     2497 2023-05-04 13:55:08.000000 tortuemobile-0.5.1/tortuemobile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2023-05-04 13:55:09.000000 tortuemobile-0.5.1/tortuemobile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 13:55:08.000000 tortuemobile-0.5.1/tortuemobile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-05-04 13:55:08.000000 tortuemobile-0.5.1/tortuemobile.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-04 13:55:08.000000 tortuemobile-0.5.1/tortuemobile.egg-info/top_level.txt
```

### Comparing `tortuemobile-0.5/LICENSE` & `tortuemobile-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tortuemobile-0.5/PKG-INFO` & `tortuemobile-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tortuemobile
-Version: 0.5
+Version: 0.5.1
 Summary: Un module pour les tortues dans les cahiers Jupyter.
 Home-page: https://github.com/callysto/tortuemobile
 Author: David Hay
 Author-email: misterhay@gmail.com
 Classifier: Framework :: IPython
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: BSD License
@@ -40,8 +40,8 @@
 |`t.cercle(rayon, degrÃ©s)`|faire dessiner Ã  la tortue un morceau de cercle de rayon Ã©gal Ã  un certain nombre de degrÃ©s|`t.cercle(40, 360)`|
 |`t.styloenhaut()`|ta tortue peut maintenant se dÃ©placer sans tracer des lignes|`t.styloenhaut()`|
 |`t.styloenbas()`|ta tortue trace Ã  nouveau des lignes|`t.styloenbas()`|
 |`t.couleurstylo('color')`|couleur de la ligne de votre tortue en utilisant un [nom de couleur](https://www.w3schools.com/colors/colors_names.asp)|`t.couleurstylo('blue')`|
 |`t.couleurstylo('rgb(R, V, B)')`|couleur de la ligne de votre tortue en utilisant valeurs de rouge, vert, et bleu de 0 Ã  255|`t.pencolor('rgb(0, 255, 100)')`|
 |`t.origine()`|remettre la tortue au centre de l'Ã©cran|`t.origine()`|
 |`t.position(x, y)`|dÃ©placer la tortue Ã  une position spÃ©cifique, (0,0) est en haut Ã  gauche et (400, 400) est en bas Ã  droite|`t.position(100, 250)`|
-|`t.cap(degrÃ©s)`|fixer le cap de la tortue Ã  un certain nombre de degrÃ©s|`t.cap(90)`|
+|`t.fixecap(degrÃ©s)`|fixer le cap de la tortue Ã  un certain nombre de degrÃ©s|`t.cap(90)`|
```

### Comparing `tortuemobile-0.5/README.md` & `tortuemobile-0.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 |`t.cercle(rayon, degrés)`|faire dessiner à la tortue un morceau de cercle de rayon égal à un certain nombre de degrés|`t.cercle(40, 360)`|
 |`t.styloenhaut()`|ta tortue peut maintenant se déplacer sans tracer des lignes|`t.styloenhaut()`|
 |`t.styloenbas()`|ta tortue trace à nouveau des lignes|`t.styloenbas()`|
 |`t.couleurstylo('color')`|couleur de la ligne de votre tortue en utilisant un [nom de couleur](https://www.w3schools.com/colors/colors_names.asp)|`t.couleurstylo('blue')`|
 |`t.couleurstylo('rgb(R, V, B)')`|couleur de la ligne de votre tortue en utilisant valeurs de rouge, vert, et bleu de 0 à 255|`t.pencolor('rgb(0, 255, 100)')`|
 |`t.origine()`|remettre la tortue au centre de l'écran|`t.origine()`|
 |`t.position(x, y)`|déplacer la tortue à une position spécifique, (0,0) est en haut à gauche et (400, 400) est en bas à droite|`t.position(100, 250)`|
-|`t.cap(degrés)`|fixer le cap de la tortue à un certain nombre de degrés|`t.cap(90)`|
+|`t.fixecap(degrés)`|fixer le cap de la tortue à un certain nombre de degrés|`t.cap(90)`|
```

### Comparing `tortuemobile-0.5/setup.py` & `tortuemobile-0.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from distutils.core import setup
 
 with open("README.md", "r") as f:
     readme = f.read()
 
 setup(name='tortuemobile',
-      version='0.5',
+      version='0.5.1',
       description='Un module pour les tortues dans les cahiers Jupyter.',
       long_description = readme,
       long_description_content_type='text/markdown',
       author='David Hay',
       author_email='misterhay@gmail.com',
       url='https://github.com/callysto/tortuemobile',
       packages=['tortuemobile'],
```

### Comparing `tortuemobile-0.5/tortuemobile/__init__.py` & `tortuemobile-0.5.1/tortuemobile/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,25 +2,23 @@
 import math
 
 from ipywidgets import widgets
 from notebook import nbextensions
 from traitlets import Unicode, List
 from IPython.display import display
 
-__version__ = '0.5'
+__version__ = '0.5.1'
 
 def install_js():
     pkgdir = os.path.dirname(__file__)
     nbextensions.install_nbextension(os.path.join(pkgdir, 'tortuemobilejs'), user=True)
 
 class Tortue(widgets.DOMWidget):
     _view_module = Unicode("nbextensions/tortuemobilejs/turtlewidget").tag(sync=True)
     _view_name = Unicode('TurtleView').tag(sync=True)
-    # TODO: Make this an eventful list, so we're not transferring the whole
-    # thing on every sync
     points = List(sync=True)
 
     SIZE = 400
     OFFSET = 20
     def __init__(self):
         '''Créer une tortue
 
@@ -71,27 +69,27 @@
         exemple::
 
             t.droite(90)
         '''
         self.cap += num
         self.cap = self.cap%360
         self.b_change = num
-        self._add_point()
+        self._ajoute_point()
 
     def gauche(self, num):
         '''Tourner lar tortue vers la gauche d'un certain nombre de degrés.
 
         exemple::
 
             t.gauche(90)
         '''
         self.cap -= num
         self.cap = self.cap%360
         self.b_change = -num
-        self._add_point()
+        self._ajoute_point()
 
     def avant(self, num):
         '''Faire avancer la tortue d'un certain nombre de pixels.
 
         exemple:
 
             t.avant(100)
@@ -106,15 +104,15 @@
 
         if self.posX > Tortue.SIZE - Tortue.OFFSET:
             self.posX = Tortue.SIZE - Tortue.OFFSET
         if self.posY > Tortue.SIZE - Tortue.OFFSET:
             self.posY = Tortue.SIZE - Tortue.OFFSET
 
         self.b_change = 0
-        self._add_point()
+        self._ajoute_point()
 
     def recule(self, num):
         '''Faire reculer la tortue d'un certain nombre de pixels.
 
         exemple::
 
             t.recule(100)
@@ -129,15 +127,15 @@
 
         if self.posX > Tortue.SIZE - Tortue.OFFSET:
             self.posX = Tortue.SIZE - Tortue.OFFSET
         if self.posY > Tortue.SIZE - Tortue.OFFSET:
             self.posY = Tortue.SIZE - Tortue.OFFSET
 
         self.b_change = 0
-        self._add_point()
+        self._ajoute_point()
 
     def couleurstylo(self, couleur):
         '''Modifier la couleur du stylo. Les noms des couleurs sont en anglais.
 
         exemple::
 
             t.couleurstylo("red")
@@ -150,34 +148,34 @@
         exemple::
 
             t.position(100, 100)
         """
         self.posX = x
         self.posY = y
         if capVar is None:
-            self._add_point()
+            self._ajoute_point()
         elif isinstance(capVar, int):
-            self.cap(capVar)
+            self.fixecap(capVar)
         else:
             raise ValueError("Le cap doit être un nombre entier")
 
-    def cap(self, capVar):
+    def fixecap(self, capVar):
         """Fixer le cap de la tortue à un certain nombre de degrés.
 
         exemple::
 
-            t.cap(180)
+            t.fixecap(180)
         """
         diff = self.cap - capVar
         self.b_change = diff
         self.cap = capVar
-        self._add_point()
+        self._ajoute_point()
         self.b_change = 0
 
-    def _add_point(self):
+    def _ajoute_point(self):
         p = dict(p=self.stylo, lc=self.couleur, x=self.posX, y=self.posY,
                  b=self.b_change, s=self.vitesseVar)
         self.points = self.points + [p]
 
     def cercle(self, radius, extent=360):
         """Faire dessiner à la tortue un morceau de cercle de rayon égal à un certain nombre de degrés.
         
@@ -188,22 +186,22 @@
             t.cercle(50, 180)
         """
         temp = self.cap
         self.b_change = 0;
         vitesseTemp = self.vitesseVar
         self.vitesseVar = 1
 
-        for i in range(0, (extent//2)):
+        for i in range(0, int(extent//2)):
             n = math.fabs(math.radians(self.b_change) * radius)
             if(radius >= 0):
-                self.forward(n)
-                self.left(2)
+                self.cercle(n)
+                self.gauche(2)
             else:
-                self.forward(n)
-                self.right(2)
+                self.cercle(n)
+                self.droite(2)
         if(radius >= 0):
             self.cap = (temp + extent)
         else:
             self.cap = (temp - extent)
         self.vitesseVar = vitesseTemp
 
     def origine(self):
@@ -216,8 +214,8 @@
         self.posX = 200
         self.posY = 200
         if 90 < self.cap <=270:
             self.b_change = - (self.cap - 90)
         else:
             self.b_change = 90 - self.cap
         self.cap = 90
-        self._add_point()
+        self._ajoute_point()
```

### Comparing `tortuemobile-0.5/tortuemobile/tortuemobilejs/paper.js` & `tortuemobile-0.5.1/tortuemobile/tortuemobilejs/paper.js`

 * *Files identical despite different names*

### Comparing `tortuemobile-0.5/tortuemobile/tortuemobilejs/turtlewidget.js` & `tortuemobile-0.5.1/tortuemobile/tortuemobilejs/turtlewidget.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -300,22 +300,22 @@
             toinsert.append(turtleArea);
 
             var buttonDiv = $('<div/>');
             buttonDiv.attr('target', 'button-area');
 
             // create help button 
             var helpButton = $('<button/>');
-            helpButton.append("Help!");
+            helpButton.append("Aider!");
             buttonDiv.append(helpButton);
 
             // create grid button  
             var gridButton = $('<button/>');
             gridButton.attr('id', 'grid-element');
             gridButton.attr('value', 0);
-            gridButton.append("Grid On/Off");
+            gridButton.append("Activer la grille");
             buttonDiv.append(gridButton);
             toinsert.append(buttonDiv);
 
             var canvasDiv = $('<div/>');
             toinsert.append(canvasDiv);
 
             var canvas = document.createElement('canvas');
```

### Comparing `tortuemobile-0.5/tortuemobile.egg-info/PKG-INFO` & `tortuemobile-0.5.1/tortuemobile.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tortuemobile
-Version: 0.5
+Version: 0.5.1
 Summary: Un module pour les tortues dans les cahiers Jupyter.
 Home-page: https://github.com/callysto/tortuemobile
 Author: David Hay
 Author-email: misterhay@gmail.com
 Classifier: Framework :: IPython
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: BSD License
@@ -40,8 +40,8 @@
 |`t.cercle(rayon, degrÃ©s)`|faire dessiner Ã  la tortue un morceau de cercle de rayon Ã©gal Ã  un certain nombre de degrÃ©s|`t.cercle(40, 360)`|
 |`t.styloenhaut()`|ta tortue peut maintenant se dÃ©placer sans tracer des lignes|`t.styloenhaut()`|
 |`t.styloenbas()`|ta tortue trace Ã  nouveau des lignes|`t.styloenbas()`|
 |`t.couleurstylo('color')`|couleur de la ligne de votre tortue en utilisant un [nom de couleur](https://www.w3schools.com/colors/colors_names.asp)|`t.couleurstylo('blue')`|
 |`t.couleurstylo('rgb(R, V, B)')`|couleur de la ligne de votre tortue en utilisant valeurs de rouge, vert, et bleu de 0 Ã  255|`t.pencolor('rgb(0, 255, 100)')`|
 |`t.origine()`|remettre la tortue au centre de l'Ã©cran|`t.origine()`|
 |`t.position(x, y)`|dÃ©placer la tortue Ã  une position spÃ©cifique, (0,0) est en haut Ã  gauche et (400, 400) est en bas Ã  droite|`t.position(100, 250)`|
-|`t.cap(degrÃ©s)`|fixer le cap de la tortue Ã  un certain nombre de degrÃ©s|`t.cap(90)`|
+|`t.fixecap(degrÃ©s)`|fixer le cap de la tortue Ã  un certain nombre de degrÃ©s|`t.cap(90)`|
```

