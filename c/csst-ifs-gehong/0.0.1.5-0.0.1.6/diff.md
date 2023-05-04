# Comparing `tmp/csst-ifs-gehong-0.0.1.5.tar.gz` & `tmp/csst-ifs-gehong-0.0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csst-ifs-gehong-0.0.1.5.tar", last modified: Wed May  3 12:15:02 2023, max compression
+gzip compressed data, was "csst-ifs-gehong-0.0.1.6.tar", last modified: Thu May  4 03:16:05 2023, max compression
```

## Comparing `csst-ifs-gehong-0.0.1.5.tar` & `csst-ifs-gehong-0.0.1.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 sfeng      (501) staff       (20)        0 2023-05-03 12:15:02.489448 csst-ifs-gehong-0.0.1.5/
--rw-r--r--   0 sfeng      (501) staff       (20)     1073 2023-04-25 01:31:05.000000 csst-ifs-gehong-0.0.1.5/LICENSE
--rw-r--r--   0 sfeng      (501) staff       (20)      228 2023-05-03 12:15:02.489538 csst-ifs-gehong-0.0.1.5/PKG-INFO
--rw-r--r--   0 sfeng      (501) staff       (20)      244 2023-04-26 13:40:59.000000 csst-ifs-gehong-0.0.1.5/README.md
--rw-r--r--   0 sfeng      (501) staff       (20)      103 2023-05-03 12:15:02.489897 csst-ifs-gehong-0.0.1.5/setup.cfg
--rw-r--r--   0 sfeng      (501) staff       (20)      392 2023-05-03 11:43:38.000000 csst-ifs-gehong-0.0.1.5/setup.py
-drwxr-xr-x   0 sfeng      (501) staff       (20)        0 2023-05-03 12:15:02.484777 csst-ifs-gehong-0.0.1.5/src/
-drwxr-xr-x   0 sfeng      (501) staff       (20)        0 2023-05-03 12:15:02.486724 csst-ifs-gehong-0.0.1.5/src/csst_ifs_gehong.egg-info/
--rw-r--r--   0 sfeng      (501) staff       (20)      228 2023-05-03 12:15:02.000000 csst-ifs-gehong-0.0.1.5/src/csst_ifs_gehong.egg-info/PKG-INFO
--rw-r--r--   0 sfeng      (501) staff       (20)      415 2023-05-03 12:15:02.000000 csst-ifs-gehong-0.0.1.5/src/csst_ifs_gehong.egg-info/SOURCES.txt
--rw-r--r--   0 sfeng      (501) staff       (20)        1 2023-05-03 12:15:02.000000 csst-ifs-gehong-0.0.1.5/src/csst_ifs_gehong.egg-info/dependency_links.txt
--rw-r--r--   0 sfeng      (501) staff       (20)        8 2023-05-03 12:15:02.000000 csst-ifs-gehong-0.0.1.5/src/csst_ifs_gehong.egg-info/requires.txt
--rw-r--r--   0 sfeng      (501) staff       (20)        7 2023-05-03 12:15:02.000000 csst-ifs-gehong-0.0.1.5/src/csst_ifs_gehong.egg-info/top_level.txt
-drwxr-xr-x   0 sfeng      (501) staff       (20)        0 2023-05-03 12:15:02.488025 csst-ifs-gehong-0.0.1.5/src/gehong/
--rw-r--r--   0 sfeng      (501) staff       (20)        0 2023-04-12 01:06:24.000000 csst-ifs-gehong-0.0.1.5/src/gehong/__init__.py
--rw-r--r--   0 sfeng      (501) staff       (20)     1236 2023-05-02 10:42:18.000000 csst-ifs-gehong-0.0.1.5/src/gehong/config.py
--rw-r--r--   0 sfeng      (501) staff       (20)     3591 2023-05-03 04:54:26.000000 csst-ifs-gehong-0.0.1.5/src/gehong/cube3d.py
--rw-r--r--   0 sfeng      (501) staff       (20)    11669 2023-05-03 04:45:44.000000 csst-ifs-gehong-0.0.1.5/src/gehong/map2d.py
--rw-r--r--   0 sfeng      (501) staff       (20)    37295 2023-05-03 12:14:02.000000 csst-ifs-gehong-0.0.1.5/src/gehong/spec1d.py
-drwxr-xr-x   0 sfeng      (501) staff       (20)        0 2023-05-03 12:15:02.488764 csst-ifs-gehong-0.0.1.5/test/
--rw-r--r--   0 sfeng      (501) staff       (20)     2710 2023-05-03 04:52:05.000000 csst-ifs-gehong-0.0.1.5/test/test_cube3d.py
--rw-r--r--   0 sfeng      (501) staff       (20)     8115 2023-05-03 04:46:37.000000 csst-ifs-gehong-0.0.1.5/test/test_map2d.py
--rw-r--r--   0 sfeng      (501) staff       (20)    17388 2023-05-03 01:16:32.000000 csst-ifs-gehong-0.0.1.5/test/test_spec1d.py
+drwxr-xr-x   0 sfeng      (501) staff       (20)        0 2023-05-04 03:16:05.078795 csst-ifs-gehong-0.0.1.6/
+-rw-r--r--   0 sfeng      (501) staff       (20)     1073 2023-04-25 01:31:05.000000 csst-ifs-gehong-0.0.1.6/LICENSE
+-rw-r--r--   0 sfeng      (501) staff       (20)      228 2023-05-04 03:16:05.078866 csst-ifs-gehong-0.0.1.6/PKG-INFO
+-rw-r--r--   0 sfeng      (501) staff       (20)      244 2023-04-26 13:40:59.000000 csst-ifs-gehong-0.0.1.6/README.md
+-rw-r--r--   0 sfeng      (501) staff       (20)      103 2023-05-04 03:16:05.079154 csst-ifs-gehong-0.0.1.6/setup.cfg
+-rw-r--r--   0 sfeng      (501) staff       (20)      392 2023-05-04 03:15:43.000000 csst-ifs-gehong-0.0.1.6/setup.py
+drwxr-xr-x   0 sfeng      (501) staff       (20)        0 2023-05-04 03:16:05.074845 csst-ifs-gehong-0.0.1.6/src/
+drwxr-xr-x   0 sfeng      (501) staff       (20)        0 2023-05-04 03:16:05.076585 csst-ifs-gehong-0.0.1.6/src/csst_ifs_gehong.egg-info/
+-rw-r--r--   0 sfeng      (501) staff       (20)      228 2023-05-04 03:16:05.000000 csst-ifs-gehong-0.0.1.6/src/csst_ifs_gehong.egg-info/PKG-INFO
+-rw-r--r--   0 sfeng      (501) staff       (20)      415 2023-05-04 03:16:05.000000 csst-ifs-gehong-0.0.1.6/src/csst_ifs_gehong.egg-info/SOURCES.txt
+-rw-r--r--   0 sfeng      (501) staff       (20)        1 2023-05-04 03:16:05.000000 csst-ifs-gehong-0.0.1.6/src/csst_ifs_gehong.egg-info/dependency_links.txt
+-rw-r--r--   0 sfeng      (501) staff       (20)        8 2023-05-04 03:16:05.000000 csst-ifs-gehong-0.0.1.6/src/csst_ifs_gehong.egg-info/requires.txt
+-rw-r--r--   0 sfeng      (501) staff       (20)        7 2023-05-04 03:16:05.000000 csst-ifs-gehong-0.0.1.6/src/csst_ifs_gehong.egg-info/top_level.txt
+drwxr-xr-x   0 sfeng      (501) staff       (20)        0 2023-05-04 03:16:05.077712 csst-ifs-gehong-0.0.1.6/src/gehong/
+-rw-r--r--   0 sfeng      (501) staff       (20)        0 2023-04-12 01:06:24.000000 csst-ifs-gehong-0.0.1.6/src/gehong/__init__.py
+-rw-r--r--   0 sfeng      (501) staff       (20)     1236 2023-05-02 10:42:18.000000 csst-ifs-gehong-0.0.1.6/src/gehong/config.py
+-rw-r--r--   0 sfeng      (501) staff       (20)     3591 2023-05-03 04:54:26.000000 csst-ifs-gehong-0.0.1.6/src/gehong/cube3d.py
+-rw-r--r--   0 sfeng      (501) staff       (20)    11669 2023-05-04 01:23:49.000000 csst-ifs-gehong-0.0.1.6/src/gehong/map2d.py
+-rw-r--r--   0 sfeng      (501) staff       (20)    37347 2023-05-04 03:11:16.000000 csst-ifs-gehong-0.0.1.6/src/gehong/spec1d.py
+drwxr-xr-x   0 sfeng      (501) staff       (20)        0 2023-05-04 03:16:05.078584 csst-ifs-gehong-0.0.1.6/test/
+-rw-r--r--   0 sfeng      (501) staff       (20)     2710 2023-05-03 04:52:05.000000 csst-ifs-gehong-0.0.1.6/test/test_cube3d.py
+-rw-r--r--   0 sfeng      (501) staff       (20)     8115 2023-05-03 04:46:37.000000 csst-ifs-gehong-0.0.1.6/test/test_map2d.py
+-rw-r--r--   0 sfeng      (501) staff       (20)    17388 2023-05-03 01:16:32.000000 csst-ifs-gehong-0.0.1.6/test/test_spec1d.py
```

### Comparing `csst-ifs-gehong-0.0.1.5/LICENSE` & `csst-ifs-gehong-0.0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `csst-ifs-gehong-0.0.1.5/src/gehong/config.py` & `csst-ifs-gehong-0.0.1.6/src/gehong/config.py`

 * *Files identical despite different names*

### Comparing `csst-ifs-gehong-0.0.1.5/src/gehong/cube3d.py` & `csst-ifs-gehong-0.0.1.6/src/gehong/cube3d.py`

 * *Files identical despite different names*

### Comparing `csst-ifs-gehong-0.0.1.5/src/gehong/map2d.py` & `csst-ifs-gehong-0.0.1.6/src/gehong/map2d.py`

 * *Files identical despite different names*

### Comparing `csst-ifs-gehong-0.0.1.5/src/gehong/spec1d.py` & `csst-ifs-gehong-0.0.1.6/src/gehong/spec1d.py`

 * *Files 0% similar despite different names*

```diff
@@ -409,14 +409,16 @@
         if sigma_gas>0: 
             sigma_dif = np.zeros(len(flux_logwave))
             idx = (sigma_gas > sigma_LSF)
             sigma_dif[idx] = np.sqrt(sigma_gas ** 2. - sigma_LSF[idx] ** 2.)
             idx = (sigma_gas <= sigma_LSF)
             sigma_dif[idx] = 0.1
             flux_broad = gaussian_filter1d(flux_logwave, sigma_dif)
+        else:
+            flux_broad = flux_logwave
             
         # Redshift
         redshift = vel / 3e5
         wave_r = np.exp(logLam) * (1 + redshift)
         flux_red = np.interp(config.wave, wave_r, flux_broad)
             
         self.wave = config.wave
@@ -663,28 +665,28 @@
     edd_ratio : float, optional
         Eddinton ratio used for calculating the luminosity of power law spectrum at 5100A, by default 0.05
     halpha_broad : float, optional
         Integral flux of Halpha broad line, by default 100.0 * 1e-17 erg/s/cm^2
     halpha_narrow : float, optional
         Integral flux of Halpha narrow line, by default 100.0 * 1e-17 erg/s/cm^2
     vdisp_broad : float, optional
-        Velocity dispersion of Halpha broad line, by default 2000.0km/s
+        Velocity dispersion of Halpha broad line, by default 5000.0km/s
     vdisp_narrow : float, optional
         Velocity dispersion of Halpha narrow line, by default 500.0km/s
     vel : float, optional
         Line of sight velocity, by default 1000.0km/s
     logz : float, optional
         Gas-phase metallicity of narrow line region, by default 0.0
     ebv : float, optional
         Dust extinction, by default 0.1
     dist : float, optional
         Luminosity distance of AGN, by default 20.0Mpc
     """
     def __init__(self, config, nlr_template, bhmass = 1e6, edd_ratio = 0.05, 
-                 halpha_broad = 100.0, halpha_narrow = 100.0, vdisp_broad = 2000.0, vdisp_narrow = 500.0, 
+                 halpha_broad = 100.0, halpha_narrow = 100.0, vdisp_broad = 5000.0, vdisp_narrow = 500.0, 
                  vel = 1000.0, logz = 0.0, ebv = 0.1, dist = 20.0):
         
         NLR = AGN_NLR(config, nlr_template, halpha = halpha_narrow, logz = logz,
                       vel = vel, vdisp = vdisp_narrow, ebv = ebv)
         if halpha_broad > 0:
             BLR = AGN_BLR(config, hbeta_flux = halpha_broad / 2.579, 
                           hbeta_fwhm = vdisp_broad / 2.355, ebv = ebv, vel = vel)
```

### Comparing `csst-ifs-gehong-0.0.1.5/test/test_cube3d.py` & `csst-ifs-gehong-0.0.1.6/test/test_cube3d.py`

 * *Files identical despite different names*

### Comparing `csst-ifs-gehong-0.0.1.5/test/test_map2d.py` & `csst-ifs-gehong-0.0.1.6/test/test_map2d.py`

 * *Files identical despite different names*

### Comparing `csst-ifs-gehong-0.0.1.5/test/test_spec1d.py` & `csst-ifs-gehong-0.0.1.6/test/test_spec1d.py`

 * *Files identical despite different names*

