# Comparing `tmp/OncoAMBER-1.2.0.tar.gz` & `tmp/OncoAMBER-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OncoAMBER-1.2.0.tar", last modified: Thu May  4 19:47:57 2023, max compression
+gzip compressed data, was "OncoAMBER-1.2.1.tar", last modified: Thu May  4 20:50:26 2023, max compression
```

## Comparing `OncoAMBER-1.2.0.tar` & `OncoAMBER-1.2.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-05-04 19:47:57.678350 OncoAMBER-1.2.0/
-drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-05-04 19:47:57.600067 OncoAMBER-1.2.0/OncoAMBER.egg-info/
--rw-r--r--   0 louiskunz   (501) staff       (20)     2758 2023-05-04 19:47:57.000000 OncoAMBER-1.2.0/OncoAMBER.egg-info/PKG-INFO
--rw-r--r--   0 louiskunz   (501) staff       (20)      588 2023-05-04 19:47:57.000000 OncoAMBER-1.2.0/OncoAMBER.egg-info/SOURCES.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-05-04 19:47:57.000000 OncoAMBER-1.2.0/OncoAMBER.egg-info/dependency_links.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-04-21 16:40:31.000000 OncoAMBER-1.2.0/OncoAMBER.egg-info/not-zip-safe
--rw-r--r--   0 louiskunz   (501) staff       (20)       47 2023-05-04 19:47:57.000000 OncoAMBER-1.2.0/OncoAMBER.egg-info/requires.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)        6 2023-05-04 19:47:57.000000 OncoAMBER-1.2.0/OncoAMBER.egg-info/top_level.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)     2758 2023-05-04 19:47:57.678104 OncoAMBER-1.2.0/PKG-INFO
--rw-r--r--   0 louiskunz   (501) staff       (20)     2002 2023-04-27 16:58:04.000000 OncoAMBER-1.2.0/README.md
-drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-05-04 19:47:57.676799 OncoAMBER-1.2.0/amber/
--rw-r--r--   0 louiskunz   (501) staff       (20)     2239 2023-04-21 16:39:43.000000 OncoAMBER-1.2.0/amber/BasicGeometries.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     6028 2023-04-27 16:58:04.000000 OncoAMBER-1.2.0/amber/BetaDistributionCalibration.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     2055 2023-05-01 16:41:03.000000 OncoAMBER-1.2.0/amber/Cell.py
--rw-r--r--   0 louiskunz   (501) staff       (20)    22475 2023-05-04 19:20:45.000000 OncoAMBER-1.2.0/amber/Process.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     1606 2023-04-21 19:04:46.000000 OncoAMBER-1.2.0/amber/ReadAndWrite.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     3438 2023-04-21 16:39:43.000000 OncoAMBER-1.2.0/amber/ScalarField.py
--rw-r--r--   0 louiskunz   (501) staff       (20)      744 2023-04-21 16:39:43.000000 OncoAMBER-1.2.0/amber/Terminal.py
--rw-r--r--   0 louiskunz   (501) staff       (20)    14625 2023-05-04 19:06:01.000000 OncoAMBER-1.2.0/amber/Vessel.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     5571 2023-05-03 20:48:53.000000 OncoAMBER-1.2.0/amber/Voxel.py
--rw-r--r--   0 louiskunz   (501) staff       (20)    24068 2023-05-04 15:26:46.000000 OncoAMBER-1.2.0/amber/World.py
--rw-r--r--   0 louiskunz   (501) staff       (20)      308 2023-05-01 16:41:03.000000 OncoAMBER-1.2.0/amber/__init__.py
--rw-r--r--   0 louiskunz   (501) staff       (20)      211 2023-05-01 16:41:03.000000 OncoAMBER-1.2.0/amber/config.py
--rw-r--r--   0 louiskunz   (501) staff       (20)    17301 2023-04-21 16:39:43.000000 OncoAMBER-1.2.0/amber/save_alpha_dataframe6.csv
--rw-r--r--   0 louiskunz   (501) staff       (20)    17411 2023-04-21 16:39:43.000000 OncoAMBER-1.2.0/amber/save_beta_dataframe6.csv
--rw-r--r--   0 louiskunz   (501) staff       (20)       38 2023-05-04 19:47:57.678422 OncoAMBER-1.2.0/setup.cfg
--rw-r--r--   0 louiskunz   (501) staff       (20)     3010 2023-05-04 19:41:40.000000 OncoAMBER-1.2.0/setup.py
+drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-05-04 20:50:26.531339 OncoAMBER-1.2.1/
+drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-05-04 20:50:26.437125 OncoAMBER-1.2.1/OncoAMBER.egg-info/
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2758 2023-05-04 20:50:26.000000 OncoAMBER-1.2.1/OncoAMBER.egg-info/PKG-INFO
+-rw-r--r--   0 louiskunz   (501) staff       (20)      588 2023-05-04 20:50:26.000000 OncoAMBER-1.2.1/OncoAMBER.egg-info/SOURCES.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-05-04 20:50:26.000000 OncoAMBER-1.2.1/OncoAMBER.egg-info/dependency_links.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-04-21 16:40:31.000000 OncoAMBER-1.2.1/OncoAMBER.egg-info/not-zip-safe
+-rw-r--r--   0 louiskunz   (501) staff       (20)       47 2023-05-04 20:50:26.000000 OncoAMBER-1.2.1/OncoAMBER.egg-info/requires.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)        6 2023-05-04 20:50:26.000000 OncoAMBER-1.2.1/OncoAMBER.egg-info/top_level.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2758 2023-05-04 20:50:26.530945 OncoAMBER-1.2.1/PKG-INFO
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2002 2023-04-27 16:58:04.000000 OncoAMBER-1.2.1/README.md
+drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-05-04 20:50:26.529459 OncoAMBER-1.2.1/amber/
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2239 2023-04-21 16:39:43.000000 OncoAMBER-1.2.1/amber/BasicGeometries.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     6028 2023-04-27 16:58:04.000000 OncoAMBER-1.2.1/amber/BetaDistributionCalibration.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2055 2023-05-01 16:41:03.000000 OncoAMBER-1.2.1/amber/Cell.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)    22475 2023-05-04 19:20:45.000000 OncoAMBER-1.2.1/amber/Process.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     1606 2023-04-21 19:04:46.000000 OncoAMBER-1.2.1/amber/ReadAndWrite.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     3438 2023-04-21 16:39:43.000000 OncoAMBER-1.2.1/amber/ScalarField.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)      744 2023-04-21 16:39:43.000000 OncoAMBER-1.2.1/amber/Terminal.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)    14776 2023-05-04 20:49:39.000000 OncoAMBER-1.2.1/amber/Vessel.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     5571 2023-05-03 20:48:53.000000 OncoAMBER-1.2.1/amber/Voxel.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)    24068 2023-05-04 15:26:46.000000 OncoAMBER-1.2.1/amber/World.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)      308 2023-05-01 16:41:03.000000 OncoAMBER-1.2.1/amber/__init__.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)      211 2023-05-01 16:41:03.000000 OncoAMBER-1.2.1/amber/config.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)    17301 2023-04-21 16:39:43.000000 OncoAMBER-1.2.1/amber/save_alpha_dataframe6.csv
+-rw-r--r--   0 louiskunz   (501) staff       (20)    17411 2023-04-21 16:39:43.000000 OncoAMBER-1.2.1/amber/save_beta_dataframe6.csv
+-rw-r--r--   0 louiskunz   (501) staff       (20)       38 2023-05-04 20:50:26.531420 OncoAMBER-1.2.1/setup.cfg
+-rw-r--r--   0 louiskunz   (501) staff       (20)     3010 2023-05-04 20:50:19.000000 OncoAMBER-1.2.1/setup.py
```

### Comparing `OncoAMBER-1.2.0/OncoAMBER.egg-info/PKG-INFO` & `OncoAMBER-1.2.1/OncoAMBER.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OncoAMBER
-Version: 1.2.0
+Version: 1.2.1
 Summary: Agent-based model of tumor growth and response to radiation therapy
 Home-page: https://github.com/lvkunz/AMBER
 Author: Louis Kunz
 Author-email: lvkunz@mgh.harvard.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
```

### Comparing `OncoAMBER-1.2.0/OncoAMBER.egg-info/SOURCES.txt` & `OncoAMBER-1.2.1/OncoAMBER.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.0/PKG-INFO` & `OncoAMBER-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OncoAMBER
-Version: 1.2.0
+Version: 1.2.1
 Summary: Agent-based model of tumor growth and response to radiation therapy
 Home-page: https://github.com/lvkunz/AMBER
 Author: Louis Kunz
 Author-email: lvkunz@mgh.harvard.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
```

### Comparing `OncoAMBER-1.2.0/README.md` & `OncoAMBER-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.0/amber/BasicGeometries.py` & `OncoAMBER-1.2.1/amber/BasicGeometries.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.0/amber/BetaDistributionCalibration.py` & `OncoAMBER-1.2.1/amber/BetaDistributionCalibration.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.0/amber/Cell.py` & `OncoAMBER-1.2.1/amber/Cell.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.0/amber/Process.py` & `OncoAMBER-1.2.1/amber/Process.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.0/amber/ReadAndWrite.py` & `OncoAMBER-1.2.1/amber/ReadAndWrite.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.0/amber/ScalarField.py` & `OncoAMBER-1.2.1/amber/ScalarField.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.0/amber/Terminal.py` & `OncoAMBER-1.2.1/amber/Terminal.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.0/amber/Vessel.py` & `OncoAMBER-1.2.1/amber/Vessel.py`

 * *Files 2% similar despite different names*

```diff
@@ -265,19 +265,26 @@
         for vessel in self.list_of_vessels:
             vessel.plot(fig, ax, color)
         return fig, ax
 
 
     def grow_and_split(self, dt, splitting_rate, vegf_gradient, pressure, macro_steps=1, micro_steps=10, weight_direction=0.5, weight_vegf=0.5, weight_pressure=0.5):
         micro_steps = micro_steps
-        macro_steps = int(macro_steps * dt)
-        if macro_steps == 0:
+
+        macro_steps_ = int(macro_steps * dt)
+
+        if macro_steps_ == 0:
             ValueError("Macro steps must be at least 1")
-            macro_steps = 1
-        for i in range(macro_steps):
+            if macro_steps == 0:
+                ValueError("Angiogenesis deactivation")
+                macro_steps_ = 0
+            else:
+                macro_steps_ = 1
+
+        for i in range(macro_steps_):
             print("Macro step {}".format(i))
             j = 0
             for vessel in self.list_of_vessels:
                 splitting_rate_ = splitting_rate
                 if j % 1000 == 0: print('current number of vessels {}'.format(len(self.list_of_vessels)))
                 if vessel.in_growth:
                     total_path_length = vessel.step_size * micro_steps
```

### Comparing `OncoAMBER-1.2.0/amber/Voxel.py` & `OncoAMBER-1.2.1/amber/Voxel.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.0/amber/World.py` & `OncoAMBER-1.2.1/amber/World.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.0/amber/save_alpha_dataframe6.csv` & `OncoAMBER-1.2.1/amber/save_alpha_dataframe6.csv`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.0/amber/save_beta_dataframe6.csv` & `OncoAMBER-1.2.1/amber/save_beta_dataframe6.csv`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.0/setup.py` & `OncoAMBER-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # Package meta-data
 NAME = 'OncoAMBER'
 DESCRIPTION = 'Agent-based model of tumor growth and response to radiation therapy'
 URL = 'https://github.com/lvkunz/AMBER'
 EMAIL = 'lvkunz@mgh.harvard.edu'
 AUTHOR = 'Louis Kunz'
 REQUIRES_PYTHON = '>=3.8.2'
-VERSION = '1.2.0'
+VERSION = '1.2.1'
 
 # Required packages for this module to be executed
 REQUIRED = ['numpy', 'pandas', 'scipy']
 
 # Optional packages
 EXTRAS = { 'plots' :['matplotlib', 'seaborn'] }
```

