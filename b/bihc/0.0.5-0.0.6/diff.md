# Comparing `tmp/bihc-0.0.5.tar.gz` & `tmp/bihc-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/edelafue/BIHC/dist/.tmp-4hn5advy/bihc-0.0.5.tar", last modified: Fri Apr 21 13:32:18 2023, max compression
+gzip compressed data, was "bihc-0.0.6.tar", last modified: Thu May  4 10:40:21 2023, max compression
```

## Comparing `bihc-0.0.5.tar` & `bihc-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 edelafue  (1000) edelafue  (1000)        0 2023-04-21 13:32:18.000000 bihc-0.0.5/
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)      760 2022-12-08 10:22:14.000000 bihc-0.0.5/LICENSE
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)      105 2022-12-08 10:22:14.000000 bihc-0.0.5/MANIFEST.in
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     3258 2023-04-21 13:32:18.000000 bihc-0.0.5/PKG-INFO
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     2686 2023-01-20 08:26:47.000000 bihc-0.0.5/README.md
-drwxrwxr-x   0 edelafue  (1000) edelafue  (1000)        0 2023-04-21 13:32:18.000000 bihc-0.0.5/bihc/
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)      172 2023-03-28 09:04:32.000000 bihc-0.0.5/bihc/__init__.py
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)    26817 2023-04-21 13:26:41.000000 bihc-0.0.5/bihc/beam.py
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     6251 2023-03-07 19:00:24.000000 bihc-0.0.5/bihc/impedance.py
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     9072 2023-03-28 09:16:31.000000 bihc-0.0.5/bihc/plot.py
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     4157 2023-03-08 15:02:48.000000 bihc-0.0.5/bihc/power.py
-drwxrwxr-x   0 edelafue  (1000) edelafue  (1000)        0 2023-04-21 13:32:18.000000 bihc-0.0.5/bihc.egg-info/
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     3258 2023-04-21 13:32:18.000000 bihc-0.0.5/bihc.egg-info/PKG-INFO
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)      334 2023-04-21 13:32:18.000000 bihc-0.0.5/bihc.egg-info/SOURCES.txt
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)        1 2023-04-21 13:32:18.000000 bihc-0.0.5/bihc.egg-info/dependency_links.txt
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)       23 2023-04-21 13:32:18.000000 bihc-0.0.5/bihc.egg-info/requires.txt
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)        5 2023-04-21 13:32:18.000000 bihc-0.0.5/bihc.egg-info/top_level.txt
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)      128 2022-12-16 15:42:39.000000 bihc-0.0.5/pyproject.toml
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)       38 2023-04-21 13:32:18.000000 bihc-0.0.5/setup.cfg
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     1080 2023-04-21 13:31:31.000000 bihc-0.0.5/setup.py
-drwxrwxr-x   0 edelafue  (1000) edelafue  (1000)        0 2023-04-21 13:32:18.000000 bihc-0.0.5/tests/
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     1886 2023-03-23 17:54:24.000000 bihc-0.0.5/tests/test_analyticBunchShapes.py
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     3008 2023-03-23 17:41:58.000000 bihc-0.0.5/tests/test_numericBunchShapes.py
+drwxrwxrwx   0 edelafue  (1000) edelafue  (1000)        0 2023-05-04 10:40:21.218445 bihc-0.0.6/
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)      760 2023-02-12 13:23:35.000000 bihc-0.0.6/LICENSE
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)      105 2023-02-12 13:23:35.000000 bihc-0.0.6/MANIFEST.in
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     3258 2023-05-04 10:40:21.202627 bihc-0.0.6/PKG-INFO
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     2686 2023-02-12 13:23:35.000000 bihc-0.0.6/README.md
+drwxrwxrwx   0 edelafue  (1000) edelafue  (1000)        0 2023-05-04 10:40:20.511503 bihc-0.0.6/bihc/
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)      172 2023-05-04 10:06:32.000000 bihc-0.0.6/bihc/__init__.py
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)    27006 2023-05-04 10:06:32.000000 bihc-0.0.6/bihc/beam.py
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     6251 2023-05-04 10:06:32.000000 bihc-0.0.6/bihc/impedance.py
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     9072 2023-05-04 10:06:32.000000 bihc-0.0.6/bihc/plot.py
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     4157 2023-05-04 10:06:32.000000 bihc-0.0.6/bihc/power.py
+drwxrwxrwx   0 edelafue  (1000) edelafue  (1000)        0 2023-05-04 10:40:20.919858 bihc-0.0.6/bihc.egg-info/
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     3258 2023-05-04 10:40:11.000000 bihc-0.0.6/bihc.egg-info/PKG-INFO
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)      334 2023-05-04 10:40:11.000000 bihc-0.0.6/bihc.egg-info/SOURCES.txt
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)        1 2023-05-04 10:40:11.000000 bihc-0.0.6/bihc.egg-info/dependency_links.txt
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)       23 2023-05-04 10:40:11.000000 bihc-0.0.6/bihc.egg-info/requires.txt
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)        5 2023-05-04 10:40:11.000000 bihc-0.0.6/bihc.egg-info/top_level.txt
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)      128 2023-02-12 13:23:36.000000 bihc-0.0.6/pyproject.toml
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)       38 2023-05-04 10:40:21.223967 bihc-0.0.6/setup.cfg
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     1080 2023-05-04 10:13:45.000000 bihc-0.0.6/setup.py
+drwxrwxrwx   0 edelafue  (1000) edelafue  (1000)        0 2023-05-04 10:40:21.079585 bihc-0.0.6/tests/
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     1886 2023-05-04 10:06:35.000000 bihc-0.0.6/tests/test_analyticBunchShapes.py
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     3008 2023-05-04 10:06:35.000000 bihc-0.0.6/tests/test_numericBunchShapes.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `bihc-0.0.5/LICENSE` & `bihc-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bihc-0.0.5/PKG-INFO` & `bihc-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bihc
-Version: 0.0.5
+Version: 0.0.6
 Summary: BIHC: Beam-Induced Heating Computation package
 Home-page: https://github.com/LeonardoSito/BIHC
 Author: Francesco Giordano
 Author-email: benoit.salvant@cern.ch
 Project-URL: Bug Tracker, https://github.com/LeonardoSito/BIHC/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bihc-0.0.5/README.md` & `bihc-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `bihc-0.0.5/bihc/beam.py` & `bihc-0.0.6/bihc/beam.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     fillMode : str, default 'FLATTOP'
         Timber label to extract data at a certain energy 'INJ', 'FLATTOP', 'STABLE'
     fillingScheme : list of bool, default [False]*3564
         Bool values to define the bunch filling scheme with length the number of buckets
     machine : str, default 'LHC'
         Name of the machine to operate with : 'PS', 'SPS', 'LHC'
     spectrum : str, default 'numeric'
-        Whether to calculate the spectrum with a numerical FFT 'numeric', or the analytical formula 'analytic'
+        Whether to calculate the spectrum with a numerical FFT 'numeric', from the analytical formula 'analytic', or from input 'user'
     realMachineLength : bool, default True
         Flag to adapt bucket size to real machine length
     ppbk : int, default 250
         Number of time samples per bucket
     frev : float, default None
         Revolution frequency in [Hz] to sample the analytic beam spectrum computation
     fmax : float, default 2e9
@@ -105,16 +105,16 @@
         self.Np = Np # Number of particles per bunch
         self.fillMode = fillMode
         self._fillNumber = fillNumber # Fill number relative to a particular fill of the machine
         
         self._isSpectrumReady = False
         self.isATimberFill    = False
         self.verbose = verbose 
-        self._machine=machine # Select the machine you are working with
-        self._spectrumtype=spectrum
+        self._machine = machine # Select the machine you are working with
+        self._spectrumtype = spectrum
         self.frev = frev
         self.fmax = fmax
 
         # Some parameters are set in a different way depending on the machine you are working with
         if self._machine == 'LHC':
             self.BUCKET_MAX = 3564
             RING_CIRCUMFERENCE = 26658.883   #[m]
@@ -228,14 +228,18 @@
             Beam spectrum in frequency. Returns the list of numpy arrays [frequency, spectrum]
         '''
         self.powerSpectrum = []
         if self._isSpectrumReady:
             [f,s] = self._spectrum
             self.powerSpectrum=[f, np.abs(s)**2]
             return self._spectrum
+
+        elif self._spectrumtype == 'user':
+            return self._spectrum #spectrum must be provided through the setter
+
         else:
     
             if self._spectrumtype == 'numeric':
                 [t,s]=self.longitudinalProfile
                 s=s/(self.filledSlots*self.J) #why is it normalized?
                 deltaT=t[10]-t[9] 
                 fc=1/deltaT                       #in frequency we have a periodic signal of period fc where fc is 1/deltaT where the sampling step
@@ -281,29 +285,30 @@
 
                 elif(self._bunchShape=='PARABOLIC'):
                     for p in progressbar(range(1,len(S)), "Computing analytic FFT: ", 20): 
                         CosSin=(np.sqrt(5)*sigmapar*p*wrev/c*np.cos(np.sqrt(5)*sigmapar*p*wrev/c)-np.sin(np.sqrt(5)*sigmapar*p*wrev/c))
                         lambdas[p]=-3*c**3/((np.sqrt(5)**3)*(sigmapar**3)*(p*wrev)**3)*CosSin
                         S[p]=np.abs(A*lambdas[p]*np.sum(an*np.exp(1j*p*wrev*n*t0)))
                 
-                f = np.linspace(1,len(S),len(S))*self.frev
+                f = np.linspace(1,len(S),len(S))*self.frev #[TODO] should it start in 0?
                 self.lambdas=[f, lambdas]
 
             if self.verbose:
                 print ('DC component: ', np.max(np.abs(S)))  
 
             self._spectrum=[f, np.abs(S)]
             self.powerSpectrum=[f, np.abs(S)**2]
-            self._isSpectrumReady=True
+            self._isSpectrumReady = True
             
             return self._spectrum
         
-    @spectrum.setter
-    def spectrum(self, newSpectrum): # TODO we want to assign the spectrum
+    #@spectrum.setter
+    def setSpectrum(self, newSpectrum): 
         self._spectrum = newSpectrum
+        self._isSpectrumReady = True
         #raise Exception("Spectrum can not be assigned")
                        
     def _setBunches(self):
         '''_setBunches method
 
         Computes the longitudinal profile of the bunches 
         with the shape specified in the class instance
```

### Comparing `bihc-0.0.5/bihc/impedance.py` & `bihc-0.0.6/bihc/impedance.py`

 * *Files identical despite different names*

### Comparing `bihc-0.0.5/bihc/plot.py` & `bihc-0.0.6/bihc/plot.py`

 * *Files identical despite different names*

### Comparing `bihc-0.0.5/bihc/power.py` & `bihc-0.0.6/bihc/power.py`

 * *Files identical despite different names*

### Comparing `bihc-0.0.5/bihc.egg-info/PKG-INFO` & `bihc-0.0.6/bihc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bihc
-Version: 0.0.5
+Version: 0.0.6
 Summary: BIHC: Beam-Induced Heating Computation package
 Home-page: https://github.com/LeonardoSito/BIHC
 Author: Francesco Giordano
 Author-email: benoit.salvant@cern.ch
 Project-URL: Bug Tracker, https://github.com/LeonardoSito/BIHC/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bihc-0.0.5/setup.py` & `bihc-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 #########
 # Setup #
 #########
 
 setup(
     name="bihc",
-    version="0.0.5",
+    version="0.0.6",
     description="BIHC: Beam-Induced Heating Computation package",
     author="Francesco Giordano",
     author_email="benoit.salvant@cern.ch", 
     packages=['bihc'],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LeonardoSito/BIHC",
```

### Comparing `bihc-0.0.5/tests/test_analyticBunchShapes.py` & `bihc-0.0.6/tests/test_analyticBunchShapes.py`

 * *Files identical despite different names*

### Comparing `bihc-0.0.5/tests/test_numericBunchShapes.py` & `bihc-0.0.6/tests/test_numericBunchShapes.py`

 * *Files identical despite different names*

