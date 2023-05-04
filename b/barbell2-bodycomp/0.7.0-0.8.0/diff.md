# Comparing `tmp/barbell2_bodycomp-0.7.0.tar.gz` & `tmp/barbell2_bodycomp-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "barbell2_bodycomp-0.7.0.tar", last modified: Tue Apr 25 13:13:12 2023, max compression
+gzip compressed data, was "dist/barbell2_bodycomp-0.8.0.tar", last modified: Thu May  4 07:25:52 2023, max compression
```

## Comparing `barbell2_bodycomp-0.7.0.tar` & `barbell2_bodycomp-0.8.0.tar`

### file list

```diff
@@ -1,33 +1,32 @@
-drwxr-xr-x   0 Ralph      (501) staff       (20)        0 2023-04-25 13:13:12.623622 barbell2_bodycomp-0.7.0/
--rw-r--r--   0 Ralph      (501) staff       (20)      791 2023-04-25 13:13:12.623184 barbell2_bodycomp-0.7.0/PKG-INFO
-drwxr-xr-x   0 Ralph      (501) staff       (20)        0 2023-04-25 13:13:12.616157 barbell2_bodycomp-0.7.0/barbell2_bodycomp/
--rw-r--r--   0 Ralph      (501) staff       (20)      392 2023-04-25 13:13:08.000000 barbell2_bodycomp-0.7.0/barbell2_bodycomp/__init__.py
--rw-r--r--   0 Ralph      (501) staff       (20)     4447 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.7.0/barbell2_bodycomp/calculator.py
-drwxr-xr-x   0 Ralph      (501) staff       (20)        0 2023-04-25 13:13:12.622032 barbell2_bodycomp-0.7.0/barbell2_bodycomp/convert/
--rw-r--r--   0 Ralph      (501) staff       (20)      403 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.7.0/barbell2_bodycomp/convert/__init__.py
--rw-r--r--   0 Ralph      (501) staff       (20)     2200 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.7.0/barbell2_bodycomp/convert/dcm2nifti.py
--rw-r--r--   0 Ralph      (501) staff       (20)     1485 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.7.0/barbell2_bodycomp/convert/dcm2npy.py
--rw-r--r--   0 Ralph      (501) staff       (20)      558 2023-04-25 11:30:39.000000 barbell2_bodycomp-0.7.0/barbell2_bodycomp/convert/dcm2raw.py
--rw-r--r--   0 Ralph      (501) staff       (20)     1405 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.7.0/barbell2_bodycomp/convert/npy2dcm.py
--rw-r--r--   0 Ralph      (501) staff       (20)      853 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.7.0/barbell2_bodycomp/convert/npy2nrrd.py
--rw-r--r--   0 Ralph      (501) staff       (20)     2030 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.7.0/barbell2_bodycomp/convert/npy2png.py
--rw-r--r--   0 Ralph      (501) staff       (20)     1059 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.7.0/barbell2_bodycomp/convert/tag2dcm.py
--rw-r--r--   0 Ralph      (501) staff       (20)      435 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.7.0/barbell2_bodycomp/convert/tag2npy.py
-drwxr-xr-x   0 Ralph      (501) staff       (20)        0 2023-04-25 13:13:12.622671 barbell2_bodycomp-0.7.0/barbell2_bodycomp/pipeline/
--rw-r--r--   0 Ralph      (501) staff       (20)        0 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.7.0/barbell2_bodycomp/pipeline/__init__.py
--rw-r--r--   0 Ralph      (501) staff       (20)     6132 2023-04-25 12:54:52.000000 barbell2_bodycomp-0.7.0/barbell2_bodycomp/pipeline/bodycomp.py
--rw-r--r--   0 Ralph      (501) staff       (20)     6054 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.7.0/barbell2_bodycomp/seg.py
--rw-r--r--   0 Ralph      (501) staff       (20)     1394 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.7.0/barbell2_bodycomp/selectroi.py
--rw-r--r--   0 Ralph      (501) staff       (20)     5804 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.7.0/barbell2_bodycomp/selectslice.py
--rw-r--r--   0 Ralph      (501) staff       (20)     1586 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.7.0/barbell2_bodycomp/totalseg.py
--rw-r--r--   0 Ralph      (501) staff       (20)     6246 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.7.0/barbell2_bodycomp/utils.py
-drwxr-xr-x   0 Ralph      (501) staff       (20)        0 2023-04-25 13:13:12.619478 barbell2_bodycomp-0.7.0/barbell2_bodycomp.egg-info/
--rw-r--r--   0 Ralph      (501) staff       (20)      791 2023-04-25 13:13:12.000000 barbell2_bodycomp-0.7.0/barbell2_bodycomp.egg-info/PKG-INFO
--rw-r--r--   0 Ralph      (501) staff       (20)      919 2023-04-25 13:13:12.000000 barbell2_bodycomp-0.7.0/barbell2_bodycomp.egg-info/SOURCES.txt
--rw-r--r--   0 Ralph      (501) staff       (20)        1 2023-04-25 13:13:12.000000 barbell2_bodycomp-0.7.0/barbell2_bodycomp.egg-info/dependency_links.txt
--rw-r--r--   0 Ralph      (501) staff       (20)       20 2023-04-25 13:13:12.000000 barbell2_bodycomp-0.7.0/barbell2_bodycomp.egg-info/entry_points.txt
--rw-r--r--   0 Ralph      (501) staff       (20)        1 2023-04-18 13:15:18.000000 barbell2_bodycomp-0.7.0/barbell2_bodycomp.egg-info/not-zip-safe
--rw-r--r--   0 Ralph      (501) staff       (20)       68 2023-04-25 13:13:12.000000 barbell2_bodycomp-0.7.0/barbell2_bodycomp.egg-info/requires.txt
--rw-r--r--   0 Ralph      (501) staff       (20)       18 2023-04-25 13:13:12.000000 barbell2_bodycomp-0.7.0/barbell2_bodycomp.egg-info/top_level.txt
--rw-r--r--   0 Ralph      (501) staff       (20)       38 2023-04-25 13:13:12.623708 barbell2_bodycomp-0.7.0/setup.cfg
--rw-r--r--   0 Ralph      (501) staff       (20)     1456 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.7.0/setup.py
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-05-04 07:25:52.582934 barbell2_bodycomp-0.8.0/
+-rw-r--r--   0 ralph      (501) staff       (20)      763 2023-05-04 07:25:52.582629 barbell2_bodycomp-0.8.0/PKG-INFO
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-05-04 07:25:52.577407 barbell2_bodycomp-0.8.0/barbell2_bodycomp/
+-rw-r--r--   0 ralph      (501) staff       (20)      392 2023-05-04 07:25:47.000000 barbell2_bodycomp-0.8.0/barbell2_bodycomp/__init__.py
+-rw-r--r--   0 ralph      (501) staff       (20)     4447 2023-04-15 10:49:32.000000 barbell2_bodycomp-0.8.0/barbell2_bodycomp/calculator.py
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-05-04 07:25:52.581910 barbell2_bodycomp-0.8.0/barbell2_bodycomp/convert/
+-rw-r--r--   0 ralph      (501) staff       (20)      403 2023-04-13 11:54:27.000000 barbell2_bodycomp-0.8.0/barbell2_bodycomp/convert/__init__.py
+-rw-r--r--   0 ralph      (501) staff       (20)     2200 2023-04-13 10:16:54.000000 barbell2_bodycomp-0.8.0/barbell2_bodycomp/convert/dcm2nifti.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1485 2023-04-13 10:26:30.000000 barbell2_bodycomp-0.8.0/barbell2_bodycomp/convert/dcm2npy.py
+-rw-r--r--   0 ralph      (501) staff       (20)      558 2023-05-04 07:15:35.000000 barbell2_bodycomp-0.8.0/barbell2_bodycomp/convert/dcm2raw.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1405 2023-04-13 10:39:19.000000 barbell2_bodycomp-0.8.0/barbell2_bodycomp/convert/npy2dcm.py
+-rw-r--r--   0 ralph      (501) staff       (20)      853 2023-04-13 10:16:54.000000 barbell2_bodycomp-0.8.0/barbell2_bodycomp/convert/npy2nrrd.py
+-rw-r--r--   0 ralph      (501) staff       (20)     2030 2023-04-13 10:40:43.000000 barbell2_bodycomp-0.8.0/barbell2_bodycomp/convert/npy2png.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1059 2023-04-13 10:41:23.000000 barbell2_bodycomp-0.8.0/barbell2_bodycomp/convert/tag2dcm.py
+-rw-r--r--   0 ralph      (501) staff       (20)      435 2023-04-13 10:41:41.000000 barbell2_bodycomp-0.8.0/barbell2_bodycomp/convert/tag2npy.py
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-05-04 07:25:52.582304 barbell2_bodycomp-0.8.0/barbell2_bodycomp/pipeline/
+-rw-r--r--   0 ralph      (501) staff       (20)        0 2023-04-13 11:55:38.000000 barbell2_bodycomp-0.8.0/barbell2_bodycomp/pipeline/__init__.py
+-rw-r--r--   0 ralph      (501) staff       (20)     6132 2023-05-04 07:15:35.000000 barbell2_bodycomp-0.8.0/barbell2_bodycomp/pipeline/bodycomp.py
+-rw-r--r--   0 ralph      (501) staff       (20)     6064 2023-05-04 07:25:10.000000 barbell2_bodycomp-0.8.0/barbell2_bodycomp/seg.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1394 2023-04-13 12:19:43.000000 barbell2_bodycomp-0.8.0/barbell2_bodycomp/selectroi.py
+-rw-r--r--   0 ralph      (501) staff       (20)     5804 2023-04-13 12:19:18.000000 barbell2_bodycomp-0.8.0/barbell2_bodycomp/selectslice.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1586 2023-04-13 11:15:28.000000 barbell2_bodycomp-0.8.0/barbell2_bodycomp/totalseg.py
+-rw-r--r--   0 ralph      (501) staff       (20)     6246 2023-04-13 10:17:39.000000 barbell2_bodycomp-0.8.0/barbell2_bodycomp/utils.py
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-05-04 07:25:52.579095 barbell2_bodycomp-0.8.0/barbell2_bodycomp.egg-info/
+-rw-r--r--   0 ralph      (501) staff       (20)      763 2023-05-04 07:25:52.000000 barbell2_bodycomp-0.8.0/barbell2_bodycomp.egg-info/PKG-INFO
+-rw-r--r--   0 ralph      (501) staff       (20)      875 2023-05-04 07:25:52.000000 barbell2_bodycomp-0.8.0/barbell2_bodycomp.egg-info/SOURCES.txt
+-rw-r--r--   0 ralph      (501) staff       (20)        1 2023-05-04 07:25:52.000000 barbell2_bodycomp-0.8.0/barbell2_bodycomp.egg-info/dependency_links.txt
+-rw-r--r--   0 ralph      (501) staff       (20)        1 2023-04-13 10:43:22.000000 barbell2_bodycomp-0.8.0/barbell2_bodycomp.egg-info/not-zip-safe
+-rw-r--r--   0 ralph      (501) staff       (20)       68 2023-05-04 07:25:52.000000 barbell2_bodycomp-0.8.0/barbell2_bodycomp.egg-info/requires.txt
+-rw-r--r--   0 ralph      (501) staff       (20)       18 2023-05-04 07:25:52.000000 barbell2_bodycomp-0.8.0/barbell2_bodycomp.egg-info/top_level.txt
+-rw-r--r--   0 ralph      (501) staff       (20)       38 2023-05-04 07:25:52.583011 barbell2_bodycomp-0.8.0/setup.cfg
+-rw-r--r--   0 ralph      (501) staff       (20)     1456 2023-04-13 12:44:51.000000 barbell2_bodycomp-0.8.0/setup.py
```

### Comparing `barbell2_bodycomp-0.7.0/PKG-INFO` & `barbell2_bodycomp-0.8.0/barbell2_bodycomp.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 Metadata-Version: 2.1
-Name: barbell2_bodycomp
-Version: 0.7.0
+Name: barbell2-bodycomp
+Version: 0.8.0
 Summary: components for command-line body composition analysis
 Home-page: https://github.com/rbrecheisen/barbell2_bodycomp
 Author: Ralph Brecheisen
 Author-email: r.brecheisen@maastrichtuniversity.nl
 License: MIT license
 Keywords: barbell2_bodycomp
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.5
-
-UNKNOWN
-
```

### Comparing `barbell2_bodycomp-0.7.0/barbell2_bodycomp/calculator.py` & `barbell2_bodycomp-0.8.0/barbell2_bodycomp/calculator.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.7.0/barbell2_bodycomp/convert/dcm2nifti.py` & `barbell2_bodycomp-0.8.0/barbell2_bodycomp/convert/dcm2nifti.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.7.0/barbell2_bodycomp/convert/dcm2npy.py` & `barbell2_bodycomp-0.8.0/barbell2_bodycomp/convert/dcm2npy.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.7.0/barbell2_bodycomp/convert/dcm2raw.py` & `barbell2_bodycomp-0.8.0/barbell2_bodycomp/convert/dcm2raw.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.7.0/barbell2_bodycomp/convert/npy2dcm.py` & `barbell2_bodycomp-0.8.0/barbell2_bodycomp/convert/npy2dcm.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.7.0/barbell2_bodycomp/convert/npy2nrrd.py` & `barbell2_bodycomp-0.8.0/barbell2_bodycomp/convert/npy2nrrd.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.7.0/barbell2_bodycomp/convert/npy2png.py` & `barbell2_bodycomp-0.8.0/barbell2_bodycomp/convert/npy2png.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.7.0/barbell2_bodycomp/convert/tag2dcm.py` & `barbell2_bodycomp-0.8.0/barbell2_bodycomp/convert/tag2dcm.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.7.0/barbell2_bodycomp/pipeline/bodycomp.py` & `barbell2_bodycomp-0.8.0/barbell2_bodycomp/pipeline/bodycomp.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.7.0/barbell2_bodycomp/seg.py` & `barbell2_bodycomp-0.8.0/barbell2_bodycomp/seg.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 class MuscleFatSegmentator:
 
     ARGMAX = 0
     PROBABILITIES = 1
 
     def __init__(self):
         self.input_files = None
-        self.image_dimensions = None
+        # self.image_dimensions = None
         self.model_files = None
         self.mode = MuscleFatSegmentator.ARGMAX
         self.output_directory = None
         self.output_segmentation_files = None
 
     @staticmethod
     def load_model(file_path):
@@ -81,17 +81,17 @@
         return new_prediction
 
     def execute(self):
         logger.info('Running MuscleFatSegmentator...')
         if self.input_files is None:
             logger.error('Input files not specified')
             return None
-        if self.image_dimensions is None:
-            logger.error('Image dimensions not specified')
-            return None
+        # if self.image_dimensions is None:
+        #     logger.error('Image dimensions not specified')
+        #     return None
         if self.model_files is None:
             logger.error('Model files not specified')
             return None
         if self.output_directory is None:
             logger.error('Output directory not specified')
             return None
         os.makedirs(self.output_directory, exist_ok=True)
@@ -132,15 +132,15 @@
 
 
 if __name__ == '__main__':
     def main():
         segmentator = MuscleFatSegmentator()
         # segmentator.input_files = ['/Users/ralph/Desktop/SliceSelector/L3.dcm']
         segmentator.input_files = ['/mnt/localscratch/cds/rbrecheisen/raw/pancreas-demo-1/1.dcm']
-        segmentator.image_dimensions = (512, 512)
+        # segmentator.image_dimensions = (512, 512)
         segmentator.model_files = [
             '/mnt/localscratch/cds/rbrecheisen/models/v2/model.zip',
             '/mnt/localscratch/cds/rbrecheisen/models/v2/contour_model.zip',
             '/mnt/localscratch/cds/rbrecheisen/models/v2/params.json',
         ]
         # segmentator.mode = MuscleFatSegmentator.ARGMAX
         segmentator.mode = MuscleFatSegmentator.PROBABILITIES
```

### Comparing `barbell2_bodycomp-0.7.0/barbell2_bodycomp/selectroi.py` & `barbell2_bodycomp-0.8.0/barbell2_bodycomp/selectroi.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.7.0/barbell2_bodycomp/selectslice.py` & `barbell2_bodycomp-0.8.0/barbell2_bodycomp/selectslice.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.7.0/barbell2_bodycomp/totalseg.py` & `barbell2_bodycomp-0.8.0/barbell2_bodycomp/totalseg.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.7.0/barbell2_bodycomp/utils.py` & `barbell2_bodycomp-0.8.0/barbell2_bodycomp/utils.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.7.0/barbell2_bodycomp.egg-info/PKG-INFO` & `barbell2_bodycomp-0.8.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 Metadata-Version: 2.1
-Name: barbell2-bodycomp
-Version: 0.7.0
+Name: barbell2_bodycomp
+Version: 0.8.0
 Summary: components for command-line body composition analysis
 Home-page: https://github.com/rbrecheisen/barbell2_bodycomp
 Author: Ralph Brecheisen
 Author-email: r.brecheisen@maastrichtuniversity.nl
 License: MIT license
 Keywords: barbell2_bodycomp
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.5
-
-UNKNOWN
-
```

### Comparing `barbell2_bodycomp-0.7.0/barbell2_bodycomp.egg-info/SOURCES.txt` & `barbell2_bodycomp-0.8.0/barbell2_bodycomp.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 barbell2_bodycomp/selectroi.py
 barbell2_bodycomp/selectslice.py
 barbell2_bodycomp/totalseg.py
 barbell2_bodycomp/utils.py
 barbell2_bodycomp.egg-info/PKG-INFO
 barbell2_bodycomp.egg-info/SOURCES.txt
 barbell2_bodycomp.egg-info/dependency_links.txt
-barbell2_bodycomp.egg-info/entry_points.txt
 barbell2_bodycomp.egg-info/not-zip-safe
 barbell2_bodycomp.egg-info/requires.txt
 barbell2_bodycomp.egg-info/top_level.txt
 barbell2_bodycomp/convert/__init__.py
 barbell2_bodycomp/convert/dcm2nifti.py
 barbell2_bodycomp/convert/dcm2npy.py
 barbell2_bodycomp/convert/dcm2raw.py
```

### Comparing `barbell2_bodycomp-0.7.0/setup.py` & `barbell2_bodycomp-0.8.0/setup.py`

 * *Files identical despite different names*

