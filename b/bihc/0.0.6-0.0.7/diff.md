# Comparing `tmp/bihc-0.0.6.tar.gz` & `tmp/bihc-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bihc-0.0.6.tar", last modified: Thu May  4 10:40:21 2023, max compression
+gzip compressed data, was "bihc-0.0.7.tar", last modified: Thu May  4 17:45:57 2023, max compression
```

## Comparing `bihc-0.0.6.tar` & `bihc-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 edelafue  (1000) edelafue  (1000)        0 2023-05-04 10:40:21.218445 bihc-0.0.6/
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)      760 2023-02-12 13:23:35.000000 bihc-0.0.6/LICENSE
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)      105 2023-02-12 13:23:35.000000 bihc-0.0.6/MANIFEST.in
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     3258 2023-05-04 10:40:21.202627 bihc-0.0.6/PKG-INFO
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     2686 2023-02-12 13:23:35.000000 bihc-0.0.6/README.md
-drwxrwxrwx   0 edelafue  (1000) edelafue  (1000)        0 2023-05-04 10:40:20.511503 bihc-0.0.6/bihc/
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)      172 2023-05-04 10:06:32.000000 bihc-0.0.6/bihc/__init__.py
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)    27006 2023-05-04 10:06:32.000000 bihc-0.0.6/bihc/beam.py
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     6251 2023-05-04 10:06:32.000000 bihc-0.0.6/bihc/impedance.py
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     9072 2023-05-04 10:06:32.000000 bihc-0.0.6/bihc/plot.py
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     4157 2023-05-04 10:06:32.000000 bihc-0.0.6/bihc/power.py
-drwxrwxrwx   0 edelafue  (1000) edelafue  (1000)        0 2023-05-04 10:40:20.919858 bihc-0.0.6/bihc.egg-info/
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     3258 2023-05-04 10:40:11.000000 bihc-0.0.6/bihc.egg-info/PKG-INFO
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)      334 2023-05-04 10:40:11.000000 bihc-0.0.6/bihc.egg-info/SOURCES.txt
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)        1 2023-05-04 10:40:11.000000 bihc-0.0.6/bihc.egg-info/dependency_links.txt
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)       23 2023-05-04 10:40:11.000000 bihc-0.0.6/bihc.egg-info/requires.txt
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)        5 2023-05-04 10:40:11.000000 bihc-0.0.6/bihc.egg-info/top_level.txt
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)      128 2023-02-12 13:23:36.000000 bihc-0.0.6/pyproject.toml
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)       38 2023-05-04 10:40:21.223967 bihc-0.0.6/setup.cfg
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     1080 2023-05-04 10:13:45.000000 bihc-0.0.6/setup.py
-drwxrwxrwx   0 edelafue  (1000) edelafue  (1000)        0 2023-05-04 10:40:21.079585 bihc-0.0.6/tests/
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     1886 2023-05-04 10:06:35.000000 bihc-0.0.6/tests/test_analyticBunchShapes.py
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     3008 2023-05-04 10:06:35.000000 bihc-0.0.6/tests/test_numericBunchShapes.py
+drwxrwxrwx   0 edelafue  (1000) edelafue  (1000)        0 2023-05-04 17:45:57.087693 bihc-0.0.7/
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)      760 2023-05-04 17:43:24.000000 bihc-0.0.7/LICENSE
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)      105 2023-05-04 17:43:24.000000 bihc-0.0.7/MANIFEST.in
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     3258 2023-05-04 17:45:57.087693 bihc-0.0.7/PKG-INFO
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     2686 2023-05-04 17:43:24.000000 bihc-0.0.7/README.md
+drwxrwxrwx   0 edelafue  (1000) edelafue  (1000)        0 2023-05-04 17:45:56.728315 bihc-0.0.7/bihc/
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)      172 2023-05-04 17:43:24.000000 bihc-0.0.7/bihc/__init__.py
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)    27053 2023-05-04 17:44:37.000000 bihc-0.0.7/bihc/beam.py
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     6251 2023-05-04 17:43:24.000000 bihc-0.0.7/bihc/impedance.py
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     9072 2023-05-04 17:43:24.000000 bihc-0.0.7/bihc/plot.py
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     4157 2023-05-04 17:43:24.000000 bihc-0.0.7/bihc/power.py
+drwxrwxrwx   0 edelafue  (1000) edelafue  (1000)        0 2023-05-04 17:45:56.947067 bihc-0.0.7/bihc.egg-info/
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     3258 2023-05-04 17:45:56.000000 bihc-0.0.7/bihc.egg-info/PKG-INFO
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)      334 2023-05-04 17:45:56.000000 bihc-0.0.7/bihc.egg-info/SOURCES.txt
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)        1 2023-05-04 17:45:56.000000 bihc-0.0.7/bihc.egg-info/dependency_links.txt
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)       23 2023-05-04 17:45:56.000000 bihc-0.0.7/bihc.egg-info/requires.txt
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)        5 2023-05-04 17:45:56.000000 bihc-0.0.7/bihc.egg-info/top_level.txt
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)      128 2023-05-04 17:43:25.000000 bihc-0.0.7/pyproject.toml
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)       38 2023-05-04 17:45:57.087693 bihc-0.0.7/setup.cfg
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     1080 2023-05-04 17:43:58.000000 bihc-0.0.7/setup.py
+drwxrwxrwx   0 edelafue  (1000) edelafue  (1000)        0 2023-05-04 17:45:57.040827 bihc-0.0.7/tests/
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     1886 2023-05-04 17:43:26.000000 bihc-0.0.7/tests/test_analyticBunchShapes.py
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     3008 2023-05-04 17:43:26.000000 bihc-0.0.7/tests/test_numericBunchShapes.py
```

### Comparing `bihc-0.0.6/LICENSE` & `bihc-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bihc-0.0.6/PKG-INFO` & `bihc-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bihc
-Version: 0.0.6
+Version: 0.0.7
 Summary: BIHC: Beam-Induced Heating Computation package
 Home-page: https://github.com/LeonardoSito/BIHC
 Author: Francesco Giordano
 Author-email: benoit.salvant@cern.ch
 Project-URL: Bug Tracker, https://github.com/LeonardoSito/BIHC/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bihc-0.0.6/README.md` & `bihc-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `bihc-0.0.6/bihc/beam.py` & `bihc-0.0.7/bihc/beam.py`

 * *Files 1% similar despite different names*

```diff
@@ -340,14 +340,15 @@
                     sTemp=(1 - 4*((tTemp - self.phi[i])/(H))**2) #Binomial function (Francesco)
 
                     #set to zero the part of each bunch that is outside the l range arount his mean
                     mask=(np.abs(tTemp - self.phi[i]))<self.l
                     mask2=(sTemp>0)
                     sTemp=sTemp*mask2*mask
                     sTemp=2*(sTemp**self.exp)/H
+                    sTemp=np.sum(sTemp)*deltaD
                     profile_1_bunch = [tTemp, sTemp]
 
                 elif(self._bunchShape=='GAUSSIAN'):
                     sTemp=1/(self._bunchLength[i] * np.sqrt(2 * np.pi)) *(np.e)**(-((tTemp - self.phi[i])**2)/(2*self._bunchLength[i]**2))  #Gaussian function
                     mask=(np.abs(tTemp - self.phi[i]))<self.l
                     mask2=np.ones(len(sTemp))
                     sTemp=sTemp*mask2*mask
```

### Comparing `bihc-0.0.6/bihc/impedance.py` & `bihc-0.0.7/bihc/impedance.py`

 * *Files identical despite different names*

### Comparing `bihc-0.0.6/bihc/plot.py` & `bihc-0.0.7/bihc/plot.py`

 * *Files identical despite different names*

### Comparing `bihc-0.0.6/bihc/power.py` & `bihc-0.0.7/bihc/power.py`

 * *Files identical despite different names*

### Comparing `bihc-0.0.6/bihc.egg-info/PKG-INFO` & `bihc-0.0.7/bihc.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bihc
-Version: 0.0.6
+Version: 0.0.7
 Summary: BIHC: Beam-Induced Heating Computation package
 Home-page: https://github.com/LeonardoSito/BIHC
 Author: Francesco Giordano
 Author-email: benoit.salvant@cern.ch
 Project-URL: Bug Tracker, https://github.com/LeonardoSito/BIHC/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bihc-0.0.6/setup.py` & `bihc-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 #########
 # Setup #
 #########
 
 setup(
     name="bihc",
-    version="0.0.6",
+    version="0.0.7",
     description="BIHC: Beam-Induced Heating Computation package",
     author="Francesco Giordano",
     author_email="benoit.salvant@cern.ch", 
     packages=['bihc'],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LeonardoSito/BIHC",
```

### Comparing `bihc-0.0.6/tests/test_analyticBunchShapes.py` & `bihc-0.0.7/tests/test_analyticBunchShapes.py`

 * *Files identical despite different names*

### Comparing `bihc-0.0.6/tests/test_numericBunchShapes.py` & `bihc-0.0.7/tests/test_numericBunchShapes.py`

 * *Files identical despite different names*

