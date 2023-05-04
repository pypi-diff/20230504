# Comparing `tmp/bihc-0.0.7.1.tar.gz` & `tmp/bihc-0.0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bihc-0.0.7.1.tar", last modified: Thu May  4 18:00:59 2023, max compression
+gzip compressed data, was "bihc-0.0.7.2.tar", last modified: Thu May  4 18:03:51 2023, max compression
```

## Comparing `bihc-0.0.7.1.tar` & `bihc-0.0.7.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 edelafue  (1000) edelafue  (1000)        0 2023-05-04 18:00:59.819388 bihc-0.0.7.1/
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)      760 2023-05-04 17:43:24.000000 bihc-0.0.7.1/LICENSE
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)      105 2023-05-04 17:43:24.000000 bihc-0.0.7.1/MANIFEST.in
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     3260 2023-05-04 18:00:59.819388 bihc-0.0.7.1/PKG-INFO
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     2686 2023-05-04 17:43:24.000000 bihc-0.0.7.1/README.md
-drwxrwxrwx   0 edelafue  (1000) edelafue  (1000)        0 2023-05-04 18:00:59.458269 bihc-0.0.7.1/bihc/
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)      172 2023-05-04 17:43:24.000000 bihc-0.0.7.1/bihc/__init__.py
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)    27057 2023-05-04 17:58:51.000000 bihc-0.0.7.1/bihc/beam.py
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     6251 2023-05-04 17:43:24.000000 bihc-0.0.7.1/bihc/impedance.py
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     9072 2023-05-04 17:43:24.000000 bihc-0.0.7.1/bihc/plot.py
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     4157 2023-05-04 17:43:24.000000 bihc-0.0.7.1/bihc/power.py
-drwxrwxrwx   0 edelafue  (1000) edelafue  (1000)        0 2023-05-04 18:00:59.669078 bihc-0.0.7.1/bihc.egg-info/
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     3260 2023-05-04 18:00:58.000000 bihc-0.0.7.1/bihc.egg-info/PKG-INFO
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)      334 2023-05-04 18:00:59.000000 bihc-0.0.7.1/bihc.egg-info/SOURCES.txt
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)        1 2023-05-04 18:00:58.000000 bihc-0.0.7.1/bihc.egg-info/dependency_links.txt
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)       23 2023-05-04 18:00:58.000000 bihc-0.0.7.1/bihc.egg-info/requires.txt
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)        5 2023-05-04 18:00:58.000000 bihc-0.0.7.1/bihc.egg-info/top_level.txt
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)      128 2023-05-04 17:43:25.000000 bihc-0.0.7.1/pyproject.toml
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)       38 2023-05-04 18:00:59.819388 bihc-0.0.7.1/setup.cfg
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     1082 2023-05-04 18:00:29.000000 bihc-0.0.7.1/setup.py
-drwxrwxrwx   0 edelafue  (1000) edelafue  (1000)        0 2023-05-04 18:00:59.747220 bihc-0.0.7.1/tests/
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     1886 2023-05-04 17:43:26.000000 bihc-0.0.7.1/tests/test_analyticBunchShapes.py
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     3008 2023-05-04 17:43:26.000000 bihc-0.0.7.1/tests/test_numericBunchShapes.py
+drwxrwxrwx   0 edelafue  (1000) edelafue  (1000)        0 2023-05-04 18:03:51.873334 bihc-0.0.7.2/
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)      760 2023-05-04 17:43:24.000000 bihc-0.0.7.2/LICENSE
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)      105 2023-05-04 17:43:24.000000 bihc-0.0.7.2/MANIFEST.in
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     3260 2023-05-04 18:03:51.873334 bihc-0.0.7.2/PKG-INFO
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     2686 2023-05-04 17:43:24.000000 bihc-0.0.7.2/README.md
+drwxrwxrwx   0 edelafue  (1000) edelafue  (1000)        0 2023-05-04 18:03:51.512548 bihc-0.0.7.2/bihc/
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)      172 2023-05-04 17:43:24.000000 bihc-0.0.7.2/bihc/__init__.py
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)    27058 2023-05-04 18:03:15.000000 bihc-0.0.7.2/bihc/beam.py
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     6251 2023-05-04 17:43:24.000000 bihc-0.0.7.2/bihc/impedance.py
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     9072 2023-05-04 17:43:24.000000 bihc-0.0.7.2/bihc/plot.py
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     4157 2023-05-04 17:43:24.000000 bihc-0.0.7.2/bihc/power.py
+drwxrwxrwx   0 edelafue  (1000) edelafue  (1000)        0 2023-05-04 18:03:51.732705 bihc-0.0.7.2/bihc.egg-info/
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     3260 2023-05-04 18:03:50.000000 bihc-0.0.7.2/bihc.egg-info/PKG-INFO
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)      334 2023-05-04 18:03:51.000000 bihc-0.0.7.2/bihc.egg-info/SOURCES.txt
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)        1 2023-05-04 18:03:50.000000 bihc-0.0.7.2/bihc.egg-info/dependency_links.txt
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)       23 2023-05-04 18:03:50.000000 bihc-0.0.7.2/bihc.egg-info/requires.txt
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)        5 2023-05-04 18:03:50.000000 bihc-0.0.7.2/bihc.egg-info/top_level.txt
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)      128 2023-05-04 17:43:25.000000 bihc-0.0.7.2/pyproject.toml
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)       38 2023-05-04 18:03:51.873334 bihc-0.0.7.2/setup.cfg
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     1082 2023-05-04 18:03:28.000000 bihc-0.0.7.2/setup.py
+drwxrwxrwx   0 edelafue  (1000) edelafue  (1000)        0 2023-05-04 18:03:51.826455 bihc-0.0.7.2/tests/
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     1886 2023-05-04 17:43:26.000000 bihc-0.0.7.2/tests/test_analyticBunchShapes.py
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     3008 2023-05-04 17:43:26.000000 bihc-0.0.7.2/tests/test_numericBunchShapes.py
```

### Comparing `bihc-0.0.7.1/LICENSE` & `bihc-0.0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bihc-0.0.7.1/PKG-INFO` & `bihc-0.0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bihc
-Version: 0.0.7.1
+Version: 0.0.7.2
 Summary: BIHC: Beam-Induced Heating Computation package
 Home-page: https://github.com/LeonardoSito/BIHC
 Author: Francesco Giordano
 Author-email: benoit.salvant@cern.ch
 Project-URL: Bug Tracker, https://github.com/LeonardoSito/BIHC/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bihc-0.0.7.1/README.md` & `bihc-0.0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `bihc-0.0.7.1/bihc/beam.py` & `bihc-0.0.7.2/bihc/beam.py`

 * *Files 0% similar despite different names*

```diff
@@ -340,15 +340,15 @@
                     sTemp=(1 - 4*((tTemp - self.phi[i])/(H))**2) #Binomial function (Francesco)
 
                     #set to zero the part of each bunch that is outside the l range arount his mean
                     mask=(np.abs(tTemp - self.phi[i]))<self.l
                     mask2=(sTemp>0)
                     sTemp=sTemp*mask2*mask
                     sTemp=2*(sTemp**self.exp)/H
-                    Temp=sTemp/(sum(sTemp)*deltaD)
+                    sTemp=sTemp/(sum(sTemp)*deltaD)
                     profile_1_bunch = [tTemp, sTemp]
 
                 elif(self._bunchShape=='GAUSSIAN'):
                     sTemp=1/(self._bunchLength[i] * np.sqrt(2 * np.pi)) *(np.e)**(-((tTemp - self.phi[i])**2)/(2*self._bunchLength[i]**2))  #Gaussian function
                     mask=(np.abs(tTemp - self.phi[i]))<self.l
                     mask2=np.ones(len(sTemp))
                     sTemp=sTemp*mask2*mask
```

### Comparing `bihc-0.0.7.1/bihc/impedance.py` & `bihc-0.0.7.2/bihc/impedance.py`

 * *Files identical despite different names*

### Comparing `bihc-0.0.7.1/bihc/plot.py` & `bihc-0.0.7.2/bihc/plot.py`

 * *Files identical despite different names*

### Comparing `bihc-0.0.7.1/bihc/power.py` & `bihc-0.0.7.2/bihc/power.py`

 * *Files identical despite different names*

### Comparing `bihc-0.0.7.1/bihc.egg-info/PKG-INFO` & `bihc-0.0.7.2/bihc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bihc
-Version: 0.0.7.1
+Version: 0.0.7.2
 Summary: BIHC: Beam-Induced Heating Computation package
 Home-page: https://github.com/LeonardoSito/BIHC
 Author: Francesco Giordano
 Author-email: benoit.salvant@cern.ch
 Project-URL: Bug Tracker, https://github.com/LeonardoSito/BIHC/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bihc-0.0.7.1/setup.py` & `bihc-0.0.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 #########
 # Setup #
 #########
 
 setup(
     name="bihc",
-    version="0.0.7.1",
+    version="0.0.7.2",
     description="BIHC: Beam-Induced Heating Computation package",
     author="Francesco Giordano",
     author_email="benoit.salvant@cern.ch", 
     packages=['bihc'],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LeonardoSito/BIHC",
```

### Comparing `bihc-0.0.7.1/tests/test_analyticBunchShapes.py` & `bihc-0.0.7.2/tests/test_analyticBunchShapes.py`

 * *Files identical despite different names*

### Comparing `bihc-0.0.7.1/tests/test_numericBunchShapes.py` & `bihc-0.0.7.2/tests/test_numericBunchShapes.py`

 * *Files identical despite different names*

