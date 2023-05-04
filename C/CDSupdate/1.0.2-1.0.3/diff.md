# Comparing `tmp/CDSupdate-1.0.2.tar.gz` & `tmp/CDSupdate-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CDSupdate-1.0.2.tar", last modified: Wed May  3 08:20:34 2023, max compression
+gzip compressed data, was "CDSupdate-1.0.3.tar", last modified: Wed May  3 13:01:02 2023, max compression
```

## Comparing `CDSupdate-1.0.2.tar` & `CDSupdate-1.0.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-03 08:20:34.969552 CDSupdate-1.0.2/
-drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-03 08:20:34.964956 CDSupdate-1.0.2/CDSupdate/
--rw-r--r--   0 yrobin     (501) staff       (20)     9238 2023-05-03 06:51:04.000000 CDSupdate-1.0.2/CDSupdate/__CDSUParams.py
--rw-r--r--   0 yrobin     (501) staff       (20)     5131 2023-05-02 14:45:32.000000 CDSupdate-1.0.2/CDSupdate/__CVarsParams.py
--rw-r--r--   0 yrobin     (501) staff       (20)     2685 2022-08-31 14:53:13.000000 CDSupdate-1.0.2/CDSupdate/__curses_doc.py
--rw-r--r--   0 yrobin     (501) staff       (20)     3690 2023-05-02 14:45:32.000000 CDSupdate-1.0.2/CDSupdate/__doc.py
--rw-r--r--   0 yrobin     (501) staff       (20)      847 2023-05-02 14:45:32.000000 CDSupdate-1.0.2/CDSupdate/__exceptions.py
--rw-r--r--   0 yrobin     (501) staff       (20)     4268 2023-05-02 14:45:32.000000 CDSupdate-1.0.2/CDSupdate/__exec.py
--rw-r--r--   0 yrobin     (501) staff       (20)    12971 2023-05-02 14:45:32.000000 CDSupdate-1.0.2/CDSupdate/__extracvars.py
--rw-r--r--   0 yrobin     (501) staff       (20)      974 2023-05-02 14:45:32.000000 CDSupdate-1.0.2/CDSupdate/__init__.py
--rw-r--r--   0 yrobin     (501) staff       (20)    14498 2023-05-02 14:45:32.000000 CDSupdate-1.0.2/CDSupdate/__io.py
--rw-r--r--   0 yrobin     (501) staff       (20)     2068 2023-05-03 06:51:04.000000 CDSupdate-1.0.2/CDSupdate/__release.py
-drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-03 08:20:34.968794 CDSupdate-1.0.2/CDSupdate/data/
--rw-r--r--   0 yrobin     (501) staff       (20)      574 2023-05-02 14:45:32.000000 CDSupdate-1.0.2/CDSupdate/data/ERA5-dptas-description.txt
--rw-r--r--   0 yrobin     (501) staff       (20)     1389 2023-05-02 14:45:32.000000 CDSupdate-1.0.2/CDSupdate/data/ERA5-name.csv
--rw-r--r--   0 yrobin     (501) staff       (20)     1572 2023-05-02 14:45:32.000000 CDSupdate-1.0.2/CDSupdate/data/ERA5-pr-description.txt
--rw-r--r--   0 yrobin     (501) staff       (20)      717 2023-05-02 14:45:32.000000 CDSupdate-1.0.2/CDSupdate/data/ERA5-ps-description.txt
--rw-r--r--   0 yrobin     (501) staff       (20)      830 2022-08-31 14:53:14.000000 CDSupdate-1.0.2/CDSupdate/data/ERA5-psl-description.txt
--rw-r--r--   0 yrobin     (501) staff       (20)      380 2022-08-31 14:53:14.000000 CDSupdate-1.0.2/CDSupdate/data/ERA5-tas-description.txt
--rw-r--r--   0 yrobin     (501) staff       (20)      604 2023-05-02 14:45:32.000000 CDSupdate-1.0.2/CDSupdate/data/ERA5-uas-description.txt
--rw-r--r--   0 yrobin     (501) staff       (20)      606 2023-05-02 14:45:32.000000 CDSupdate-1.0.2/CDSupdate/data/ERA5-vas-description.txt
--rw-r--r--   0 yrobin     (501) staff       (20)      842 2023-05-02 14:45:32.000000 CDSupdate-1.0.2/CDSupdate/data/ERA5-zg-description.txt
--rw-r--r--   0 yrobin     (501) staff       (20)      723 2023-05-02 14:45:32.000000 CDSupdate-1.0.2/CDSupdate/data/__init__.py
--rw-r--r--   0 yrobin     (501) staff       (20)      134 2023-05-03 06:31:49.000000 CDSupdate-1.0.2/CDSupdate/data/areas.csv
-drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-03 08:20:34.965847 CDSupdate-1.0.2/CDSupdate.egg-info/
--rw-r--r--   0 yrobin     (501) staff       (20)      561 2023-05-03 08:20:34.000000 CDSupdate-1.0.2/CDSupdate.egg-info/PKG-INFO
--rw-r--r--   0 yrobin     (501) staff       (20)      821 2023-05-03 08:20:34.000000 CDSupdate-1.0.2/CDSupdate.egg-info/SOURCES.txt
--rw-r--r--   0 yrobin     (501) staff       (20)        1 2023-05-03 08:20:34.000000 CDSupdate-1.0.2/CDSupdate.egg-info/dependency_links.txt
--rw-r--r--   0 yrobin     (501) staff       (20)       10 2023-05-03 08:20:34.000000 CDSupdate-1.0.2/CDSupdate.egg-info/top_level.txt
--rw-r--r--   0 yrobin     (501) staff       (20)    35149 2022-03-16 15:22:09.000000 CDSupdate-1.0.2/LICENSE
--rw-r--r--   0 yrobin     (501) staff       (20)       58 2022-08-31 14:53:14.000000 CDSupdate-1.0.2/MANIFEST.in
--rw-r--r--   0 yrobin     (501) staff       (20)      561 2023-05-03 08:20:34.969430 CDSupdate-1.0.2/PKG-INFO
--rw-r--r--   0 yrobin     (501) staff       (20)     1526 2023-05-02 14:45:32.000000 CDSupdate-1.0.2/README.md
-drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-03 08:20:34.969223 CDSupdate-1.0.2/scripts/
--rwxr-xr-x   0 yrobin     (501) staff       (20)      894 2023-05-02 14:45:32.000000 CDSupdate-1.0.2/scripts/cdsupdate
--rw-r--r--   0 yrobin     (501) staff       (20)       38 2023-05-03 08:20:34.969588 CDSupdate-1.0.2/setup.cfg
--rwxr-xr-x   0 yrobin     (501) staff       (20)     2004 2023-05-02 14:45:32.000000 CDSupdate-1.0.2/setup.py
+drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-03 13:01:02.259701 CDSupdate-1.0.3/
+drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-03 13:01:02.256174 CDSupdate-1.0.3/CDSupdate/
+-rw-r--r--   0 yrobin     (501) staff       (20)     9238 2023-05-03 06:51:04.000000 CDSupdate-1.0.3/CDSupdate/__CDSUParams.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     5131 2023-05-02 14:45:32.000000 CDSupdate-1.0.3/CDSupdate/__CVarsParams.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     2685 2022-08-31 14:53:13.000000 CDSupdate-1.0.3/CDSupdate/__curses_doc.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     3690 2023-05-02 14:45:32.000000 CDSupdate-1.0.3/CDSupdate/__doc.py
+-rw-r--r--   0 yrobin     (501) staff       (20)      847 2023-05-02 14:45:32.000000 CDSupdate-1.0.3/CDSupdate/__exceptions.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     4268 2023-05-02 14:45:32.000000 CDSupdate-1.0.3/CDSupdate/__exec.py
+-rw-r--r--   0 yrobin     (501) staff       (20)    12819 2023-05-03 12:54:20.000000 CDSupdate-1.0.3/CDSupdate/__extracvars.py
+-rw-r--r--   0 yrobin     (501) staff       (20)      974 2023-05-02 14:45:32.000000 CDSupdate-1.0.3/CDSupdate/__init__.py
+-rw-r--r--   0 yrobin     (501) staff       (20)    14464 2023-05-03 12:54:20.000000 CDSupdate-1.0.3/CDSupdate/__io.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     2068 2023-05-03 12:54:20.000000 CDSupdate-1.0.3/CDSupdate/__release.py
+drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-03 13:01:02.259134 CDSupdate-1.0.3/CDSupdate/data/
+-rw-r--r--   0 yrobin     (501) staff       (20)      574 2023-05-02 14:45:32.000000 CDSupdate-1.0.3/CDSupdate/data/ERA5-dptas-description.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)     1389 2023-05-02 14:45:32.000000 CDSupdate-1.0.3/CDSupdate/data/ERA5-name.csv
+-rw-r--r--   0 yrobin     (501) staff       (20)     1572 2023-05-02 14:45:32.000000 CDSupdate-1.0.3/CDSupdate/data/ERA5-pr-description.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)      717 2023-05-02 14:45:32.000000 CDSupdate-1.0.3/CDSupdate/data/ERA5-ps-description.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)      830 2022-08-31 14:53:14.000000 CDSupdate-1.0.3/CDSupdate/data/ERA5-psl-description.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)      380 2022-08-31 14:53:14.000000 CDSupdate-1.0.3/CDSupdate/data/ERA5-tas-description.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)      604 2023-05-02 14:45:32.000000 CDSupdate-1.0.3/CDSupdate/data/ERA5-uas-description.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)      606 2023-05-02 14:45:32.000000 CDSupdate-1.0.3/CDSupdate/data/ERA5-vas-description.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)      842 2023-05-02 14:45:32.000000 CDSupdate-1.0.3/CDSupdate/data/ERA5-zg-description.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)      723 2023-05-02 14:45:32.000000 CDSupdate-1.0.3/CDSupdate/data/__init__.py
+-rw-r--r--   0 yrobin     (501) staff       (20)      134 2023-05-03 06:31:49.000000 CDSupdate-1.0.3/CDSupdate/data/areas.csv
+drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-03 13:01:02.256800 CDSupdate-1.0.3/CDSupdate.egg-info/
+-rw-r--r--   0 yrobin     (501) staff       (20)      561 2023-05-03 13:01:02.000000 CDSupdate-1.0.3/CDSupdate.egg-info/PKG-INFO
+-rw-r--r--   0 yrobin     (501) staff       (20)      821 2023-05-03 13:01:02.000000 CDSupdate-1.0.3/CDSupdate.egg-info/SOURCES.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)        1 2023-05-03 13:01:02.000000 CDSupdate-1.0.3/CDSupdate.egg-info/dependency_links.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)       10 2023-05-03 13:01:02.000000 CDSupdate-1.0.3/CDSupdate.egg-info/top_level.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)    35149 2022-03-16 15:22:09.000000 CDSupdate-1.0.3/LICENSE
+-rw-r--r--   0 yrobin     (501) staff       (20)       58 2022-08-31 14:53:14.000000 CDSupdate-1.0.3/MANIFEST.in
+-rw-r--r--   0 yrobin     (501) staff       (20)      561 2023-05-03 13:01:02.259584 CDSupdate-1.0.3/PKG-INFO
+-rw-r--r--   0 yrobin     (501) staff       (20)     1526 2023-05-02 14:45:32.000000 CDSupdate-1.0.3/README.md
+drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-03 13:01:02.259398 CDSupdate-1.0.3/scripts/
+-rwxr-xr-x   0 yrobin     (501) staff       (20)      894 2023-05-02 14:45:32.000000 CDSupdate-1.0.3/scripts/cdsupdate
+-rw-r--r--   0 yrobin     (501) staff       (20)       38 2023-05-03 13:01:02.259733 CDSupdate-1.0.3/setup.cfg
+-rwxr-xr-x   0 yrobin     (501) staff       (20)     2004 2023-05-02 14:45:32.000000 CDSupdate-1.0.3/setup.py
```

### Comparing `CDSupdate-1.0.2/CDSupdate/__CDSUParams.py` & `CDSupdate-1.0.3/CDSupdate/__CDSUParams.py`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.0.2/CDSupdate/__CVarsParams.py` & `CDSupdate-1.0.3/CDSupdate/__CVarsParams.py`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.0.2/CDSupdate/__curses_doc.py` & `CDSupdate-1.0.3/CDSupdate/__curses_doc.py`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.0.2/CDSupdate/__doc.py` & `CDSupdate-1.0.3/CDSupdate/__doc.py`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.0.2/CDSupdate/__exceptions.py` & `CDSupdate-1.0.3/CDSupdate/__exceptions.py`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.0.2/CDSupdate/__exec.py` & `CDSupdate-1.0.3/CDSupdate/__exec.py`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.0.2/CDSupdate/__extracvars.py` & `CDSupdate-1.0.3/CDSupdate/__extracvars.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,24 +129,23 @@
 		odatah = idatau.copy( deep = True ).rename( uas = "sfcWind" )
 		odatah["sfcWind"] = np.sqrt( idatau["uas"]**2 + idatav["vas"]**2 )
 		
 		## Build daily
 		odatad = odatah.groupby("time.dayofyear").mean().rename( dayofyear = "time" ).assign_coords( time = dtime )
 		
 		## Save hourly
-		if cdsuParams.keep_hourly:
-			opath = os.path.join( cdsuParams.tmp , "ERA5-AMIP" , "hr" , "sfcWind" )
-			t0    = str(odatah.time[ 0].values)[:13].replace("-","").replace(" ","").replace("T","")
-			t1    = str(odatah.time[-1].values)[:13].replace("-","").replace(" ","").replace("T","")
-			ofile = f"ERA5-AMIP_sfcWind_hr_{area_name}_{t0}-{t1}.nc"
-			target = os.path.join( opath , ofile )
-			if not os.path.isdir(opath):
-				os.makedirs(opath)
-			logger.info( f" * Save 'TMP/ERA5-AMIP/hr/sfcWind/{ofile}'" )
-			odatah.to_netcdf( os.path.join( opath , ofile ) )
+		opath = os.path.join( cdsuParams.tmp , "ERA5-AMIP" , "hr" , "sfcWind" )
+		t0    = str(odatah.time[ 0].values)[:13].replace("-","").replace(" ","").replace("T","")
+		t1    = str(odatah.time[-1].values)[:13].replace("-","").replace(" ","").replace("T","")
+		ofile = f"ERA5-AMIP_sfcWind_hr_{area_name}_{t0}-{t1}.nc"
+		target = os.path.join( opath , ofile )
+		if not os.path.isdir(opath):
+			os.makedirs(opath)
+		logger.info( f" * Save 'TMP/ERA5-AMIP/hr/sfcWind/{ofile}'" )
+		odatah.to_netcdf( os.path.join( opath , ofile ) )
 		
 		## Save daily
 		opath = os.path.join( cdsuParams.tmp , "ERA5-AMIP" , "day" , "sfcWind" )
 		t0    = str(odatad.time[ 0].values)[:10].replace("-","").replace(" ","").replace("T","")
 		t1    = str(odatad.time[-1].values)[:10].replace("-","").replace(" ","").replace("T","")
 		ofile = f"ERA5-AMIP_sfcWind_day_{area_name}_{t0}-{t1}.nc"
 		target = os.path.join( opath , ofile )
@@ -184,24 +183,23 @@
 		eT     = 6.1078 * np.exp( 17.1 * ( idataT[  "tas"] - 273.15 ) / ( 235 + idataT[  "tas"] - 273.15 ) )
 		odatah[cvar] = eD / eT * 100
 		
 		## Build daily
 		odatad = odatah.groupby("time.dayofyear").mean().rename( dayofyear = "time" ).assign_coords( time = dtime )
 		
 		## Save hourly
-		if cdsuParams.keep_hourly:
-			opath = os.path.join( cdsuParams.tmp , "ERA5-AMIP" , "hr" , cvar )
-			t0    = str(odatah.time[ 0].values)[:13].replace("-","").replace(" ","").replace("T","")
-			t1    = str(odatah.time[-1].values)[:13].replace("-","").replace(" ","").replace("T","")
-			ofile = f"ERA5-AMIP_{cvar}_hr_{area_name}_{t0}-{t1}.nc"
-			target = os.path.join( opath , ofile )
-			if not os.path.isdir(opath):
-				os.makedirs(opath)
-			logger.info( f" * Save 'TMP/ERA5-AMIP/hr/{cvar}/{ofile}'" )
-			odatah.to_netcdf( os.path.join( opath , ofile ) )
+		opath = os.path.join( cdsuParams.tmp , "ERA5-AMIP" , "hr" , cvar )
+		t0    = str(odatah.time[ 0].values)[:13].replace("-","").replace(" ","").replace("T","")
+		t1    = str(odatah.time[-1].values)[:13].replace("-","").replace(" ","").replace("T","")
+		ofile = f"ERA5-AMIP_{cvar}_hr_{area_name}_{t0}-{t1}.nc"
+		target = os.path.join( opath , ofile )
+		if not os.path.isdir(opath):
+			os.makedirs(opath)
+		logger.info( f" * Save 'TMP/ERA5-AMIP/hr/{cvar}/{ofile}'" )
+		odatah.to_netcdf( os.path.join( opath , ofile ) )
 		
 		## Save daily
 		opath = os.path.join( cdsuParams.tmp , "ERA5-AMIP" , "day" , cvar )
 		t0    = str(odatad.time[ 0].values)[:10].replace("-","").replace(" ","").replace("T","")
 		t1    = str(odatad.time[-1].values)[:10].replace("-","").replace(" ","").replace("T","")
 		ofile = f"ERA5-AMIP_{cvar}_day_{area_name}_{t0}-{t1}.nc"
 		target = os.path.join( opath , ofile )
@@ -244,24 +242,23 @@
 		E            = a1 * np.exp( a3 * ( idataD["dptas"] - T0 ) / ( idataD["dptas"] - a4 ) )
 		odatah[cvar] = E * ( rdry / rvap ) / ( idataP["ps"] - ( E * ( 1 - rdry / rvap ) ) )
 		
 		## Build daily
 		odatad = odatah.groupby("time.dayofyear").mean().rename( dayofyear = "time" ).assign_coords( time = dtime )
 		
 		## Save hourly
-		if cdsuParams.keep_hourly:
-			opath = os.path.join( cdsuParams.tmp , "ERA5-AMIP" , "hr" , cvar )
-			t0    = str(odatah.time[ 0].values)[:13].replace("-","").replace(" ","").replace("T","")
-			t1    = str(odatah.time[-1].values)[:13].replace("-","").replace(" ","").replace("T","")
-			ofile = f"ERA5-AMIP_{cvar}_hr_{area_name}_{t0}-{t1}.nc"
-			target = os.path.join( opath , ofile )
-			if not os.path.isdir(opath):
-				os.makedirs(opath)
-			logger.info( f" * Save 'TMP/ERA5-AMIP/hr/{cvar}/{ofile}'" )
-			odatah.to_netcdf( os.path.join( opath , ofile ) )
+		opath = os.path.join( cdsuParams.tmp , "ERA5-AMIP" , "hr" , cvar )
+		t0    = str(odatah.time[ 0].values)[:13].replace("-","").replace(" ","").replace("T","")
+		t1    = str(odatah.time[-1].values)[:13].replace("-","").replace(" ","").replace("T","")
+		ofile = f"ERA5-AMIP_{cvar}_hr_{area_name}_{t0}-{t1}.nc"
+		target = os.path.join( opath , ofile )
+		if not os.path.isdir(opath):
+			os.makedirs(opath)
+		logger.info( f" * Save 'TMP/ERA5-AMIP/hr/{cvar}/{ofile}'" )
+		odatah.to_netcdf( os.path.join( opath , ofile ) )
 		
 		## Save daily
 		opath = os.path.join( cdsuParams.tmp , "ERA5-AMIP" , "day" , cvar )
 		t0    = str(odatad.time[ 0].values)[:10].replace("-","").replace(" ","").replace("T","")
 		t1    = str(odatad.time[-1].values)[:10].replace("-","").replace(" ","").replace("T","")
 		ofile = f"ERA5-AMIP_{cvar}_day_{area_name}_{t0}-{t1}.nc"
 		target = os.path.join( opath , ofile )
@@ -312,24 +309,23 @@
 		odatah[cvar] = 273.15 + c0 + c1 * T + c2 * H + c3 * T * H + c4 * T**2 + c5 * H**2 + c6 * T**2 * H + c7 * T * H**2 + c8 * T**2 * H**2
 		odatah[cvar] = odatah[cvar].where( T > 20 , np.nan )
 		
 		## Build daily
 		odatad = odatah.groupby("time.dayofyear").mean().rename( dayofyear = "time" ).assign_coords( time = dtime )
 		
 		## Save hourly
-		if cdsuParams.keep_hourly:
-			opath = os.path.join( cdsuParams.tmp , "ERA5-AMIP" , "hr" , cvar )
-			t0    = str(odatah.time[ 0].values)[:13].replace("-","").replace(" ","").replace("T","")
-			t1    = str(odatah.time[-1].values)[:13].replace("-","").replace(" ","").replace("T","")
-			ofile = f"ERA5-AMIP_{cvar}_hr_{area_name}_{t0}-{t1}.nc"
-			target = os.path.join( opath , ofile )
-			if not os.path.isdir(opath):
-				os.makedirs(opath)
-			logger.info( f" * Save 'TMP/ERA5-AMIP/hr/{cvar}/{ofile}'" )
-			odatah.to_netcdf( os.path.join( opath , ofile ) )
+		opath = os.path.join( cdsuParams.tmp , "ERA5-AMIP" , "hr" , cvar )
+		t0    = str(odatah.time[ 0].values)[:13].replace("-","").replace(" ","").replace("T","")
+		t1    = str(odatah.time[-1].values)[:13].replace("-","").replace(" ","").replace("T","")
+		ofile = f"ERA5-AMIP_{cvar}_hr_{area_name}_{t0}-{t1}.nc"
+		target = os.path.join( opath , ofile )
+		if not os.path.isdir(opath):
+			os.makedirs(opath)
+		logger.info( f" * Save 'TMP/ERA5-AMIP/hr/{cvar}/{ofile}'" )
+		odatah.to_netcdf( os.path.join( opath , ofile ) )
 		
 		## Save daily
 		opath = os.path.join( cdsuParams.tmp , "ERA5-AMIP" , "day" , cvar )
 		t0    = str(odatad.time[ 0].values)[:10].replace("-","").replace(" ","").replace("T","")
 		t1    = str(odatad.time[-1].values)[:10].replace("-","").replace(" ","").replace("T","")
 		ofile = f"ERA5-AMIP_{cvar}_day_{area_name}_{t0}-{t1}.nc"
 		target = os.path.join( opath , ofile )
```

### Comparing `CDSupdate-1.0.2/CDSupdate/__init__.py` & `CDSupdate-1.0.3/CDSupdate/__init__.py`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.0.2/CDSupdate/__io.py` & `CDSupdate-1.0.3/CDSupdate/__io.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,25 +183,24 @@
 				idata = idata.sel( time = slice(t0,tm) ).compute()
 			
 			## Change scale
 			if cvar in ["zg"]:
 				g = 9.80665
 				idata[cvar+h] = idata[cvar+h] / g
 			
-			## Save hourly variable
-			if cdsuParams.keep_hourly:
-				opath = os.path.join( cdsuParams.tmp , "ERA5-AMIP" , "hr" , cvar + h )
-				t0    = str(idata.time[ 0].values)[:13].replace("-","").replace(" ","").replace("T","")
-				t1    = str(idata.time[-1].values)[:13].replace("-","").replace(" ","").replace("T","")
-				ofile = f"ERA5-AMIP_{cvar+h}_hr_{area_name}_{t0}-{t1}.nc"
-				target = os.path.join( opath , ofile )
-				if not os.path.isdir(opath):
-					os.makedirs(opath)
-				logger.info( f" * Save 'TMP/ERA5-AMIP/hr/{cvar+h}/{ofile}'" )
-				idata.to_netcdf( os.path.join( opath , ofile ) )
+			## Transform hourly variable
+			opath = os.path.join( cdsuParams.tmp , "ERA5-AMIP" , "hr" , cvar + h )
+			t0    = str(idata.time[ 0].values)[:13].replace("-","").replace(" ","").replace("T","")
+			t1    = str(idata.time[-1].values)[:13].replace("-","").replace(" ","").replace("T","")
+			ofile = f"ERA5-AMIP_{cvar+h}_hr_{area_name}_{t0}-{t1}.nc"
+			target = os.path.join( opath , ofile )
+			if not os.path.isdir(opath):
+				os.makedirs(opath)
+			logger.info( f" * Save 'TMP/ERA5-AMIP/hr/{cvar+h}/{ofile}'" )
+			idata.to_netcdf( os.path.join( opath , ofile ) )
 			
 			## Build daily variable
 			dtime = [dt.datetime(int(year),1,1) + dt.timedelta( days = int(i) - 1 ) for i in np.unique(idata.time.dt.dayofyear.values)]
 			ddata = idata.groupby("time.dayofyear").mean().rename( dayofyear = "time" ).assign_coords( time = dtime )
 			
 			## Save daily variable
 			opath = os.path.join( cdsuParams.tmp , "ERA5-AMIP" , "day" , cvar + h )
```

### Comparing `CDSupdate-1.0.2/CDSupdate/__release.py` & `CDSupdate-1.0.3/CDSupdate/__release.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 ## 
 ## You should have received a copy of the GNU General Public License
 ## along with CDSupdate.  If not, see <https://www.gnu.org/licenses/>.
 
 
 version_major = "1"
 version_minor = "0"
-version_patch = "2"
+version_patch = "3"
 version_extra = ""
 version       = f"{version_major}.{version_minor}.{version_patch}{version_extra}"
 
 name = "CDSupdate"
 
 description = "Auto-updater of data from the Climate Data Store"
```

### Comparing `CDSupdate-1.0.2/CDSupdate/data/ERA5-dptas-description.txt` & `CDSupdate-1.0.3/CDSupdate/data/ERA5-dptas-description.txt`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.0.2/CDSupdate/data/ERA5-name.csv` & `CDSupdate-1.0.3/CDSupdate/data/ERA5-name.csv`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.0.2/CDSupdate/data/ERA5-pr-description.txt` & `CDSupdate-1.0.3/CDSupdate/data/ERA5-pr-description.txt`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.0.2/CDSupdate/data/ERA5-ps-description.txt` & `CDSupdate-1.0.3/CDSupdate/data/ERA5-ps-description.txt`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.0.2/CDSupdate/data/ERA5-psl-description.txt` & `CDSupdate-1.0.3/CDSupdate/data/ERA5-psl-description.txt`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.0.2/CDSupdate/data/ERA5-uas-description.txt` & `CDSupdate-1.0.3/CDSupdate/data/ERA5-uas-description.txt`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.0.2/CDSupdate/data/ERA5-vas-description.txt` & `CDSupdate-1.0.3/CDSupdate/data/ERA5-vas-description.txt`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.0.2/CDSupdate/data/ERA5-zg-description.txt` & `CDSupdate-1.0.3/CDSupdate/data/ERA5-zg-description.txt`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.0.2/CDSupdate/data/__init__.py` & `CDSupdate-1.0.3/CDSupdate/data/__init__.py`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.0.2/CDSupdate.egg-info/PKG-INFO` & `CDSupdate-1.0.3/CDSupdate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CDSupdate
-Version: 1.0.2
+Version: 1.0.3
 Summary: Auto-updater of data from the Climate Data Store
 Home-page: https://github.com/yrobink/CDSupdate
 Author: Yoann Robin
 Author-email: yoann.robin.k@gmail.com
 License: GNU-GPL3
 Keywords: Climate Data Store,Auto update
 Platform: linux
```

### Comparing `CDSupdate-1.0.2/CDSupdate.egg-info/SOURCES.txt` & `CDSupdate-1.0.3/CDSupdate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.0.2/LICENSE` & `CDSupdate-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.0.2/PKG-INFO` & `CDSupdate-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CDSupdate
-Version: 1.0.2
+Version: 1.0.3
 Summary: Auto-updater of data from the Climate Data Store
 Home-page: https://github.com/yrobink/CDSupdate
 Author: Yoann Robin
 Author-email: yoann.robin.k@gmail.com
 License: GNU-GPL3
 Keywords: Climate Data Store,Auto update
 Platform: linux
```

### Comparing `CDSupdate-1.0.2/README.md` & `CDSupdate-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.0.2/scripts/cdsupdate` & `CDSupdate-1.0.3/scripts/cdsupdate`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.0.2/setup.py` & `CDSupdate-1.0.3/setup.py`

 * *Files identical despite different names*

