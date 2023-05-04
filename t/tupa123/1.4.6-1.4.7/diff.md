# Comparing `tmp/tupa123-1.4.6.tar.gz` & `tmp/tupa123-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tupa123-1.4.6.tar", last modified: Wed May  3 11:37:41 2023, max compression
+gzip compressed data, was "tupa123-1.4.7.tar", last modified: Thu May  4 13:08:03 2023, max compression
```

## Comparing `tupa123-1.4.6.tar` & `tupa123-1.4.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 11:37:41.128047 tupa123-1.4.6/
--rw-rw-rw-   0        0        0     1101 2023-03-27 13:05:36.000000 tupa123-1.4.6/LICENSE.txt
--rw-rw-rw-   0        0        0     2352 2023-05-03 11:37:41.126693 tupa123-1.4.6/PKG-INFO
--rw-rw-rw-   0        0        0     1876 2023-04-18 13:58:59.000000 tupa123-1.4.6/README.md
--rw-rw-rw-   0        0        0       42 2023-05-03 11:37:41.128047 tupa123-1.4.6/setup.cfg
--rw-rw-rw-   0        0        0      763 2023-05-03 11:37:15.000000 tupa123-1.4.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:37:41.114946 tupa123-1.4.6/tupa123/
--rw-rw-rw-   0        0        0       24 2023-03-27 17:38:15.000000 tupa123-1.4.6/tupa123/__init__.py
--rw-rw-rw-   0        0        0    73652 2023-05-03 11:35:08.000000 tupa123-1.4.6/tupa123/tupa123.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:37:41.124666 tupa123-1.4.6/tupa123.egg-info/
--rw-rw-rw-   0        0        0     2352 2023-05-03 11:37:40.000000 tupa123-1.4.6/tupa123.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-05-03 11:37:41.000000 tupa123-1.4.6/tupa123.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 11:37:40.000000 tupa123-1.4.6/tupa123.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-03 11:37:40.000000 tupa123-1.4.6/tupa123.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-03 11:37:40.000000 tupa123-1.4.6/tupa123.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 13:08:03.540884 tupa123-1.4.7/
+-rw-rw-rw-   0        0        0     1101 2023-03-27 13:05:36.000000 tupa123-1.4.7/LICENSE.txt
+-rw-rw-rw-   0        0        0     2352 2023-05-04 13:08:03.540884 tupa123-1.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1876 2023-04-18 13:58:59.000000 tupa123-1.4.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-04 13:08:03.540884 tupa123-1.4.7/setup.cfg
+-rw-rw-rw-   0        0        0      763 2023-05-04 13:06:55.000000 tupa123-1.4.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 13:08:03.528775 tupa123-1.4.7/tupa123/
+-rw-rw-rw-   0        0        0       24 2023-03-27 17:38:15.000000 tupa123-1.4.7/tupa123/__init__.py
+-rw-rw-rw-   0        0        0    74598 2023-05-04 13:00:12.000000 tupa123-1.4.7/tupa123/tupa123.py
+drwxrwxrwx   0        0        0        0 2023-05-04 13:08:03.538850 tupa123-1.4.7/tupa123.egg-info/
+-rw-rw-rw-   0        0        0     2352 2023-05-04 13:08:03.000000 tupa123-1.4.7/tupa123.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-05-04 13:08:03.000000 tupa123-1.4.7/tupa123.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 13:08:03.000000 tupa123-1.4.7/tupa123.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-04 13:08:03.000000 tupa123-1.4.7/tupa123.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-04 13:08:03.000000 tupa123-1.4.7/tupa123.egg-info/top_level.txt
```

### Comparing `tupa123-1.4.6/LICENSE.txt` & `tupa123-1.4.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tupa123-1.4.6/PKG-INFO` & `tupa123-1.4.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tupa123
-Version: 1.4.6
+Version: 1.4.7
 Summary: fully connected neural network with four layers
 Author: Leandro Schemmer
 Author-email: leandro.schemmer@gmail.com
 License: MIT
 Keywords: artificial-intelligence neural-networks four-layers regression regression-analysis classification-algorithms tupa123 deep-learning machine-learning data-science artificial-neural-network open-source
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `tupa123-1.4.6/README.md` & `tupa123-1.4.7/README.md`

 * *Files identical despite different names*

### Comparing `tupa123-1.4.6/setup.py` & `tupa123-1.4.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='tupa123',
-    version='1.4.6',
+    version='1.4.7',
     license = 'MIT',
     license_files=('LICENSE.txt',),    
     packages=['tupa123'],
     install_requires=['numpy','matplotlib','pandas'],    
     author='Leandro Schemmer',
     author_email='leandro.schemmer@gmail.com',
     description= 'fully connected neural network with four layers',
```

### Comparing `tupa123-1.4.6/tupa123/tupa123.py` & `tupa123-1.4.7/tupa123/tupa123.py`

 * *Files 0% similar despite different names*

```diff
@@ -1949,8 +1949,39 @@
             plt.xlabel('Study data')
             plt.ylabel('Error, mse')
             plt.plot(eixoX, eixoY, marker = '', color = 'darkblue')  
             plt.show()
 
 
 
+
+
+###############################################################
+###############################################################
+################ Auxliliar calculation   ######################
+###############################################################
+###############################################################
+
+
+    #Mean squared error  ----------------------------------------------------------
+    def MSE(self):
+
+        if (self.sbw==1):
+            
+            #ajuste do local de salvamento, se especificado
+            if (self.namenet==''):
+                nomepasta=''
+            else:
+                nomepasta = self.namenet + '/'
+
+            
+            #grafico da convergencia
+            Conve = np.load(nomepasta + "Convergencia.npy")
+            tamanho = len(Conve)
+        
+            MenorErro = np.min(Conve)
+            itemenorerro = Conve[0]
+
+            return MenorErro
+
+
```

### Comparing `tupa123-1.4.6/tupa123.egg-info/PKG-INFO` & `tupa123-1.4.7/tupa123.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tupa123
-Version: 1.4.6
+Version: 1.4.7
 Summary: fully connected neural network with four layers
 Author: Leandro Schemmer
 Author-email: leandro.schemmer@gmail.com
 License: MIT
 Keywords: artificial-intelligence neural-networks four-layers regression regression-analysis classification-algorithms tupa123 deep-learning machine-learning data-science artificial-neural-network open-source
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

