# Comparing `tmp/tupa123-1.4.7.tar.gz` & `tmp/tupa123-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tupa123-1.4.7.tar", last modified: Thu May  4 13:08:03 2023, max compression
+gzip compressed data, was "tupa123-1.4.8.tar", last modified: Thu May  4 14:49:46 2023, max compression
```

## Comparing `tupa123-1.4.7.tar` & `tupa123-1.4.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 13:08:03.540884 tupa123-1.4.7/
--rw-rw-rw-   0        0        0     1101 2023-03-27 13:05:36.000000 tupa123-1.4.7/LICENSE.txt
--rw-rw-rw-   0        0        0     2352 2023-05-04 13:08:03.540884 tupa123-1.4.7/PKG-INFO
--rw-rw-rw-   0        0        0     1876 2023-04-18 13:58:59.000000 tupa123-1.4.7/README.md
--rw-rw-rw-   0        0        0       42 2023-05-04 13:08:03.540884 tupa123-1.4.7/setup.cfg
--rw-rw-rw-   0        0        0      763 2023-05-04 13:06:55.000000 tupa123-1.4.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-04 13:08:03.528775 tupa123-1.4.7/tupa123/
--rw-rw-rw-   0        0        0       24 2023-03-27 17:38:15.000000 tupa123-1.4.7/tupa123/__init__.py
--rw-rw-rw-   0        0        0    74598 2023-05-04 13:00:12.000000 tupa123-1.4.7/tupa123/tupa123.py
-drwxrwxrwx   0        0        0        0 2023-05-04 13:08:03.538850 tupa123-1.4.7/tupa123.egg-info/
--rw-rw-rw-   0        0        0     2352 2023-05-04 13:08:03.000000 tupa123-1.4.7/tupa123.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-05-04 13:08:03.000000 tupa123-1.4.7/tupa123.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 13:08:03.000000 tupa123-1.4.7/tupa123.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-04 13:08:03.000000 tupa123-1.4.7/tupa123.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-04 13:08:03.000000 tupa123-1.4.7/tupa123.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 14:49:46.687133 tupa123-1.4.8/
+-rw-rw-rw-   0        0        0     1101 2023-03-27 13:05:36.000000 tupa123-1.4.8/LICENSE.txt
+-rw-rw-rw-   0        0        0     2352 2023-05-04 14:49:46.687133 tupa123-1.4.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1876 2023-04-18 13:58:59.000000 tupa123-1.4.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-04 14:49:46.687133 tupa123-1.4.8/setup.cfg
+-rw-rw-rw-   0        0        0      763 2023-05-04 14:49:10.000000 tupa123-1.4.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 14:49:46.655887 tupa123-1.4.8/tupa123/
+-rw-rw-rw-   0        0        0       24 2023-03-27 17:38:15.000000 tupa123-1.4.8/tupa123/__init__.py
+-rw-rw-rw-   0        0        0    75594 2023-05-04 14:46:14.000000 tupa123-1.4.8/tupa123/tupa123.py
+drwxrwxrwx   0        0        0        0 2023-05-04 14:49:46.671647 tupa123-1.4.8/tupa123.egg-info/
+-rw-rw-rw-   0        0        0     2352 2023-05-04 14:49:46.000000 tupa123-1.4.8/tupa123.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-05-04 14:49:46.000000 tupa123-1.4.8/tupa123.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 14:49:46.000000 tupa123-1.4.8/tupa123.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-04 14:49:46.000000 tupa123-1.4.8/tupa123.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-04 14:49:46.000000 tupa123-1.4.8/tupa123.egg-info/top_level.txt
```

### Comparing `tupa123-1.4.7/LICENSE.txt` & `tupa123-1.4.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tupa123-1.4.7/PKG-INFO` & `tupa123-1.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tupa123
-Version: 1.4.7
+Version: 1.4.8
 Summary: fully connected neural network with four layers
 Author: Leandro Schemmer
 Author-email: leandro.schemmer@gmail.com
 License: MIT
 Keywords: artificial-intelligence neural-networks four-layers regression regression-analysis classification-algorithms tupa123 deep-learning machine-learning data-science artificial-neural-network open-source
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `tupa123-1.4.7/README.md` & `tupa123-1.4.8/README.md`

 * *Files identical despite different names*

### Comparing `tupa123-1.4.7/setup.py` & `tupa123-1.4.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='tupa123',
-    version='1.4.7',
+    version='1.4.8',
     license = 'MIT',
     license_files=('LICENSE.txt',),    
     packages=['tupa123'],
     install_requires=['numpy','matplotlib','pandas'],    
     author='Leandro Schemmer',
     author_email='leandro.schemmer@gmail.com',
     description= 'fully connected neural network with four layers',
```

### Comparing `tupa123-1.4.7/tupa123/tupa123.py` & `tupa123-1.4.8/tupa123/tupa123.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,45 @@
         print('------ Only for classification 0 or 1 -----')
         print('')
         print('Number of hits for a maximum difference of 10% = ' + str(result) + '%' )
         print('')
 
 
 
+#Make basic comparative statistics between two sets of data
+def Statistics02(Calculated, Targeted, opt):
+    
+    numdata,numevar = Calculated.shape
+
+    erromedio = np.zeros((numevar))
+    desviopad = np.zeros((numevar))
+    maxerro = np.zeros((numevar))
+    coefcorrelacao = np.zeros((numevar))
+         
+    for j in range(0,numevar):
+        
+        erroari = Calculated[:,j] - Targeted[:,j]
+        
+        erromedio[j] = np.mean(erroari) #Mean difference, variable
+        desviopad[j] = np.std(erroari) #Standard deviation, variable         
+        maxerro[j] = np.max(abs(erroari)) #Biggest absolute point difference, variable
+        coefcorrelacao[j] = np.corrcoef(Targeted[:,j], Calculated[:,j])[1][0] #Correlation coefficient between Calculated and Target, variable
+        
+    if (opt==1):
+        return erromedio
+    if (opt==2):
+        return desviopad
+    if (opt==3):
+        return maxerro
+    if (opt==4):
+        return coefcorrelacao
+
+
+
+
 ###############################################################
 ###############################################################
 #########  Auxliar function to graphs   #######################
 ###############################################################
 ###############################################################
```

### Comparing `tupa123-1.4.7/tupa123.egg-info/PKG-INFO` & `tupa123-1.4.8/tupa123.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tupa123
-Version: 1.4.7
+Version: 1.4.8
 Summary: fully connected neural network with four layers
 Author: Leandro Schemmer
 Author-email: leandro.schemmer@gmail.com
 License: MIT
 Keywords: artificial-intelligence neural-networks four-layers regression regression-analysis classification-algorithms tupa123 deep-learning machine-learning data-science artificial-neural-network open-source
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

