# Comparing `tmp/ukmon_meteortools-2023.5.5.tar.gz` & `tmp/ukmon_meteortools-2023.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ukmon_meteortools-2023.5.5.tar", last modified: Thu May  4 20:15:58 2023, max compression
+gzip compressed data, was "ukmon_meteortools-2023.5.6.tar", last modified: Thu May  4 20:21:46 2023, max compression
```

## Comparing `ukmon_meteortools-2023.5.5.tar` & `ukmon_meteortools-2023.5.6.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 20:15:58.729425 ukmon_meteortools-2023.5.5/
--rw-rw-rw-   0        0        0    35149 2020-04-29 17:18:36.000000 ukmon_meteortools-2023.5.5/LICENSE
--rw-rw-rw-   0        0        0    42659 2023-05-04 20:15:58.726418 ukmon_meteortools-2023.5.5/PKG-INFO
--rw-rw-rw-   0        0        0     1063 2023-04-12 22:46:43.000000 ukmon_meteortools-2023.5.5/README.md
--rw-rw-rw-   0        0        0     2185 2023-05-04 20:15:23.000000 ukmon_meteortools-2023.5.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-04 20:15:58.729425 ukmon_meteortools-2023.5.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-04 20:15:58.602747 ukmon_meteortools-2023.5.5/ukmon_meteortools/
--rw-rw-rw-   0        0        0      756 2023-05-02 21:24:36.000000 ukmon_meteortools-2023.5.5/ukmon_meteortools/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 20:15:58.650753 ukmon_meteortools-2023.5.5/ukmon_meteortools/fileformats/
--rw-rw-rw-   0        0        0     2372 2023-05-04 20:03:03.000000 ukmon_meteortools-2023.5.5/ukmon_meteortools/fileformats/ECSVhandler.py
--rw-rw-rw-   0        0        0    10159 2023-05-02 20:41:26.000000 ukmon_meteortools-2023.5.5/ukmon_meteortools/fileformats/UFOAnalyzerXML.py
--rw-rw-rw-   0        0        0     6742 2023-05-02 20:41:44.000000 ukmon_meteortools-2023.5.5/ukmon_meteortools/fileformats/UFOCapXML.py
--rw-rw-rw-   0        0        0      520 2023-05-04 19:41:10.000000 ukmon_meteortools-2023.5.5/ukmon_meteortools/fileformats/__init__.py
--rw-rw-rw-   0        0        0    19243 2023-05-02 20:13:35.000000 ukmon_meteortools-2023.5.5/ukmon_meteortools/fileformats/ftpDetectInfo.py
--rw-rw-rw-   0        0        0     7393 2023-05-02 21:34:25.000000 ukmon_meteortools-2023.5.5/ukmon_meteortools/fileformats/imoWorkingShowerList.py
--rw-rw-rw-   0        0        0     3642 2023-05-04 19:26:25.000000 ukmon_meteortools-2023.5.5/ukmon_meteortools/fileformats/kmlHandlers.py
--rw-rw-rw-   0        0        0     2948 2023-05-02 20:46:56.000000 ukmon_meteortools-2023.5.5/ukmon_meteortools/fileformats/platepar.py
-drwxrwxrwx   0        0        0        0 2023-05-04 20:15:58.670032 ukmon_meteortools-2023.5.5/ukmon_meteortools/rmsutils/
--rw-rw-rw-   0        0        0      720 2023-05-04 19:42:49.000000 ukmon_meteortools-2023.5.5/ukmon_meteortools/rmsutils/__init__.py
--rw-rw-rw-   0        0        0     1909 2023-05-02 20:41:57.000000 ukmon_meteortools-2023.5.5/ukmon_meteortools/rmsutils/analyseUFOwithRMS.py
--rw-rw-rw-   0        0        0     6077 2023-05-02 20:34:59.000000 ukmon_meteortools-2023.5.5/ukmon_meteortools/rmsutils/multiDayRadiant.py
--rw-rw-rw-   0        0        0     3763 2023-05-02 20:35:34.000000 ukmon_meteortools-2023.5.5/ukmon_meteortools/rmsutils/multiEventGroundMap.py
--rw-rw-rw-   0        0        0     5242 2023-05-03 14:21:56.000000 ukmon_meteortools-2023.5.5/ukmon_meteortools/rmsutils/multiTrackStack.py
--rw-rw-rw-   0        0        0     2297 2023-05-02 20:31:43.000000 ukmon_meteortools-2023.5.5/ukmon_meteortools/rmsutils/plotCAMSOrbits.py
--rw-rw-rw-   0        0        0     2281 2023-05-02 20:31:31.000000 ukmon_meteortools-2023.5.5/ukmon_meteortools/rmsutils/plotRMSOrbits.py
--rw-rw-rw-   0        0        0     1439 2023-05-04 19:30:59.000000 ukmon_meteortools-2023.5.5/ukmon_meteortools/rmsutils/trajPickle.py
-drwxrwxrwx   0        0        0        0 2023-05-04 20:15:58.678193 ukmon_meteortools-2023.5.5/ukmon_meteortools/share/
--rw-rw-rw-   0        0        0     8977 2023-04-18 21:24:56.000000 ukmon_meteortools-2023.5.5/ukmon_meteortools/share/IMO_Working_Meteor_Shower_List.xml
--rw-rw-rw-   0        0        0      525 2023-05-02 21:29:15.000000 ukmon_meteortools-2023.5.5/ukmon_meteortools/share/__init__.py
--rw-rw-rw-   0        0        0  5702528 2023-04-18 21:40:34.000000 ukmon_meteortools-2023.5.5/ukmon_meteortools/share/streamfulldata.npy
-drwxrwxrwx   0        0        0        0 2023-05-04 20:15:58.700420 ukmon_meteortools-2023.5.5/ukmon_meteortools/usertools/
--rw-rw-rw-   0        0        0      444 2023-05-04 19:36:38.000000 ukmon_meteortools-2023.5.5/ukmon_meteortools/usertools/__init__.py
--rw-rw-rw-   0        0        0     2945 2023-05-04 15:03:26.000000 ukmon_meteortools-2023.5.5/ukmon_meteortools/usertools/apiExampleCode.py
--rw-rw-rw-   0        0        0     1420 2023-03-08 12:49:12.000000 ukmon_meteortools-2023.5.5/ukmon_meteortools/usertools/findNearDuplicates.py
--rw-rw-rw-   0        0        0     4372 2023-05-04 16:56:04.000000 ukmon_meteortools-2023.5.5/ukmon_meteortools/usertools/getLiveImages.py
--rw-rw-rw-   0        0        0     3244 2023-05-04 19:33:10.000000 ukmon_meteortools-2023.5.5/ukmon_meteortools/usertools/getOverlappingFovs.py
--rw-rw-rw-   0        0        0     3589 2023-05-02 20:20:03.000000 ukmon_meteortools-2023.5.5/ukmon_meteortools/usertools/plotTrack.py
-drwxrwxrwx   0        0        0        0 2023-05-04 20:15:58.723420 ukmon_meteortools-2023.5.5/ukmon_meteortools/utils/
--rw-rw-rw-   0        0        0    13798 2023-05-02 20:57:25.000000 ukmon_meteortools-2023.5.5/ukmon_meteortools/utils/Math.py
--rw-rw-rw-   0        0        0      512 2023-04-29 16:53:34.000000 ukmon_meteortools-2023.5.5/ukmon_meteortools/utils/VectorMaths.py
--rw-rw-rw-   0        0        0     1296 2023-05-04 20:12:42.000000 ukmon_meteortools-2023.5.5/ukmon_meteortools/utils/__init__.py
--rw-rw-rw-   0        0        0     2519 2023-05-02 21:35:02.000000 ukmon_meteortools-2023.5.5/ukmon_meteortools/utils/annotateImage.py
--rw-rw-rw-   0        0        0     1313 2023-05-02 21:35:22.000000 ukmon_meteortools-2023.5.5/ukmon_meteortools/utils/convertSolLon.py
--rw-rw-rw-   0        0        0     2476 2023-05-02 20:12:42.000000 ukmon_meteortools-2023.5.5/ukmon_meteortools/utils/drawFTPfile.py
--rw-rw-rw-   0        0        0     2114 2023-05-02 21:35:49.000000 ukmon_meteortools-2023.5.5/ukmon_meteortools/utils/getActiveShowers.py
--rw-rw-rw-   0        0        0     3937 2023-05-02 21:41:36.000000 ukmon_meteortools-2023.5.5/ukmon_meteortools/utils/getShowerDates.py
--rw-rw-rw-   0        0        0     3699 2023-05-02 20:49:10.000000 ukmon_meteortools-2023.5.5/ukmon_meteortools/utils/sendAnEmail.py
-drwxrwxrwx   0        0        0        0 2023-05-04 20:15:58.634748 ukmon_meteortools-2023.5.5/ukmon_meteortools.egg-info/
--rw-rw-rw-   0        0        0    42659 2023-05-04 20:15:58.000000 ukmon_meteortools-2023.5.5/ukmon_meteortools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1752 2023-05-04 20:15:58.000000 ukmon_meteortools-2023.5.5/ukmon_meteortools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 20:15:58.000000 ukmon_meteortools-2023.5.5/ukmon_meteortools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      257 2023-05-04 20:15:58.000000 ukmon_meteortools-2023.5.5/ukmon_meteortools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-04 20:15:58.000000 ukmon_meteortools-2023.5.5/ukmon_meteortools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 20:21:46.092393 ukmon_meteortools-2023.5.6/
+-rw-rw-rw-   0        0        0    35149 2020-04-29 17:18:36.000000 ukmon_meteortools-2023.5.6/LICENSE
+-rw-rw-rw-   0        0        0    42659 2023-05-04 20:21:46.080390 ukmon_meteortools-2023.5.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1063 2023-04-12 22:46:43.000000 ukmon_meteortools-2023.5.6/README.md
+-rw-rw-rw-   0        0        0     2185 2023-05-04 20:21:22.000000 ukmon_meteortools-2023.5.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-04 20:21:46.093392 ukmon_meteortools-2023.5.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-04 20:21:45.885399 ukmon_meteortools-2023.5.6/ukmon_meteortools/
+-rw-rw-rw-   0        0        0      756 2023-05-02 21:24:36.000000 ukmon_meteortools-2023.5.6/ukmon_meteortools/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 20:21:45.976390 ukmon_meteortools-2023.5.6/ukmon_meteortools/fileformats/
+-rw-rw-rw-   0        0        0     2372 2023-05-04 20:03:03.000000 ukmon_meteortools-2023.5.6/ukmon_meteortools/fileformats/ECSVhandler.py
+-rw-rw-rw-   0        0        0    10159 2023-05-02 20:41:26.000000 ukmon_meteortools-2023.5.6/ukmon_meteortools/fileformats/UFOAnalyzerXML.py
+-rw-rw-rw-   0        0        0     6742 2023-05-02 20:41:44.000000 ukmon_meteortools-2023.5.6/ukmon_meteortools/fileformats/UFOCapXML.py
+-rw-rw-rw-   0        0        0      520 2023-05-04 19:41:10.000000 ukmon_meteortools-2023.5.6/ukmon_meteortools/fileformats/__init__.py
+-rw-rw-rw-   0        0        0    19244 2023-05-04 20:20:41.000000 ukmon_meteortools-2023.5.6/ukmon_meteortools/fileformats/ftpDetectInfo.py
+-rw-rw-rw-   0        0        0     7393 2023-05-02 21:34:25.000000 ukmon_meteortools-2023.5.6/ukmon_meteortools/fileformats/imoWorkingShowerList.py
+-rw-rw-rw-   0        0        0     3642 2023-05-04 19:26:25.000000 ukmon_meteortools-2023.5.6/ukmon_meteortools/fileformats/kmlHandlers.py
+-rw-rw-rw-   0        0        0     2948 2023-05-02 20:46:56.000000 ukmon_meteortools-2023.5.6/ukmon_meteortools/fileformats/platepar.py
+drwxrwxrwx   0        0        0        0 2023-05-04 20:21:45.996390 ukmon_meteortools-2023.5.6/ukmon_meteortools/rmsutils/
+-rw-rw-rw-   0        0        0      720 2023-05-04 19:42:49.000000 ukmon_meteortools-2023.5.6/ukmon_meteortools/rmsutils/__init__.py
+-rw-rw-rw-   0        0        0     1909 2023-05-02 20:41:57.000000 ukmon_meteortools-2023.5.6/ukmon_meteortools/rmsutils/analyseUFOwithRMS.py
+-rw-rw-rw-   0        0        0     6077 2023-05-02 20:34:59.000000 ukmon_meteortools-2023.5.6/ukmon_meteortools/rmsutils/multiDayRadiant.py
+-rw-rw-rw-   0        0        0     3763 2023-05-02 20:35:34.000000 ukmon_meteortools-2023.5.6/ukmon_meteortools/rmsutils/multiEventGroundMap.py
+-rw-rw-rw-   0        0        0     5242 2023-05-03 14:21:56.000000 ukmon_meteortools-2023.5.6/ukmon_meteortools/rmsutils/multiTrackStack.py
+-rw-rw-rw-   0        0        0     2297 2023-05-02 20:31:43.000000 ukmon_meteortools-2023.5.6/ukmon_meteortools/rmsutils/plotCAMSOrbits.py
+-rw-rw-rw-   0        0        0     2281 2023-05-02 20:31:31.000000 ukmon_meteortools-2023.5.6/ukmon_meteortools/rmsutils/plotRMSOrbits.py
+-rw-rw-rw-   0        0        0     1439 2023-05-04 19:30:59.000000 ukmon_meteortools-2023.5.6/ukmon_meteortools/rmsutils/trajPickle.py
+drwxrwxrwx   0        0        0        0 2023-05-04 20:21:46.001395 ukmon_meteortools-2023.5.6/ukmon_meteortools/share/
+-rw-rw-rw-   0        0        0     8977 2023-04-18 21:24:56.000000 ukmon_meteortools-2023.5.6/ukmon_meteortools/share/IMO_Working_Meteor_Shower_List.xml
+-rw-rw-rw-   0        0        0      525 2023-05-02 21:29:15.000000 ukmon_meteortools-2023.5.6/ukmon_meteortools/share/__init__.py
+-rw-rw-rw-   0        0        0  5702528 2023-04-18 21:40:34.000000 ukmon_meteortools-2023.5.6/ukmon_meteortools/share/streamfulldata.npy
+drwxrwxrwx   0        0        0        0 2023-05-04 20:21:46.046388 ukmon_meteortools-2023.5.6/ukmon_meteortools/usertools/
+-rw-rw-rw-   0        0        0      444 2023-05-04 19:36:38.000000 ukmon_meteortools-2023.5.6/ukmon_meteortools/usertools/__init__.py
+-rw-rw-rw-   0        0        0     2945 2023-05-04 15:03:26.000000 ukmon_meteortools-2023.5.6/ukmon_meteortools/usertools/apiExampleCode.py
+-rw-rw-rw-   0        0        0     1420 2023-03-08 12:49:12.000000 ukmon_meteortools-2023.5.6/ukmon_meteortools/usertools/findNearDuplicates.py
+-rw-rw-rw-   0        0        0     4372 2023-05-04 16:56:04.000000 ukmon_meteortools-2023.5.6/ukmon_meteortools/usertools/getLiveImages.py
+-rw-rw-rw-   0        0        0     3244 2023-05-04 19:33:10.000000 ukmon_meteortools-2023.5.6/ukmon_meteortools/usertools/getOverlappingFovs.py
+-rw-rw-rw-   0        0        0     3589 2023-05-02 20:20:03.000000 ukmon_meteortools-2023.5.6/ukmon_meteortools/usertools/plotTrack.py
+drwxrwxrwx   0        0        0        0 2023-05-04 20:21:46.079389 ukmon_meteortools-2023.5.6/ukmon_meteortools/utils/
+-rw-rw-rw-   0        0        0    13798 2023-05-02 20:57:25.000000 ukmon_meteortools-2023.5.6/ukmon_meteortools/utils/Math.py
+-rw-rw-rw-   0        0        0      512 2023-04-29 16:53:34.000000 ukmon_meteortools-2023.5.6/ukmon_meteortools/utils/VectorMaths.py
+-rw-rw-rw-   0        0        0     1296 2023-05-04 20:12:42.000000 ukmon_meteortools-2023.5.6/ukmon_meteortools/utils/__init__.py
+-rw-rw-rw-   0        0        0     2519 2023-05-02 21:35:02.000000 ukmon_meteortools-2023.5.6/ukmon_meteortools/utils/annotateImage.py
+-rw-rw-rw-   0        0        0     1313 2023-05-02 21:35:22.000000 ukmon_meteortools-2023.5.6/ukmon_meteortools/utils/convertSolLon.py
+-rw-rw-rw-   0        0        0     2476 2023-05-02 20:12:42.000000 ukmon_meteortools-2023.5.6/ukmon_meteortools/utils/drawFTPfile.py
+-rw-rw-rw-   0        0        0     2114 2023-05-02 21:35:49.000000 ukmon_meteortools-2023.5.6/ukmon_meteortools/utils/getActiveShowers.py
+-rw-rw-rw-   0        0        0     3937 2023-05-02 21:41:36.000000 ukmon_meteortools-2023.5.6/ukmon_meteortools/utils/getShowerDates.py
+-rw-rw-rw-   0        0        0     3699 2023-05-02 20:49:10.000000 ukmon_meteortools-2023.5.6/ukmon_meteortools/utils/sendAnEmail.py
+drwxrwxrwx   0        0        0        0 2023-05-04 20:21:45.958390 ukmon_meteortools-2023.5.6/ukmon_meteortools.egg-info/
+-rw-rw-rw-   0        0        0    42659 2023-05-04 20:21:45.000000 ukmon_meteortools-2023.5.6/ukmon_meteortools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1752 2023-05-04 20:21:45.000000 ukmon_meteortools-2023.5.6/ukmon_meteortools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 20:21:45.000000 ukmon_meteortools-2023.5.6/ukmon_meteortools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      257 2023-05-04 20:21:45.000000 ukmon_meteortools-2023.5.6/ukmon_meteortools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-04 20:21:45.000000 ukmon_meteortools-2023.5.6/ukmon_meteortools.egg-info/top_level.txt
```

### Comparing `ukmon_meteortools-2023.5.5/LICENSE` & `ukmon_meteortools-2023.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.5/PKG-INFO` & `ukmon_meteortools-2023.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ukmon_meteortools
-Version: 2023.5.5
+Version: 2023.5.6
 Summary: Python Tools for Meteor Data Analysis
 Author-email: Mark McIntyre <ukmon@markmcintyreastro.co.uk>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ukmon_meteortools-2023.5.5/README.md` & `ukmon_meteortools-2023.5.6/README.md`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.5/pyproject.toml` & `ukmon_meteortools-2023.5.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ukmon_meteortools"
-version = "2023.05.5"
+version = "2023.05.6"
 description = "Python Tools for Meteor Data Analysis"
 readme = "ukmon_meteortools/README.md"
 authors = [{ name = "Mark McIntyre", email = "ukmon@markmcintyreastro.co.uk" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -62,15 +62,15 @@
 #[tool.setuptools.packages.find]
 #where = ["ukmon_meteortools"]
 
 [tool.setuptools.package-data]
 "*" = ["*.npy", "*.xml"]
 
 [tool.bumpver]
-current_version = "2023.05.5"
+current_version = "2023.05.6"
 version_pattern = "YYYY.0M.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `ukmon_meteortools-2023.5.5/ukmon_meteortools/README.md` & `ukmon_meteortools-2023.5.6/ukmon_meteortools/README.md`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.5/ukmon_meteortools/fileformats/ECSVhandler.py` & `ukmon_meteortools-2023.5.6/ukmon_meteortools/fileformats/ECSVhandler.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.5/ukmon_meteortools/fileformats/UFOAnalyzerXML.py` & `ukmon_meteortools-2023.5.6/ukmon_meteortools/fileformats/UFOAnalyzerXML.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.5/ukmon_meteortools/fileformats/UFOCapXML.py` & `ukmon_meteortools-2023.5.6/ukmon_meteortools/fileformats/UFOCapXML.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.5/ukmon_meteortools/fileformats/__init__.py` & `ukmon_meteortools-2023.5.6/ukmon_meteortools/fileformats/__init__.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.5/ukmon_meteortools/fileformats/ftpDetectInfo.py` & `ukmon_meteortools-2023.5.6/ukmon_meteortools/fileformats/ftpDetectInfo.py`

 * *Files 0% similar despite different names*

```diff
@@ -346,15 +346,15 @@
             met1.mag_data = np.append(met1.mag_data, met2.mag_data)
 
             # Merge the FF file name and create a list
             if (met1.ff_name is not None) and (met2.ff_name is not None):
                 met1.ff_name = met1.ff_name + ',' + met2.ff_name
 
             # Sort all observations by time
-            met1.finish()
+            met1._finish()
 
             # Indicate that the next observation is to be skipped
             merged_indices.append(i + 1)
 
         # Removed merged meteors from the list
         meteor_list = [element for i, element in enumerate(meteor_list) if i not in merged_indices]
```

### Comparing `ukmon_meteortools-2023.5.5/ukmon_meteortools/fileformats/imoWorkingShowerList.py` & `ukmon_meteortools-2023.5.6/ukmon_meteortools/fileformats/imoWorkingShowerList.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.5/ukmon_meteortools/fileformats/kmlHandlers.py` & `ukmon_meteortools-2023.5.6/ukmon_meteortools/fileformats/kmlHandlers.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.5/ukmon_meteortools/fileformats/platepar.py` & `ukmon_meteortools-2023.5.6/ukmon_meteortools/fileformats/platepar.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.5/ukmon_meteortools/rmsutils/__init__.py` & `ukmon_meteortools-2023.5.6/ukmon_meteortools/rmsutils/__init__.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.5/ukmon_meteortools/rmsutils/analyseUFOwithRMS.py` & `ukmon_meteortools-2023.5.6/ukmon_meteortools/rmsutils/analyseUFOwithRMS.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.5/ukmon_meteortools/rmsutils/multiDayRadiant.py` & `ukmon_meteortools-2023.5.6/ukmon_meteortools/rmsutils/multiDayRadiant.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.5/ukmon_meteortools/rmsutils/multiEventGroundMap.py` & `ukmon_meteortools-2023.5.6/ukmon_meteortools/rmsutils/multiEventGroundMap.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.5/ukmon_meteortools/rmsutils/multiTrackStack.py` & `ukmon_meteortools-2023.5.6/ukmon_meteortools/rmsutils/multiTrackStack.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.5/ukmon_meteortools/rmsutils/plotCAMSOrbits.py` & `ukmon_meteortools-2023.5.6/ukmon_meteortools/rmsutils/plotCAMSOrbits.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.5/ukmon_meteortools/rmsutils/plotRMSOrbits.py` & `ukmon_meteortools-2023.5.6/ukmon_meteortools/rmsutils/plotRMSOrbits.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.5/ukmon_meteortools/rmsutils/trajPickle.py` & `ukmon_meteortools-2023.5.6/ukmon_meteortools/rmsutils/trajPickle.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.5/ukmon_meteortools/share/IMO_Working_Meteor_Shower_List.xml` & `ukmon_meteortools-2023.5.6/ukmon_meteortools/share/IMO_Working_Meteor_Shower_List.xml`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.5/ukmon_meteortools/share/__init__.py` & `ukmon_meteortools-2023.5.6/ukmon_meteortools/share/__init__.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.5/ukmon_meteortools/share/streamfulldata.npy` & `ukmon_meteortools-2023.5.6/ukmon_meteortools/share/streamfulldata.npy`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.5/ukmon_meteortools/usertools/apiExampleCode.py` & `ukmon_meteortools-2023.5.6/ukmon_meteortools/usertools/apiExampleCode.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.5/ukmon_meteortools/usertools/findNearDuplicates.py` & `ukmon_meteortools-2023.5.6/ukmon_meteortools/usertools/findNearDuplicates.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.5/ukmon_meteortools/usertools/getLiveImages.py` & `ukmon_meteortools-2023.5.6/ukmon_meteortools/usertools/getLiveImages.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.5/ukmon_meteortools/usertools/getOverlappingFovs.py` & `ukmon_meteortools-2023.5.6/ukmon_meteortools/usertools/getOverlappingFovs.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.5/ukmon_meteortools/usertools/plotTrack.py` & `ukmon_meteortools-2023.5.6/ukmon_meteortools/usertools/plotTrack.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.5/ukmon_meteortools/utils/Math.py` & `ukmon_meteortools-2023.5.6/ukmon_meteortools/utils/Math.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.5/ukmon_meteortools/utils/VectorMaths.py` & `ukmon_meteortools-2023.5.6/ukmon_meteortools/utils/VectorMaths.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.5/ukmon_meteortools/utils/__init__.py` & `ukmon_meteortools-2023.5.6/ukmon_meteortools/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.5/ukmon_meteortools/utils/annotateImage.py` & `ukmon_meteortools-2023.5.6/ukmon_meteortools/utils/annotateImage.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.5/ukmon_meteortools/utils/convertSolLon.py` & `ukmon_meteortools-2023.5.6/ukmon_meteortools/utils/convertSolLon.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.5/ukmon_meteortools/utils/drawFTPfile.py` & `ukmon_meteortools-2023.5.6/ukmon_meteortools/utils/drawFTPfile.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.5/ukmon_meteortools/utils/getActiveShowers.py` & `ukmon_meteortools-2023.5.6/ukmon_meteortools/utils/getActiveShowers.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.5/ukmon_meteortools/utils/getShowerDates.py` & `ukmon_meteortools-2023.5.6/ukmon_meteortools/utils/getShowerDates.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.5/ukmon_meteortools/utils/sendAnEmail.py` & `ukmon_meteortools-2023.5.6/ukmon_meteortools/utils/sendAnEmail.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.5/ukmon_meteortools.egg-info/PKG-INFO` & `ukmon_meteortools-2023.5.6/ukmon_meteortools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ukmon-meteortools
-Version: 2023.5.5
+Version: 2023.5.6
 Summary: Python Tools for Meteor Data Analysis
 Author-email: Mark McIntyre <ukmon@markmcintyreastro.co.uk>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ukmon_meteortools-2023.5.5/ukmon_meteortools.egg-info/SOURCES.txt` & `ukmon_meteortools-2023.5.6/ukmon_meteortools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

