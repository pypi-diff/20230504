# Comparing `tmp/ismrmrd-1.9.7.tar.gz` & `tmp/ismrmrd-1.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ismrmrd-1.9.7.tar", last modified: Fri Mar  4 22:56:15 2022, max compression
+gzip compressed data, was "ismrmrd-1.9.8.tar", last modified: Fri Mar  4 23:21:34 2022, max compression
```

## Comparing `ismrmrd-1.9.7.tar` & `ismrmrd-1.9.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 22:56:15.685305 ismrmrd-1.9.7/
--rw-r--r--   0 runner    (1001) docker     (121)     1740 2022-03-04 22:55:47.000000 ismrmrd-1.9.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-03-04 22:55:47.000000 ismrmrd-1.9.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      555 2022-03-04 22:56:15.685305 ismrmrd-1.9.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-03-04 22:55:47.000000 ismrmrd-1.9.7/README
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 22:56:15.685305 ismrmrd-1.9.7/ismrmrd/
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-03-04 22:55:47.000000 ismrmrd-1.9.7/ismrmrd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9319 2022-03-04 22:55:47.000000 ismrmrd-1.9.7/ismrmrd/acquisition.py
--rw-r--r--   0 runner    (1001) docker     (121)     2810 2022-03-04 22:55:47.000000 ismrmrd-1.9.7/ismrmrd/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)      393 2022-03-04 22:55:47.000000 ismrmrd-1.9.7/ismrmrd/equality.py
--rw-r--r--   0 runner    (1001) docker     (121)    10829 2022-03-04 22:55:47.000000 ismrmrd-1.9.7/ismrmrd/file.py
--rw-r--r--   0 runner    (1001) docker     (121)      566 2022-03-04 22:55:47.000000 ismrmrd-1.9.7/ismrmrd/flags.py
--rw-r--r--   0 runner    (1001) docker     (121)    13975 2022-03-04 22:55:47.000000 ismrmrd-1.9.7/ismrmrd/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (121)    12142 2022-03-04 22:55:47.000000 ismrmrd-1.9.7/ismrmrd/image.py
--rw-r--r--   0 runner    (1001) docker     (121)     2730 2022-03-04 22:55:47.000000 ismrmrd-1.9.7/ismrmrd/meta.py
--rw-r--r--   0 runner    (1001) docker     (121)     4968 2022-03-04 22:55:47.000000 ismrmrd-1.9.7/ismrmrd/waveform.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 22:56:15.685305 ismrmrd-1.9.7/ismrmrd/xsd/
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-03-04 22:55:47.000000 ismrmrd-1.9.7/ismrmrd/xsd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      958 2022-03-04 22:55:47.000000 ismrmrd-1.9.7/ismrmrd/xsd/pyxb_compat.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 22:56:15.685305 ismrmrd-1.9.7/ismrmrd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      555 2022-03-04 22:56:15.000000 ismrmrd-1.9.7/ismrmrd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      470 2022-03-04 22:56:15.000000 ismrmrd-1.9.7/ismrmrd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-04 22:56:15.000000 ismrmrd-1.9.7/ismrmrd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-03-04 22:56:15.000000 ismrmrd-1.9.7/ismrmrd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-03-04 22:56:15.000000 ismrmrd-1.9.7/ismrmrd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-03-04 22:55:47.000000 ismrmrd-1.9.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 22:56:15.685305 ismrmrd-1.9.7/schema/
--rw-r--r--   0 runner    (1001) docker     (121)    13930 2022-03-04 22:55:47.000000 ismrmrd-1.9.7/schema/ismrmrd.xsd
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-03-04 22:56:15.689305 ismrmrd-1.9.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2362 2022-03-04 22:55:47.000000 ismrmrd-1.9.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 23:21:34.083099 ismrmrd-1.9.8/
+-rw-r--r--   0 runner    (1001) docker     (121)     1740 2022-03-04 23:21:08.000000 ismrmrd-1.9.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       67 2022-03-04 23:21:08.000000 ismrmrd-1.9.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      555 2022-03-04 23:21:34.083099 ismrmrd-1.9.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2022-03-04 23:21:08.000000 ismrmrd-1.9.8/README
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 23:21:34.083099 ismrmrd-1.9.8/ismrmrd/
+-rw-r--r--   0 runner    (1001) docker     (121)      190 2022-03-04 23:21:08.000000 ismrmrd-1.9.8/ismrmrd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9319 2022-03-04 23:21:08.000000 ismrmrd-1.9.8/ismrmrd/acquisition.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2900 2022-03-04 23:21:08.000000 ismrmrd-1.9.8/ismrmrd/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)      393 2022-03-04 23:21:08.000000 ismrmrd-1.9.8/ismrmrd/equality.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10829 2022-03-04 23:21:08.000000 ismrmrd-1.9.8/ismrmrd/file.py
+-rw-r--r--   0 runner    (1001) docker     (121)      566 2022-03-04 23:21:08.000000 ismrmrd-1.9.8/ismrmrd/flags.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13975 2022-03-04 23:21:08.000000 ismrmrd-1.9.8/ismrmrd/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12142 2022-03-04 23:21:08.000000 ismrmrd-1.9.8/ismrmrd/image.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2730 2022-03-04 23:21:08.000000 ismrmrd-1.9.8/ismrmrd/meta.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4968 2022-03-04 23:21:08.000000 ismrmrd-1.9.8/ismrmrd/waveform.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 23:21:34.083099 ismrmrd-1.9.8/ismrmrd/xsd/
+-rw-r--r--   0 runner    (1001) docker     (121)       90 2022-03-04 23:21:08.000000 ismrmrd-1.9.8/ismrmrd/xsd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      958 2022-03-04 23:21:08.000000 ismrmrd-1.9.8/ismrmrd/xsd/pyxb_compat.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 23:21:34.083099 ismrmrd-1.9.8/ismrmrd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      555 2022-03-04 23:21:33.000000 ismrmrd-1.9.8/ismrmrd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      470 2022-03-04 23:21:34.000000 ismrmrd-1.9.8/ismrmrd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-04 23:21:33.000000 ismrmrd-1.9.8/ismrmrd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2022-03-04 23:21:34.000000 ismrmrd-1.9.8/ismrmrd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-03-04 23:21:34.000000 ismrmrd-1.9.8/ismrmrd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      121 2022-03-04 23:21:08.000000 ismrmrd-1.9.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 23:21:34.083099 ismrmrd-1.9.8/schema/
+-rw-r--r--   0 runner    (1001) docker     (121)    13930 2022-03-04 23:21:08.000000 ismrmrd-1.9.8/schema/ismrmrd.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)       85 2022-03-04 23:21:34.083099 ismrmrd-1.9.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2362 2022-03-04 23:21:08.000000 ismrmrd-1.9.8/setup.py
```

### Comparing `ismrmrd-1.9.7/LICENSE` & `ismrmrd-1.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ismrmrd-1.9.7/PKG-INFO` & `ismrmrd-1.9.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ismrmrd
-Version: 1.9.7
+Version: 1.9.8
 Summary: Python implementation of the ISMRMRD
 Home-page: https://ismrmrd.github.io
 Author: ISMRMRD Developers
 Author-email: dchansen@gradientsoftware.net
 License: Public Domain
 Keywords: ismrmrd
 Platform: UNKNOWN
```

### Comparing `ismrmrd-1.9.7/ismrmrd/acquisition.py` & `ismrmrd-1.9.8/ismrmrd/acquisition.py`

 * *Files identical despite different names*

### Comparing `ismrmrd-1.9.7/ismrmrd/constants.py` & `ismrmrd-1.9.8/ismrmrd/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,14 +43,16 @@
 ACQ_IS_NAVIGATION_DATA                  = 23
 ACQ_IS_PHASECORR_DATA                   = 24
 ACQ_LAST_IN_MEASUREMENT                 = 25
 ACQ_IS_HPFEEDBACK_DATA                  = 26
 ACQ_IS_DUMMYSCAN_DATA                   = 27
 ACQ_IS_RTFEEDBACK_DATA                  = 28
 ACQ_IS_SURFACECOILCORRECTIONSCAN_DATA   = 29
+ACQ_IS_PHASE_STABILIZATION_REFERENCE    = 30
+ACQ_IS_PHASE_STABILIZATION              = 31
 ACQ_COMPRESSION1                        = 53
 ACQ_COMPRESSION2                        = 54
 ACQ_COMPRESSION3                        = 55
 ACQ_COMPRESSION4                        = 56
 ACQ_USER1                               = 57
 ACQ_USER2                               = 58
 ACQ_USER3                               = 59
```

### Comparing `ismrmrd-1.9.7/ismrmrd/file.py` & `ismrmrd-1.9.8/ismrmrd/file.py`

 * *Files identical despite different names*

### Comparing `ismrmrd-1.9.7/ismrmrd/flags.py` & `ismrmrd-1.9.8/ismrmrd/flags.py`

 * *Files identical despite different names*

### Comparing `ismrmrd-1.9.7/ismrmrd/hdf5.py` & `ismrmrd-1.9.8/ismrmrd/hdf5.py`

 * *Files identical despite different names*

### Comparing `ismrmrd-1.9.7/ismrmrd/image.py` & `ismrmrd-1.9.8/ismrmrd/image.py`

 * *Files identical despite different names*

### Comparing `ismrmrd-1.9.7/ismrmrd/meta.py` & `ismrmrd-1.9.8/ismrmrd/meta.py`

 * *Files identical despite different names*

### Comparing `ismrmrd-1.9.7/ismrmrd/waveform.py` & `ismrmrd-1.9.8/ismrmrd/waveform.py`

 * *Files identical despite different names*

### Comparing `ismrmrd-1.9.7/ismrmrd/xsd/pyxb_compat.py` & `ismrmrd-1.9.8/ismrmrd/xsd/pyxb_compat.py`

 * *Files identical despite different names*

### Comparing `ismrmrd-1.9.7/ismrmrd.egg-info/PKG-INFO` & `ismrmrd-1.9.8/ismrmrd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ismrmrd
-Version: 1.9.7
+Version: 1.9.8
 Summary: Python implementation of the ISMRMRD
 Home-page: https://ismrmrd.github.io
 Author: ISMRMRD Developers
 Author-email: dchansen@gradientsoftware.net
 License: Public Domain
 Keywords: ismrmrd
 Platform: UNKNOWN
```

### Comparing `ismrmrd-1.9.7/schema/ismrmrd.xsd` & `ismrmrd-1.9.8/schema/ismrmrd.xsd`

 * *Files identical despite different names*

### Comparing `ismrmrd-1.9.7/setup.py` & `ismrmrd-1.9.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     subprocess.run(args)
     fix_init_file(subpackage_name,f"{subpackage_name}/__init__.py")
     shutil.rmtree(os.path.join(outloc,subpackage_name),ignore_errors=True)
     shutil.move(subpackage_name,outloc)
 
 setup(
     name='ismrmrd',
-    version='1.9.7',
+    version='1.9.8',
     author='ISMRMRD Developers',
     author_email='dchansen@gradientsoftware.net',
     description='Python implementation of the ISMRMRD',
     license='Public Domain',
     keywords='ismrmrd',
     url='https://ismrmrd.github.io',
     packages=find_packages(),
```

