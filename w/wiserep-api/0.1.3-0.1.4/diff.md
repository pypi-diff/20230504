# Comparing `tmp/wiserep_api-0.1.3.tar.gz` & `tmp/wiserep_api-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiserep_api-0.1.3.tar", last modified: Thu May  4 07:26:31 2023, max compression
+gzip compressed data, was "wiserep_api-0.1.4.tar", last modified: Thu May  4 08:11:59 2023, max compression
```

## Comparing `wiserep_api-0.1.3.tar` & `wiserep_api-0.1.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-04 07:26:31.086501 wiserep_api-0.1.3/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1080 2023-05-02 06:17:37.000000 wiserep_api-0.1.3/LICENSE
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       51 2023-05-04 05:31:12.000000 wiserep_api-0.1.3/MANIFEST.in
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4129 2023-05-04 07:26:31.086501 wiserep_api-0.1.3/PKG-INFO
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3641 2023-05-04 05:27:21.000000 wiserep_api-0.1.3/README.md
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       30 2023-05-02 08:10:24.000000 wiserep_api-0.1.3/requirements.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       38 2023-05-04 07:26:31.086501 wiserep_api-0.1.3/setup.cfg
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1134 2023-05-04 05:33:37.000000 wiserep_api-0.1.3/setup.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-04 07:26:31.086501 wiserep_api-0.1.3/tests/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)        0 2022-06-28 14:16:32.000000 wiserep_api-0.1.3/tests/__init__.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      309 2023-05-04 03:16:44.000000 wiserep_api-0.1.3/tests/test_classification.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2326 2023-05-04 07:16:40.000000 wiserep_api-0.1.3/tests/test_download_spectra.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      475 2023-05-04 07:25:36.000000 wiserep_api-0.1.3/tests/test_search.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-04 07:26:31.086501 wiserep_api-0.1.3/wiserep_api/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      266 2023-05-04 03:01:55.000000 wiserep_api-0.1.3/wiserep_api/__init__.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       46 2023-05-04 07:25:21.000000 wiserep_api-0.1.3/wiserep_api/_version.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2844 2023-05-04 07:21:49.000000 wiserep_api-0.1.3/wiserep_api/api.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1749 2023-05-03 06:34:19.000000 wiserep_api-0.1.3/wiserep_api/classification.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3433 2023-05-04 03:46:52.000000 wiserep_api-0.1.3/wiserep_api/search.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2878 2023-05-04 03:16:44.000000 wiserep_api-0.1.3/wiserep_api/snid.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5790 2023-05-04 07:19:34.000000 wiserep_api-0.1.3/wiserep_api/spectra.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-04 07:26:31.086501 wiserep_api-0.1.3/wiserep_api/static/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      744 2023-05-04 01:46:48.000000 wiserep_api-0.1.3/wiserep_api/static/spectral_types.json
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-04 07:26:31.086501 wiserep_api-0.1.3/wiserep_api.egg-info/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4129 2023-05-04 07:26:31.000000 wiserep_api-0.1.3/wiserep_api.egg-info/PKG-INFO
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      529 2023-05-04 07:26:31.000000 wiserep_api-0.1.3/wiserep_api.egg-info/SOURCES.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)        1 2023-05-04 07:26:31.000000 wiserep_api-0.1.3/wiserep_api.egg-info/dependency_links.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       30 2023-05-04 07:26:31.000000 wiserep_api-0.1.3/wiserep_api.egg-info/requires.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       18 2023-05-04 07:26:31.000000 wiserep_api-0.1.3/wiserep_api.egg-info/top_level.txt
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-04 08:11:59.140195 wiserep_api-0.1.4/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1080 2023-05-02 06:17:37.000000 wiserep_api-0.1.4/LICENSE
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       51 2023-05-04 05:31:12.000000 wiserep_api-0.1.4/MANIFEST.in
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4129 2023-05-04 08:11:59.140195 wiserep_api-0.1.4/PKG-INFO
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3641 2023-05-04 05:27:21.000000 wiserep_api-0.1.4/README.md
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       30 2023-05-02 08:10:24.000000 wiserep_api-0.1.4/requirements.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       38 2023-05-04 08:11:59.140195 wiserep_api-0.1.4/setup.cfg
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1134 2023-05-04 05:33:37.000000 wiserep_api-0.1.4/setup.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-04 08:11:59.136195 wiserep_api-0.1.4/tests/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)        0 2022-06-28 14:16:32.000000 wiserep_api-0.1.4/tests/__init__.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      309 2023-05-04 03:16:44.000000 wiserep_api-0.1.4/tests/test_classification.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2326 2023-05-04 07:16:40.000000 wiserep_api-0.1.4/tests/test_download_spectra.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      475 2023-05-04 07:25:36.000000 wiserep_api-0.1.4/tests/test_search.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-04 08:11:59.136195 wiserep_api-0.1.4/wiserep_api/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      266 2023-05-04 03:01:55.000000 wiserep_api-0.1.4/wiserep_api/__init__.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       46 2023-05-04 08:09:33.000000 wiserep_api-0.1.4/wiserep_api/_version.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2844 2023-05-04 07:21:49.000000 wiserep_api-0.1.4/wiserep_api/api.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1749 2023-05-03 06:34:19.000000 wiserep_api-0.1.4/wiserep_api/classification.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3433 2023-05-04 03:46:52.000000 wiserep_api-0.1.4/wiserep_api/search.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3427 2023-05-04 08:07:12.000000 wiserep_api-0.1.4/wiserep_api/snid.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5790 2023-05-04 07:19:34.000000 wiserep_api-0.1.4/wiserep_api/spectra.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-04 08:11:59.140195 wiserep_api-0.1.4/wiserep_api/static/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      744 2023-05-04 01:46:48.000000 wiserep_api-0.1.4/wiserep_api/static/spectral_types.json
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-04 08:11:59.140195 wiserep_api-0.1.4/wiserep_api.egg-info/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4129 2023-05-04 08:11:59.000000 wiserep_api-0.1.4/wiserep_api.egg-info/PKG-INFO
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      529 2023-05-04 08:11:59.000000 wiserep_api-0.1.4/wiserep_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)        1 2023-05-04 08:11:59.000000 wiserep_api-0.1.4/wiserep_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       30 2023-05-04 08:11:59.000000 wiserep_api-0.1.4/wiserep_api.egg-info/requires.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       18 2023-05-04 08:11:59.000000 wiserep_api-0.1.4/wiserep_api.egg-info/top_level.txt
```

### Comparing `wiserep_api-0.1.3/LICENSE` & `wiserep_api-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wiserep_api-0.1.3/PKG-INFO` & `wiserep_api-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiserep_api
-Version: 0.1.3
+Version: 0.1.4
 Summary: API to access WiserRep data from command lines
 Home-page: https://github.com/temuller/wiserep_api
 Author: Tomás Enrique Müller-Bravo
 Author-email: t.e.muller-bravo@ice.csic.es
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `wiserep_api-0.1.3/README.md` & `wiserep_api-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `wiserep_api-0.1.3/setup.py` & `wiserep_api-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `wiserep_api-0.1.3/tests/test_download_spectra.py` & `wiserep_api-0.1.4/tests/test_download_spectra.py`

 * *Files identical despite different names*

### Comparing `wiserep_api-0.1.3/wiserep_api/api.py` & `wiserep_api-0.1.4/wiserep_api/api.py`

 * *Files identical despite different names*

### Comparing `wiserep_api-0.1.3/wiserep_api/classification.py` & `wiserep_api-0.1.4/wiserep_api/classification.py`

 * *Files identical despite different names*

### Comparing `wiserep_api-0.1.3/wiserep_api/search.py` & `wiserep_api-0.1.4/wiserep_api/search.py`

 * *Files identical despite different names*

### Comparing `wiserep_api-0.1.3/wiserep_api/snid.py` & `wiserep_api-0.1.4/wiserep_api/snid.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,66 +21,82 @@
         if file.endswith(".fits") is False
         and "snid" not in file
         and "output" not in file
     ]
 
     # create a new file in the format that SNID likes
     for file in sn_files:
+        with open(file, 'r') as f:
+            first_line = f.readlines()[0]
+            if 'wave' not in first_line or 'flux' not in first_line:
+                # this is not a spectrum
+                continue
+            
         sn_df = pd.read_csv(file)
         snid_df = sn_df[["wave", "flux"]]
         outfile = os.path.splitext(file)[0] + ".snid"
         snid_df.to_csv(outfile, header=False, index=False, sep="\t")
 
 
-def run_snid(directory, command=None):
+def run_snid(directory, command=None, skip_fits=False):
     """Runs SNID on the given directory.
 
     SNID is run on all the files with spectra in the given directory.
     For more information, check the SNID website:
     https://people.lam.fr/blondin.stephane/software/snid/howto.html
 
     Parameters
     ----------
     directory : str
         Target's directory, e.g. ``spectra/2004eo``.
     command : str, optional
         SNID command. By default, ``snid inter=0 plot=0 aband=0`` is used.
+    skip_fits: bool, ``False``
+        Whether to skip files that were already run with SNID.
     """
     create_snid_inputs(directory)
 
     if command is None:
         command = "snid inter=0 plot=0 aband=0"
 
     # get SNID input files
     all_directory_files = glob.glob(os.path.join(directory, "*"))
     snid_files = [file for file in all_directory_files if file.endswith(".snid")]
 
     for file in snid_files:
-        # go to the SN directory, run SNID and come back
+        # get output file name
         basename = os.path.basename(file)
+        print_file = os.path.splitext(basename)[0]
+        snid_output = os.path.join(directory, f"{print_file}_snid.output")
+        
+        if skip_fits is True and os.path.isfile(snid_output) is True:
+            # skip this file that was previously fitted with SNID
+            continue
+
+        # go to the SN directory, run SNID and come back
         os.chdir(directory)
         os.system(f"{command} {basename}")
         os.chdir("../..")
 
-        # get SNID output file
-        print_file = os.path.splitext(basename)[0]
-        snid_output = os.path.join(directory, f"{print_file}_snid.output")
+        # remove temporary files
+        os.remove(file) 
+        snid_param_file = os.path.join(directory, "snid.param")
+        os.remove(snid_param_file)
+        
+        # check SNID output file
         if os.path.isfile(snid_output) is False:
-            print(f"No SNID output found for {print_file}! Probably a failed fit...")
+            print(f"\nNo SNID output found for {print_file}! Probably a failed fit...")
+            
             continue
 
+        # get SNID output and "clean" it
         with open(snid_output) as f:
             skiprows = 0
             for i, line in enumerate(f.readlines()):
                 if line.startswith("#no. sn type"):
                     break
                 skiprows += 1
 
+        # save new output
         output_df = pd.read_csv(snid_output, skiprows=skiprows, delim_whitespace=True)
         output_df = output_df[output_df.grade == "good"]  # keep only the good fits
-        # outfile = os.path.join(directory, f'output_{basename.split(".")[0]}.txt')
         output_df.to_csv(snid_output, index=False)
-
-        # clean directory:
-        os.remove(file)
-        snid_param_file = os.path.join(directory, "snid.param")
-        os.remove(snid_param_file)
```

### Comparing `wiserep_api-0.1.3/wiserep_api/spectra.py` & `wiserep_api-0.1.4/wiserep_api/spectra.py`

 * *Files identical despite different names*

### Comparing `wiserep_api-0.1.3/wiserep_api/static/spectral_types.json` & `wiserep_api-0.1.4/wiserep_api/static/spectral_types.json`

 * *Files identical despite different names*

### Comparing `wiserep_api-0.1.3/wiserep_api.egg-info/PKG-INFO` & `wiserep_api-0.1.4/wiserep_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiserep-api
-Version: 0.1.3
+Version: 0.1.4
 Summary: API to access WiserRep data from command lines
 Home-page: https://github.com/temuller/wiserep_api
 Author: Tomás Enrique Müller-Bravo
 Author-email: t.e.muller-bravo@ice.csic.es
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `wiserep_api-0.1.3/wiserep_api.egg-info/SOURCES.txt` & `wiserep_api-0.1.4/wiserep_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

