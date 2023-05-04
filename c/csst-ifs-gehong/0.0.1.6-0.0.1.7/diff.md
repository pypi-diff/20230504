# Comparing `tmp/csst-ifs-gehong-0.0.1.6.tar.gz` & `tmp/csst-ifs-gehong-0.0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csst-ifs-gehong-0.0.1.6.tar", last modified: Thu May  4 03:16:05 2023, max compression
+gzip compressed data, was "csst-ifs-gehong-0.0.1.7.tar", last modified: Thu May  4 05:29:44 2023, max compression
```

## Comparing `csst-ifs-gehong-0.0.1.6.tar` & `csst-ifs-gehong-0.0.1.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 sfeng      (501) staff       (20)        0 2023-05-04 03:16:05.078795 csst-ifs-gehong-0.0.1.6/
--rw-r--r--   0 sfeng      (501) staff       (20)     1073 2023-04-25 01:31:05.000000 csst-ifs-gehong-0.0.1.6/LICENSE
--rw-r--r--   0 sfeng      (501) staff       (20)      228 2023-05-04 03:16:05.078866 csst-ifs-gehong-0.0.1.6/PKG-INFO
--rw-r--r--   0 sfeng      (501) staff       (20)      244 2023-04-26 13:40:59.000000 csst-ifs-gehong-0.0.1.6/README.md
--rw-r--r--   0 sfeng      (501) staff       (20)      103 2023-05-04 03:16:05.079154 csst-ifs-gehong-0.0.1.6/setup.cfg
--rw-r--r--   0 sfeng      (501) staff       (20)      392 2023-05-04 03:15:43.000000 csst-ifs-gehong-0.0.1.6/setup.py
-drwxr-xr-x   0 sfeng      (501) staff       (20)        0 2023-05-04 03:16:05.074845 csst-ifs-gehong-0.0.1.6/src/
-drwxr-xr-x   0 sfeng      (501) staff       (20)        0 2023-05-04 03:16:05.076585 csst-ifs-gehong-0.0.1.6/src/csst_ifs_gehong.egg-info/
--rw-r--r--   0 sfeng      (501) staff       (20)      228 2023-05-04 03:16:05.000000 csst-ifs-gehong-0.0.1.6/src/csst_ifs_gehong.egg-info/PKG-INFO
--rw-r--r--   0 sfeng      (501) staff       (20)      415 2023-05-04 03:16:05.000000 csst-ifs-gehong-0.0.1.6/src/csst_ifs_gehong.egg-info/SOURCES.txt
--rw-r--r--   0 sfeng      (501) staff       (20)        1 2023-05-04 03:16:05.000000 csst-ifs-gehong-0.0.1.6/src/csst_ifs_gehong.egg-info/dependency_links.txt
--rw-r--r--   0 sfeng      (501) staff       (20)        8 2023-05-04 03:16:05.000000 csst-ifs-gehong-0.0.1.6/src/csst_ifs_gehong.egg-info/requires.txt
--rw-r--r--   0 sfeng      (501) staff       (20)        7 2023-05-04 03:16:05.000000 csst-ifs-gehong-0.0.1.6/src/csst_ifs_gehong.egg-info/top_level.txt
-drwxr-xr-x   0 sfeng      (501) staff       (20)        0 2023-05-04 03:16:05.077712 csst-ifs-gehong-0.0.1.6/src/gehong/
--rw-r--r--   0 sfeng      (501) staff       (20)        0 2023-04-12 01:06:24.000000 csst-ifs-gehong-0.0.1.6/src/gehong/__init__.py
--rw-r--r--   0 sfeng      (501) staff       (20)     1236 2023-05-02 10:42:18.000000 csst-ifs-gehong-0.0.1.6/src/gehong/config.py
--rw-r--r--   0 sfeng      (501) staff       (20)     3591 2023-05-03 04:54:26.000000 csst-ifs-gehong-0.0.1.6/src/gehong/cube3d.py
--rw-r--r--   0 sfeng      (501) staff       (20)    11669 2023-05-04 01:23:49.000000 csst-ifs-gehong-0.0.1.6/src/gehong/map2d.py
--rw-r--r--   0 sfeng      (501) staff       (20)    37347 2023-05-04 03:11:16.000000 csst-ifs-gehong-0.0.1.6/src/gehong/spec1d.py
-drwxr-xr-x   0 sfeng      (501) staff       (20)        0 2023-05-04 03:16:05.078584 csst-ifs-gehong-0.0.1.6/test/
--rw-r--r--   0 sfeng      (501) staff       (20)     2710 2023-05-03 04:52:05.000000 csst-ifs-gehong-0.0.1.6/test/test_cube3d.py
--rw-r--r--   0 sfeng      (501) staff       (20)     8115 2023-05-03 04:46:37.000000 csst-ifs-gehong-0.0.1.6/test/test_map2d.py
--rw-r--r--   0 sfeng      (501) staff       (20)    17388 2023-05-03 01:16:32.000000 csst-ifs-gehong-0.0.1.6/test/test_spec1d.py
+drwxr-xr-x   0 sfeng      (501) staff       (20)        0 2023-05-04 05:29:44.787645 csst-ifs-gehong-0.0.1.7/
+-rw-r--r--   0 sfeng      (501) staff       (20)     1073 2023-04-25 01:31:05.000000 csst-ifs-gehong-0.0.1.7/LICENSE
+-rw-r--r--   0 sfeng      (501) staff       (20)      228 2023-05-04 05:29:44.787728 csst-ifs-gehong-0.0.1.7/PKG-INFO
+-rw-r--r--   0 sfeng      (501) staff       (20)      244 2023-04-26 13:40:59.000000 csst-ifs-gehong-0.0.1.7/README.md
+-rw-r--r--   0 sfeng      (501) staff       (20)      103 2023-05-04 05:29:44.788024 csst-ifs-gehong-0.0.1.7/setup.cfg
+-rw-r--r--   0 sfeng      (501) staff       (20)      392 2023-05-04 05:29:20.000000 csst-ifs-gehong-0.0.1.7/setup.py
+drwxr-xr-x   0 sfeng      (501) staff       (20)        0 2023-05-04 05:29:44.782931 csst-ifs-gehong-0.0.1.7/src/
+drwxr-xr-x   0 sfeng      (501) staff       (20)        0 2023-05-04 05:29:44.784947 csst-ifs-gehong-0.0.1.7/src/csst_ifs_gehong.egg-info/
+-rw-r--r--   0 sfeng      (501) staff       (20)      228 2023-05-04 05:29:44.000000 csst-ifs-gehong-0.0.1.7/src/csst_ifs_gehong.egg-info/PKG-INFO
+-rw-r--r--   0 sfeng      (501) staff       (20)      415 2023-05-04 05:29:44.000000 csst-ifs-gehong-0.0.1.7/src/csst_ifs_gehong.egg-info/SOURCES.txt
+-rw-r--r--   0 sfeng      (501) staff       (20)        1 2023-05-04 05:29:44.000000 csst-ifs-gehong-0.0.1.7/src/csst_ifs_gehong.egg-info/dependency_links.txt
+-rw-r--r--   0 sfeng      (501) staff       (20)        8 2023-05-04 05:29:44.000000 csst-ifs-gehong-0.0.1.7/src/csst_ifs_gehong.egg-info/requires.txt
+-rw-r--r--   0 sfeng      (501) staff       (20)        7 2023-05-04 05:29:44.000000 csst-ifs-gehong-0.0.1.7/src/csst_ifs_gehong.egg-info/top_level.txt
+drwxr-xr-x   0 sfeng      (501) staff       (20)        0 2023-05-04 05:29:44.785812 csst-ifs-gehong-0.0.1.7/src/gehong/
+-rw-r--r--   0 sfeng      (501) staff       (20)        0 2023-04-12 01:06:24.000000 csst-ifs-gehong-0.0.1.7/src/gehong/__init__.py
+-rw-r--r--   0 sfeng      (501) staff       (20)     1236 2023-05-02 10:42:18.000000 csst-ifs-gehong-0.0.1.7/src/gehong/config.py
+-rw-r--r--   0 sfeng      (501) staff       (20)     3593 2023-05-04 05:29:07.000000 csst-ifs-gehong-0.0.1.7/src/gehong/cube3d.py
+-rw-r--r--   0 sfeng      (501) staff       (20)    11669 2023-05-04 01:23:49.000000 csst-ifs-gehong-0.0.1.7/src/gehong/map2d.py
+-rw-r--r--   0 sfeng      (501) staff       (20)    37347 2023-05-04 03:11:16.000000 csst-ifs-gehong-0.0.1.7/src/gehong/spec1d.py
+drwxr-xr-x   0 sfeng      (501) staff       (20)        0 2023-05-04 05:29:44.787184 csst-ifs-gehong-0.0.1.7/test/
+-rw-r--r--   0 sfeng      (501) staff       (20)     2710 2023-05-03 04:52:05.000000 csst-ifs-gehong-0.0.1.7/test/test_cube3d.py
+-rw-r--r--   0 sfeng      (501) staff       (20)     8115 2023-05-03 04:46:37.000000 csst-ifs-gehong-0.0.1.7/test/test_map2d.py
+-rw-r--r--   0 sfeng      (501) staff       (20)    17388 2023-05-03 01:16:32.000000 csst-ifs-gehong-0.0.1.7/test/test_spec1d.py
```

### Comparing `csst-ifs-gehong-0.0.1.6/LICENSE` & `csst-ifs-gehong-0.0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `csst-ifs-gehong-0.0.1.6/src/gehong/config.py` & `csst-ifs-gehong-0.0.1.7/src/gehong/config.py`

 * *Files identical despite different names*

### Comparing `csst-ifs-gehong-0.0.1.6/src/gehong/cube3d.py` & `csst-ifs-gehong-0.0.1.7/src/gehong/cube3d.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,15 +45,15 @@
                 else:
                     self.flux[i,j,:] = ss.flux
                     
     def wcs_info(self):
         wcs = fits.Header()
         wcs_dict = {'CTYPE1': 'WAVE    ', 
                     'CUNIT1': 'Angstrom', 
-                    'CDELT1': self.inst.dlam, 
+                    'CDELT1': self.config.dlam, 
                     'CRPIX1': 1, 
                     'CRVAL1': np.min(self.wave), 
                     'CTYPE2': 'RA---TAN', 
                     'CUNIT2': 'deg', 
                     'CDELT2': self.dpix / 3600., 
                     'CRPIX2': np.round(self.ny / 2.), 
                     'CRVAL2': 0.5,
```

### Comparing `csst-ifs-gehong-0.0.1.6/src/gehong/map2d.py` & `csst-ifs-gehong-0.0.1.7/src/gehong/map2d.py`

 * *Files identical despite different names*

### Comparing `csst-ifs-gehong-0.0.1.6/src/gehong/spec1d.py` & `csst-ifs-gehong-0.0.1.7/src/gehong/spec1d.py`

 * *Files identical despite different names*

### Comparing `csst-ifs-gehong-0.0.1.6/test/test_cube3d.py` & `csst-ifs-gehong-0.0.1.7/test/test_cube3d.py`

 * *Files identical despite different names*

### Comparing `csst-ifs-gehong-0.0.1.6/test/test_map2d.py` & `csst-ifs-gehong-0.0.1.7/test/test_map2d.py`

 * *Files identical despite different names*

### Comparing `csst-ifs-gehong-0.0.1.6/test/test_spec1d.py` & `csst-ifs-gehong-0.0.1.7/test/test_spec1d.py`

 * *Files identical despite different names*

