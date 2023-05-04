# Comparing `tmp/wiserep_api-0.1.2.tar.gz` & `tmp/wiserep_api-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiserep_api-0.1.2.tar", last modified: Thu May  4 05:35:25 2023, max compression
+gzip compressed data, was "wiserep_api-0.1.3.tar", last modified: Thu May  4 07:26:31 2023, max compression
```

## Comparing `wiserep_api-0.1.2.tar` & `wiserep_api-0.1.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-04 05:35:25.635905 wiserep_api-0.1.2/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1080 2023-05-02 06:17:37.000000 wiserep_api-0.1.2/LICENSE
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       51 2023-05-04 05:31:12.000000 wiserep_api-0.1.2/MANIFEST.in
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4129 2023-05-04 05:35:25.635905 wiserep_api-0.1.2/PKG-INFO
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3641 2023-05-04 05:27:21.000000 wiserep_api-0.1.2/README.md
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       30 2023-05-02 08:10:24.000000 wiserep_api-0.1.2/requirements.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       38 2023-05-04 05:35:25.635905 wiserep_api-0.1.2/setup.cfg
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1134 2023-05-04 05:33:37.000000 wiserep_api-0.1.2/setup.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-04 05:35:25.631905 wiserep_api-0.1.2/tests/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)        0 2022-06-28 14:16:32.000000 wiserep_api-0.1.2/tests/__init__.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      309 2023-05-04 03:16:44.000000 wiserep_api-0.1.2/tests/test_classification.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2246 2023-05-04 03:16:44.000000 wiserep_api-0.1.2/tests/test_download_spectra.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      387 2023-05-04 03:16:44.000000 wiserep_api-0.1.2/tests/test_search.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-04 05:35:25.631905 wiserep_api-0.1.2/wiserep_api/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      266 2023-05-04 03:01:55.000000 wiserep_api-0.1.2/wiserep_api/__init__.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       46 2023-05-04 05:34:36.000000 wiserep_api-0.1.2/wiserep_api/_version.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2910 2023-05-03 06:34:19.000000 wiserep_api-0.1.2/wiserep_api/api.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1749 2023-05-03 06:34:19.000000 wiserep_api-0.1.2/wiserep_api/classification.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3433 2023-05-04 03:46:52.000000 wiserep_api-0.1.2/wiserep_api/search.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2878 2023-05-04 03:16:44.000000 wiserep_api-0.1.2/wiserep_api/snid.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5782 2023-05-03 06:34:19.000000 wiserep_api-0.1.2/wiserep_api/spectra.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-04 05:35:25.635905 wiserep_api-0.1.2/wiserep_api/static/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      744 2023-05-04 01:46:48.000000 wiserep_api-0.1.2/wiserep_api/static/spectral_types.json
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-04 05:35:25.635905 wiserep_api-0.1.2/wiserep_api.egg-info/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4129 2023-05-04 05:35:25.000000 wiserep_api-0.1.2/wiserep_api.egg-info/PKG-INFO
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      529 2023-05-04 05:35:25.000000 wiserep_api-0.1.2/wiserep_api.egg-info/SOURCES.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)        1 2023-05-04 05:35:25.000000 wiserep_api-0.1.2/wiserep_api.egg-info/dependency_links.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       30 2023-05-04 05:35:25.000000 wiserep_api-0.1.2/wiserep_api.egg-info/requires.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       18 2023-05-04 05:35:25.000000 wiserep_api-0.1.2/wiserep_api.egg-info/top_level.txt
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-04 07:26:31.086501 wiserep_api-0.1.3/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1080 2023-05-02 06:17:37.000000 wiserep_api-0.1.3/LICENSE
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       51 2023-05-04 05:31:12.000000 wiserep_api-0.1.3/MANIFEST.in
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4129 2023-05-04 07:26:31.086501 wiserep_api-0.1.3/PKG-INFO
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3641 2023-05-04 05:27:21.000000 wiserep_api-0.1.3/README.md
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       30 2023-05-02 08:10:24.000000 wiserep_api-0.1.3/requirements.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       38 2023-05-04 07:26:31.086501 wiserep_api-0.1.3/setup.cfg
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1134 2023-05-04 05:33:37.000000 wiserep_api-0.1.3/setup.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-04 07:26:31.086501 wiserep_api-0.1.3/tests/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)        0 2022-06-28 14:16:32.000000 wiserep_api-0.1.3/tests/__init__.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      309 2023-05-04 03:16:44.000000 wiserep_api-0.1.3/tests/test_classification.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2326 2023-05-04 07:16:40.000000 wiserep_api-0.1.3/tests/test_download_spectra.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      475 2023-05-04 07:25:36.000000 wiserep_api-0.1.3/tests/test_search.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-04 07:26:31.086501 wiserep_api-0.1.3/wiserep_api/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      266 2023-05-04 03:01:55.000000 wiserep_api-0.1.3/wiserep_api/__init__.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       46 2023-05-04 07:25:21.000000 wiserep_api-0.1.3/wiserep_api/_version.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2844 2023-05-04 07:21:49.000000 wiserep_api-0.1.3/wiserep_api/api.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1749 2023-05-03 06:34:19.000000 wiserep_api-0.1.3/wiserep_api/classification.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3433 2023-05-04 03:46:52.000000 wiserep_api-0.1.3/wiserep_api/search.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2878 2023-05-04 03:16:44.000000 wiserep_api-0.1.3/wiserep_api/snid.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5790 2023-05-04 07:19:34.000000 wiserep_api-0.1.3/wiserep_api/spectra.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-04 07:26:31.086501 wiserep_api-0.1.3/wiserep_api/static/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      744 2023-05-04 01:46:48.000000 wiserep_api-0.1.3/wiserep_api/static/spectral_types.json
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-04 07:26:31.086501 wiserep_api-0.1.3/wiserep_api.egg-info/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4129 2023-05-04 07:26:31.000000 wiserep_api-0.1.3/wiserep_api.egg-info/PKG-INFO
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      529 2023-05-04 07:26:31.000000 wiserep_api-0.1.3/wiserep_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)        1 2023-05-04 07:26:31.000000 wiserep_api-0.1.3/wiserep_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       30 2023-05-04 07:26:31.000000 wiserep_api-0.1.3/wiserep_api.egg-info/requires.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       18 2023-05-04 07:26:31.000000 wiserep_api-0.1.3/wiserep_api.egg-info/top_level.txt
```

### Comparing `wiserep_api-0.1.2/LICENSE` & `wiserep_api-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wiserep_api-0.1.2/PKG-INFO` & `wiserep_api-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiserep_api
-Version: 0.1.2
+Version: 0.1.3
 Summary: API to access WiserRep data from command lines
 Home-page: https://github.com/temuller/wiserep_api
 Author: Tomás Enrique Müller-Bravo
 Author-email: t.e.muller-bravo@ice.csic.es
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `wiserep_api-0.1.2/README.md` & `wiserep_api-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `wiserep_api-0.1.2/setup.py` & `wiserep_api-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `wiserep_api-0.1.2/tests/test_download_spectra.py` & `wiserep_api-0.1.3/tests/test_download_spectra.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import os
 import glob
+import shutil
 import unittest
 import numpy as np
 import warnings
 from astropy.utils.exceptions import AstropyWarning
 from wiserep_api import download_target_spectra
 
+if os.path.isdir('spectra') is True:
+    shutil.rmtree('spectra')
 
 class TestDownloadSpectra(unittest.TestCase):
     def test_download_spectra(self):
         target = "ASASSN-14jg"
         with warnings.catch_warnings():
             warnings.simplefilter("ignore", AstropyWarning)
             download_target_spectra(target)
```

### Comparing `wiserep_api-0.1.2/wiserep_api/api.py` & `wiserep_api-0.1.3/wiserep_api/api.py`

 * *Files 11% similar despite different names*

```diff
@@ -40,15 +40,16 @@
 
     ###############################################################
     response = requests.get(url, headers=headers)
 
     if response.status_code == 200:
         return response
     else:
-        print(http_errors[response.status_code])
+        print('Response error:', http_errors[response.status_code])
+        print(url)
         return None
 
 
 def get_object_id(iau_name, verbose=False):
     """Obtains the objects's Wiserep ID.
 
     Parameters
@@ -61,31 +62,30 @@
     Returns
     -------
     obj_id: str
         The object's Wiserep ID. Returns 'Unknown' if not found
         or None if there is a problem of some other kind.
     """
     # look for the target ID in the search webpage
-    wiserep_search_url = "https://www.wiserep.org/search?name="
-    target_search_url = wiserep_search_url + iau_name
+    wiserep_search_url = "https://www.wiserep.org/search?"
+    search_name = iau_name.replace('+', '%2B')  # is this an html thing?
+    target_search_url = wiserep_search_url + f'name={search_name}&name_like=1'
     response = get_response(target_search_url)
     if response is None:
+        print(f'Could not load the webpage of {iau_name}')
         return None
 
-    split_text = response.text.split('href="/object/')
-    if len(split_text) < 2:
-        print(f"No target with this name found on Wiserep: {iau_name}")
-        return "Unknown"
-    else:
-        obj_id = None  # return None if object ID is not found
-        for line in split_text:
-            # check only the lines at the bottom of the search page
-            if "Click to Object page" in line:
-                if (f"{iau_name}</a>" in line) or (f"{iau_name}, " in line):
-                    obj_id = line.split('"')[0]
-        if verbose:
-            print("Object ID (Wiserep):", obj_id)
+    obj_id = None
+    split_text = response.text.split('="Click to Object page">')
+    for st in split_text:
+        if f'{iau_name}<' in st:
+            if 'href="/object/' in st:
+                obj_id = st.split('href="/object/')[1].split('"')[0]
+                break
+            
+    if verbose:
+        print("Object ID (Wiserep):", obj_id)
 
-        if obj_id is None:
-            print(f"No target with this name found on Wiserep: {iau_name}")
-
-        return obj_id
+    if obj_id is None:
+        print(f"No target with this name found on Wiserep: {iau_name}")
+    
+    return obj_id
```

### Comparing `wiserep_api-0.1.2/wiserep_api/classification.py` & `wiserep_api-0.1.3/wiserep_api/classification.py`

 * *Files identical despite different names*

### Comparing `wiserep_api-0.1.2/wiserep_api/search.py` & `wiserep_api-0.1.3/wiserep_api/search.py`

 * *Files identical despite different names*

### Comparing `wiserep_api-0.1.2/wiserep_api/snid.py` & `wiserep_api-0.1.3/wiserep_api/snid.py`

 * *Files identical despite different names*

### Comparing `wiserep_api-0.1.2/wiserep_api/spectra.py` & `wiserep_api-0.1.3/wiserep_api/spectra.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
     split_text = response.text.split("asciifile=https%3A//")
     for st in split_text:
         url = st.split('"')[0]
         if (url not in txt_urls) and ("&amp" not in url) and ("DOCTYPE" not in url):
             txt_urls.append(url)
     if verbose is True:
         print(f"Found {len(txt_urls)} URLs with spectra (ASCII): {txt_urls}")
-
+        
     # FITS
     fits_urls = []
     split_text = response.text.split("https://")
     for st in split_text:
         url = st.split('"')[0]
         if (url not in fits_urls) and (".fits" in url) and ("rel-file" not in url):
             fits_urls.append(url)
```

### Comparing `wiserep_api-0.1.2/wiserep_api/static/spectral_types.json` & `wiserep_api-0.1.3/wiserep_api/static/spectral_types.json`

 * *Files identical despite different names*

### Comparing `wiserep_api-0.1.2/wiserep_api.egg-info/PKG-INFO` & `wiserep_api-0.1.3/wiserep_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiserep-api
-Version: 0.1.2
+Version: 0.1.3
 Summary: API to access WiserRep data from command lines
 Home-page: https://github.com/temuller/wiserep_api
 Author: Tomás Enrique Müller-Bravo
 Author-email: t.e.muller-bravo@ice.csic.es
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `wiserep_api-0.1.2/wiserep_api.egg-info/SOURCES.txt` & `wiserep_api-0.1.3/wiserep_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

