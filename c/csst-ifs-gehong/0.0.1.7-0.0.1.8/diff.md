# Comparing `tmp/csst-ifs-gehong-0.0.1.7.tar.gz` & `tmp/csst-ifs-gehong-0.0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csst-ifs-gehong-0.0.1.7.tar", last modified: Thu May  4 05:29:44 2023, max compression
+gzip compressed data, was "csst-ifs-gehong-0.0.1.8.tar", last modified: Thu May  4 11:51:12 2023, max compression
```

## Comparing `csst-ifs-gehong-0.0.1.7.tar` & `csst-ifs-gehong-0.0.1.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 sfeng      (501) staff       (20)        0 2023-05-04 05:29:44.787645 csst-ifs-gehong-0.0.1.7/
--rw-r--r--   0 sfeng      (501) staff       (20)     1073 2023-04-25 01:31:05.000000 csst-ifs-gehong-0.0.1.7/LICENSE
--rw-r--r--   0 sfeng      (501) staff       (20)      228 2023-05-04 05:29:44.787728 csst-ifs-gehong-0.0.1.7/PKG-INFO
--rw-r--r--   0 sfeng      (501) staff       (20)      244 2023-04-26 13:40:59.000000 csst-ifs-gehong-0.0.1.7/README.md
--rw-r--r--   0 sfeng      (501) staff       (20)      103 2023-05-04 05:29:44.788024 csst-ifs-gehong-0.0.1.7/setup.cfg
--rw-r--r--   0 sfeng      (501) staff       (20)      392 2023-05-04 05:29:20.000000 csst-ifs-gehong-0.0.1.7/setup.py
-drwxr-xr-x   0 sfeng      (501) staff       (20)        0 2023-05-04 05:29:44.782931 csst-ifs-gehong-0.0.1.7/src/
-drwxr-xr-x   0 sfeng      (501) staff       (20)        0 2023-05-04 05:29:44.784947 csst-ifs-gehong-0.0.1.7/src/csst_ifs_gehong.egg-info/
--rw-r--r--   0 sfeng      (501) staff       (20)      228 2023-05-04 05:29:44.000000 csst-ifs-gehong-0.0.1.7/src/csst_ifs_gehong.egg-info/PKG-INFO
--rw-r--r--   0 sfeng      (501) staff       (20)      415 2023-05-04 05:29:44.000000 csst-ifs-gehong-0.0.1.7/src/csst_ifs_gehong.egg-info/SOURCES.txt
--rw-r--r--   0 sfeng      (501) staff       (20)        1 2023-05-04 05:29:44.000000 csst-ifs-gehong-0.0.1.7/src/csst_ifs_gehong.egg-info/dependency_links.txt
--rw-r--r--   0 sfeng      (501) staff       (20)        8 2023-05-04 05:29:44.000000 csst-ifs-gehong-0.0.1.7/src/csst_ifs_gehong.egg-info/requires.txt
--rw-r--r--   0 sfeng      (501) staff       (20)        7 2023-05-04 05:29:44.000000 csst-ifs-gehong-0.0.1.7/src/csst_ifs_gehong.egg-info/top_level.txt
-drwxr-xr-x   0 sfeng      (501) staff       (20)        0 2023-05-04 05:29:44.785812 csst-ifs-gehong-0.0.1.7/src/gehong/
--rw-r--r--   0 sfeng      (501) staff       (20)        0 2023-04-12 01:06:24.000000 csst-ifs-gehong-0.0.1.7/src/gehong/__init__.py
--rw-r--r--   0 sfeng      (501) staff       (20)     1236 2023-05-02 10:42:18.000000 csst-ifs-gehong-0.0.1.7/src/gehong/config.py
--rw-r--r--   0 sfeng      (501) staff       (20)     3593 2023-05-04 05:29:07.000000 csst-ifs-gehong-0.0.1.7/src/gehong/cube3d.py
--rw-r--r--   0 sfeng      (501) staff       (20)    11669 2023-05-04 01:23:49.000000 csst-ifs-gehong-0.0.1.7/src/gehong/map2d.py
--rw-r--r--   0 sfeng      (501) staff       (20)    37347 2023-05-04 03:11:16.000000 csst-ifs-gehong-0.0.1.7/src/gehong/spec1d.py
-drwxr-xr-x   0 sfeng      (501) staff       (20)        0 2023-05-04 05:29:44.787184 csst-ifs-gehong-0.0.1.7/test/
--rw-r--r--   0 sfeng      (501) staff       (20)     2710 2023-05-03 04:52:05.000000 csst-ifs-gehong-0.0.1.7/test/test_cube3d.py
--rw-r--r--   0 sfeng      (501) staff       (20)     8115 2023-05-03 04:46:37.000000 csst-ifs-gehong-0.0.1.7/test/test_map2d.py
--rw-r--r--   0 sfeng      (501) staff       (20)    17388 2023-05-03 01:16:32.000000 csst-ifs-gehong-0.0.1.7/test/test_spec1d.py
+drwxr-xr-x   0 sfeng      (501) staff       (20)        0 2023-05-04 11:51:12.083974 csst-ifs-gehong-0.0.1.8/
+-rw-r--r--   0 sfeng      (501) staff       (20)     1073 2023-04-25 01:31:05.000000 csst-ifs-gehong-0.0.1.8/LICENSE
+-rw-r--r--   0 sfeng      (501) staff       (20)      228 2023-05-04 11:51:12.084092 csst-ifs-gehong-0.0.1.8/PKG-INFO
+-rw-r--r--   0 sfeng      (501) staff       (20)      244 2023-04-26 13:40:59.000000 csst-ifs-gehong-0.0.1.8/README.md
+-rw-r--r--   0 sfeng      (501) staff       (20)      103 2023-05-04 11:51:12.084495 csst-ifs-gehong-0.0.1.8/setup.cfg
+-rw-r--r--   0 sfeng      (501) staff       (20)      392 2023-05-04 11:50:41.000000 csst-ifs-gehong-0.0.1.8/setup.py
+drwxr-xr-x   0 sfeng      (501) staff       (20)        0 2023-05-04 11:51:12.080198 csst-ifs-gehong-0.0.1.8/src/
+drwxr-xr-x   0 sfeng      (501) staff       (20)        0 2023-05-04 11:51:12.081535 csst-ifs-gehong-0.0.1.8/src/csst_ifs_gehong.egg-info/
+-rw-r--r--   0 sfeng      (501) staff       (20)      228 2023-05-04 11:51:12.000000 csst-ifs-gehong-0.0.1.8/src/csst_ifs_gehong.egg-info/PKG-INFO
+-rw-r--r--   0 sfeng      (501) staff       (20)      415 2023-05-04 11:51:12.000000 csst-ifs-gehong-0.0.1.8/src/csst_ifs_gehong.egg-info/SOURCES.txt
+-rw-r--r--   0 sfeng      (501) staff       (20)        1 2023-05-04 11:51:12.000000 csst-ifs-gehong-0.0.1.8/src/csst_ifs_gehong.egg-info/dependency_links.txt
+-rw-r--r--   0 sfeng      (501) staff       (20)        8 2023-05-04 11:51:12.000000 csst-ifs-gehong-0.0.1.8/src/csst_ifs_gehong.egg-info/requires.txt
+-rw-r--r--   0 sfeng      (501) staff       (20)        7 2023-05-04 11:51:12.000000 csst-ifs-gehong-0.0.1.8/src/csst_ifs_gehong.egg-info/top_level.txt
+drwxr-xr-x   0 sfeng      (501) staff       (20)        0 2023-05-04 11:51:12.082734 csst-ifs-gehong-0.0.1.8/src/gehong/
+-rw-r--r--   0 sfeng      (501) staff       (20)        0 2023-04-12 01:06:24.000000 csst-ifs-gehong-0.0.1.8/src/gehong/__init__.py
+-rw-r--r--   0 sfeng      (501) staff       (20)     1236 2023-05-02 10:42:18.000000 csst-ifs-gehong-0.0.1.8/src/gehong/config.py
+-rw-r--r--   0 sfeng      (501) staff       (20)     3593 2023-05-04 09:46:41.000000 csst-ifs-gehong-0.0.1.8/src/gehong/cube3d.py
+-rw-r--r--   0 sfeng      (501) staff       (20)    11669 2023-05-04 01:23:49.000000 csst-ifs-gehong-0.0.1.8/src/gehong/map2d.py
+-rw-r--r--   0 sfeng      (501) staff       (20)    37404 2023-05-04 11:50:16.000000 csst-ifs-gehong-0.0.1.8/src/gehong/spec1d.py
+drwxr-xr-x   0 sfeng      (501) staff       (20)        0 2023-05-04 11:51:12.083499 csst-ifs-gehong-0.0.1.8/test/
+-rw-r--r--   0 sfeng      (501) staff       (20)     2710 2023-05-03 04:52:05.000000 csst-ifs-gehong-0.0.1.8/test/test_cube3d.py
+-rw-r--r--   0 sfeng      (501) staff       (20)     8115 2023-05-03 04:46:37.000000 csst-ifs-gehong-0.0.1.8/test/test_map2d.py
+-rw-r--r--   0 sfeng      (501) staff       (20)    17388 2023-05-03 01:16:32.000000 csst-ifs-gehong-0.0.1.8/test/test_spec1d.py
```

### Comparing `csst-ifs-gehong-0.0.1.7/LICENSE` & `csst-ifs-gehong-0.0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `csst-ifs-gehong-0.0.1.7/src/gehong/config.py` & `csst-ifs-gehong-0.0.1.8/src/gehong/config.py`

 * *Files identical despite different names*

### Comparing `csst-ifs-gehong-0.0.1.7/src/gehong/cube3d.py` & `csst-ifs-gehong-0.0.1.8/src/gehong/cube3d.py`

 * *Files identical despite different names*

### Comparing `csst-ifs-gehong-0.0.1.7/src/gehong/map2d.py` & `csst-ifs-gehong-0.0.1.8/src/gehong/map2d.py`

 * *Files identical despite different names*

### Comparing `csst-ifs-gehong-0.0.1.7/src/gehong/spec1d.py` & `csst-ifs-gehong-0.0.1.8/src/gehong/spec1d.py`

 * *Files 1% similar despite different names*

```diff
@@ -383,15 +383,15 @@
     def __init__(self, config, temp, halpha = 100.0, logz = 0.0,
                  vel = 100.0, vdisp = 120.0, ebv = 0.1):
 
         if (logz > -2) & (logz < 0.5):
             indz = np.argmin(np.abs(logz - temp.logz_grid))
             flux_ratio = temp.flux_ratio[indz, :]
         else:
-            raise ValueError('The range of logZ is not correct!')
+            raise ValueError('The value of logZ is not in the range of [-2, 0.5]!')
         
         # Make emission line spectra through adding emission lines                 
         emlines = temp.emission_lines * flux_ratio
         flux_combine = np.sum(emlines, axis = 1)
         flux_calibrate = flux_combine * halpha      # Units: erg/s/A/cm^2
         
         # Dust attenuation
@@ -459,46 +459,46 @@
     def __init__(self, config, temp, halpha = 100.0, logz = 0.0,
                  vel = 100.0, vdisp = 120.0, ebv = 0.1):
         
         if (logz > -2) & (logz < 0.5):
             indz = np.argmin(np.abs(logz - temp.logz_grid))
             flux_ratio = temp.flux_ratio[indz, :]
         else:
-            raise ValueError('The value of logZ is not correct!')
+            raise ValueError('The value of logZ is not in the range of [-2, 0.5]!')
         
         # Make emission line spectra through adding emission lines                 
-        emlines = temp.emission_lines * flux_ratio
+        emlines = temp.emission_lines * (flux_ratio / flux_ratio[6] )
         flux_combine = np.sum(emlines, axis = 1)
         flux_calibrate = flux_combine * halpha      # Units: 1e-17 erg/s/A/cm^2
         
         # Dust attenuation
         if np.isscalar(ebv):
             flux_dust = reddening(temp.wave, flux_calibrate, ebv = ebv)
             
         # Broadening caused by Velocity Dispersion
         velscale = 10
         lam_range = [np.min(temp.wave), np.max(temp.wave)]
         flux_logwave, logLam = log_rebin(lam_range, flux_dust, velscale=velscale)[:2]
         
-        sigma_gas = vdisp / velscale                                # in pixel
-        sigma_LSF = temp.FWHM_inst / (np.exp(logLam)) * 3e5 / velscale          # in pixel
+        sigma_gas = vdisp / velscale                                        # in pixel
+        sigma_LSF = temp.FWHM_inst / (np.exp(logLam)) * 3e5 / velscale      # in pixel
         
         if sigma_gas>0: 
             sigma_dif = np.zeros(len(flux_logwave))
             idx = (sigma_gas > sigma_LSF)
             sigma_dif[idx] = np.sqrt(sigma_gas ** 2. - sigma_LSF[idx] ** 2.)
             idx = (sigma_gas <= sigma_LSF)
             sigma_dif[idx] = 0.1
             flux_broad = gaussian_filter1d(flux_logwave, sigma_dif)
             
         # Redshift
         redshift = vel / 3e5
         wave_r = np.exp(logLam) * (1 + redshift)
         flux_red = np.interp(config.wave, wave_r, flux_broad)
-            
+        
         self.wave = config.wave
         self.flux = flux_red
 
 class AGN_BLR():
 
     """
     Class for the broad line region of AGN
@@ -516,15 +516,15 @@
     ebv : float, optional
         Dust extinction, by default 0.1
     lam_range : list, optional
         Wavelength range, by default [500, 15000]
     """
 
     def __init__(self, config, hbeta_flux = 100.0, hbeta_fwhm = 2000.0, ebv = 0.1, 
-                 vel = 0.,lam_range = [500, 15000]):
+                 vel = 0., lam_range = [500, 15000]):
 
         wave_rest = np.arange(lam_range[0], lam_range[1], 0.1)
         
         line_names = ['Hepsilon', 'Hdelta', 'Hgamma', 'Hbeta', 'Halpha']
         line_waves = [3970.079, 4101.742, 4340.471, 4861.333, 6562.819]
         line_ratio = [0.101, 0.208, 0.405, 1.000, 2.579]              # From Ilic et al. (2006)
         
@@ -573,14 +573,15 @@
     vel : float, optional
         Line of sight velocity, by default 100.0km/s
     ebv : float, optional
         Dust extinction, by default 0.1
     """
     
     def __init__(self, config, hbeta_broad = 100.0, r4570 = 0.4, ebv = 0.1, vel = 100.0):
+
         filename = data_path + '/data/FeII.AGN.fits'
         
         # Loading FeII template
         hdulist = fits.open(filename)
         data = hdulist[1].data
         wave_rest  = data['WAVE']
         flux_model = data['FLUX']
```

### Comparing `csst-ifs-gehong-0.0.1.7/test/test_cube3d.py` & `csst-ifs-gehong-0.0.1.8/test/test_cube3d.py`

 * *Files identical despite different names*

### Comparing `csst-ifs-gehong-0.0.1.7/test/test_map2d.py` & `csst-ifs-gehong-0.0.1.8/test/test_map2d.py`

 * *Files identical despite different names*

### Comparing `csst-ifs-gehong-0.0.1.7/test/test_spec1d.py` & `csst-ifs-gehong-0.0.1.8/test/test_spec1d.py`

 * *Files identical despite different names*

