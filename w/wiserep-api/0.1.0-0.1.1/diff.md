# Comparing `tmp/wiserep_api-0.1.0.tar.gz` & `tmp/wiserep_api-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiserep_api-0.1.0.tar", last modified: Wed May  3 05:14:05 2023, max compression
+gzip compressed data, was "wiserep_api-0.1.1.tar", last modified: Thu May  4 05:24:09 2023, max compression
```

## Comparing `wiserep_api-0.1.0.tar` & `wiserep_api-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-03 05:14:05.114794 wiserep_api-0.1.0/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1080 2023-05-02 06:17:37.000000 wiserep_api-0.1.0/LICENSE
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       25 2023-05-02 06:18:42.000000 wiserep_api-0.1.0/MANIFEST.in
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      548 2023-05-03 05:14:05.110794 wiserep_api-0.1.0/PKG-INFO
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       61 2023-05-02 06:17:37.000000 wiserep_api-0.1.0/README.md
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       30 2023-05-02 08:10:24.000000 wiserep_api-0.1.0/requirements.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       38 2023-05-03 05:14:05.114794 wiserep_api-0.1.0/setup.cfg
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1160 2023-05-02 06:19:51.000000 wiserep_api-0.1.0/setup.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-03 05:14:05.110794 wiserep_api-0.1.0/tests/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)        0 2022-06-28 14:16:32.000000 wiserep_api-0.1.0/tests/__init__.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      309 2023-05-02 08:13:25.000000 wiserep_api-0.1.0/tests/test_classification.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2246 2023-05-03 05:07:24.000000 wiserep_api-0.1.0/tests/test_download_spectra.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-03 05:14:05.110794 wiserep_api-0.1.0/wiserep_api/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      180 2023-05-02 08:10:59.000000 wiserep_api-0.1.0/wiserep_api/__init__.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       45 2023-05-02 06:29:00.000000 wiserep_api-0.1.0/wiserep_api/_version.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2991 2023-05-02 10:15:31.000000 wiserep_api-0.1.0/wiserep_api/api.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1763 2023-05-02 08:11:41.000000 wiserep_api-0.1.0/wiserep_api/classification.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5884 2023-05-03 03:28:29.000000 wiserep_api-0.1.0/wiserep_api/spectra.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-03 05:14:05.110794 wiserep_api-0.1.0/wiserep_api.egg-info/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      548 2023-05-03 05:14:05.000000 wiserep_api-0.1.0/wiserep_api.egg-info/PKG-INFO
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      427 2023-05-03 05:14:05.000000 wiserep_api-0.1.0/wiserep_api.egg-info/SOURCES.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)        1 2023-05-03 05:14:05.000000 wiserep_api-0.1.0/wiserep_api.egg-info/dependency_links.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       30 2023-05-03 05:14:05.000000 wiserep_api-0.1.0/wiserep_api.egg-info/requires.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       18 2023-05-03 05:14:05.000000 wiserep_api-0.1.0/wiserep_api.egg-info/top_level.txt
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-04 05:24:09.175104 wiserep_api-0.1.1/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1080 2023-05-02 06:17:37.000000 wiserep_api-0.1.1/LICENSE
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       25 2023-05-02 06:18:42.000000 wiserep_api-0.1.1/MANIFEST.in
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4106 2023-05-04 05:24:09.175104 wiserep_api-0.1.1/PKG-INFO
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3618 2023-05-04 05:21:20.000000 wiserep_api-0.1.1/README.md
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       30 2023-05-02 08:10:24.000000 wiserep_api-0.1.1/requirements.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       38 2023-05-04 05:24:09.175104 wiserep_api-0.1.1/setup.cfg
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1161 2023-05-03 06:34:19.000000 wiserep_api-0.1.1/setup.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-04 05:24:09.171104 wiserep_api-0.1.1/tests/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)        0 2022-06-28 14:16:32.000000 wiserep_api-0.1.1/tests/__init__.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      309 2023-05-04 03:16:44.000000 wiserep_api-0.1.1/tests/test_classification.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2246 2023-05-04 03:16:44.000000 wiserep_api-0.1.1/tests/test_download_spectra.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      387 2023-05-04 03:16:44.000000 wiserep_api-0.1.1/tests/test_search.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-04 05:24:09.171104 wiserep_api-0.1.1/wiserep_api/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      266 2023-05-04 03:01:55.000000 wiserep_api-0.1.1/wiserep_api/__init__.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       46 2023-05-04 05:23:20.000000 wiserep_api-0.1.1/wiserep_api/_version.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2910 2023-05-03 06:34:19.000000 wiserep_api-0.1.1/wiserep_api/api.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1749 2023-05-03 06:34:19.000000 wiserep_api-0.1.1/wiserep_api/classification.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3433 2023-05-04 03:46:52.000000 wiserep_api-0.1.1/wiserep_api/search.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2878 2023-05-04 03:16:44.000000 wiserep_api-0.1.1/wiserep_api/snid.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5782 2023-05-03 06:34:19.000000 wiserep_api-0.1.1/wiserep_api/spectra.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-04 05:24:09.175104 wiserep_api-0.1.1/wiserep_api.egg-info/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4106 2023-05-04 05:24:09.000000 wiserep_api-0.1.1/wiserep_api.egg-info/PKG-INFO
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      490 2023-05-04 05:24:09.000000 wiserep_api-0.1.1/wiserep_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)        1 2023-05-04 05:24:09.000000 wiserep_api-0.1.1/wiserep_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       30 2023-05-04 05:24:09.000000 wiserep_api-0.1.1/wiserep_api.egg-info/requires.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       18 2023-05-04 05:24:09.000000 wiserep_api-0.1.1/wiserep_api.egg-info/top_level.txt
```

### Comparing `wiserep_api-0.1.0/LICENSE` & `wiserep_api-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wiserep_api-0.1.0/setup.py` & `wiserep_api-0.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,10 +25,10 @@
     python_requires=">=3.8",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=requirements,
-    #package_data={"idsred": ["lamps/*", "standards/*", "extinction/*"]},
+    # package_data={"idsred": ["lamps/*", "standards/*", "extinction/*"]},
     include_package_data=True,
 )
```

### Comparing `wiserep_api-0.1.0/tests/test_download_spectra.py` & `wiserep_api-0.1.1/tests/test_download_spectra.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,57 +1,58 @@
 import os
 import glob
 import unittest
 import numpy as np
 import warnings
 from astropy.utils.exceptions import AstropyWarning
-from wiserep_api import download_target_spectra 
+from wiserep_api import download_target_spectra
 
 
 class TestDownloadSpectra(unittest.TestCase):
     def test_download_spectra(self):
-        target = 'ASASSN-14jg'
+        target = "ASASSN-14jg"
         with warnings.catch_warnings():
             warnings.simplefilter("ignore", AstropyWarning)
             download_target_spectra(target)
-        files = glob.glob(os.path.join('spectra', target, '*'))
+        files = glob.glob(os.path.join("spectra", target, "*"))
 
-        txt_files = [file for file in files if '.fits' not in file]
+        txt_files = [file for file in files if ".fits" not in file]
         err_msg = "Number of files does not match (ASCII)"
         np.testing.assert_equal(len(txt_files), 5, err_msg)
 
-        fits_files = [file for file in files if '.fits' in file]
+        fits_files = [file for file in files if ".fits" in file]
         err_msg = "Number of files does not match (FITS)"
         np.testing.assert_equal(len(fits_files), 3, err_msg)
 
     def test_exclude(self):
-        target = '2017ixi'
+        target = "2017ixi"
         with warnings.catch_warnings():
             warnings.simplefilter("ignore", AstropyWarning)
-            download_target_spectra(target, exclude=['PESSTO'])
-        files = glob.glob(os.path.join('spectra', target, '*'))
+            download_target_spectra(target, exclude=["PESSTO"])
+        files = glob.glob(os.path.join("spectra", target, "*"))
 
-        txt_files = [file for file in files if '.fits' not in file]
+        txt_files = [file for file in files if ".fits" not in file]
         err_msg = "There should be no files downloaded (ASCII)"
         np.testing.assert_equal(len(txt_files), 0, err_msg)
 
-        fits_files = [file for file in files if '.fits' in file]
+        fits_files = [file for file in files if ".fits" in file]
         err_msg = "There should be no files downloaded (FITS)"
         np.testing.assert_equal(len(fits_files), 0, err_msg)
 
     def test_include(self):
-        target = 'ASASSN-14hr'
+        target = "ASASSN-14hr"
         with warnings.catch_warnings():
             warnings.simplefilter("ignore", AstropyWarning)
-            download_target_spectra(target, include=['WiFeS'])
-        files = glob.glob(os.path.join('spectra', target, '*'))
+            download_target_spectra(target, include=["WiFeS"])
+        files = glob.glob(os.path.join("spectra", target, "*"))
 
-        txt_files = [file for file in files if '.fits' not in file]
+        txt_files = [file for file in files if ".fits" not in file]
         err_msg = "Number of files does not match (ASCII)"
         np.testing.assert_equal(len(txt_files), 2, err_msg)
 
-        fits_files = [file for file in files if '.fits' in file]
+        fits_files = [file for file in files if ".fits" in file]
         err_msg = "Number of files does not match (FITS)"
         np.testing.assert_equal(len(fits_files), 2, err_msg)
 
+
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `wiserep_api-0.1.0/wiserep_api/api.py` & `wiserep_api-0.1.1/wiserep_api/api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,87 +1,91 @@
 import requests
 
+
 def get_response(url):
     """Obtains the response from a given Wiserep URL.
-    
+
     Parameters
     ----------
     url: str
         Wiserep URL.
-        
+
     Returns
     -------
     response: requests.Response
         Response object.
     """
     # ID of your Bot:
-    YOUR_BOT_ID=1234
+    YOUR_BOT_ID = 1234
     # name of your Bot:
-    YOUR_BOT_NAME="My_Bot1"
+    YOUR_BOT_NAME = "My_Bot1"
     # API key of your Bot:
-    api_key="604d60d302f86eb38fd1407abe41d05b438043bd"
+    api_key = "604d60d302f86eb38fd1407abe41d05b438043bd"
 
-    headers={'User-Agent':'tns_marker{"tns_id":'+str(YOUR_BOT_ID)+', "type":"bot",'\
-                 ' "name":"'+YOUR_BOT_NAME+'"}'}
-    
-    http_errors = {                                                                               
-    304: 'Error 304: Not Modified: There was no new data to return.',
-    400: 'Error 400: Bad Request: The request was invalid. '\
-         'An accompanying error message will explain why.',
-    403: 'Error 403: Forbidden: The request is understood, but it has '\
-         'been refused. An accompanying error message will explain why.',
-    404: 'Error 404: Not Found: The URI requested is invalid or the '\
-         'resource requested, such as a category, does not exists.',
-    500: 'Error 500: Internal Server Error: Something is broken.',
-    503: 'Error 503: Service Unavailable.'
+    headers = {
+        "User-Agent": 'tns_marker{"tns_id":' + str(YOUR_BOT_ID) + ', "type":"bot",'
+        ' "name":"' + YOUR_BOT_NAME + '"}'
     }
-    
+
+    http_errors = {
+        304: "Error 304: Not Modified: There was no new data to return.",
+        400: "Error 400: Bad Request: The request was invalid. "
+        "An accompanying error message will explain why.",
+        403: "Error 403: Forbidden: The request is understood, but it has "
+        "been refused. An accompanying error message will explain why.",
+        404: "Error 404: Not Found: The URI requested is invalid or the "
+        "resource requested, such as a category, does not exists.",
+        500: "Error 500: Internal Server Error: Something is broken.",
+        503: "Error 503: Service Unavailable.",
+    }
+
     ###############################################################
     response = requests.get(url, headers=headers)
 
     if response.status_code == 200:
         return response
     else:
         print(http_errors[response.status_code])
         return None
 
+
 def get_object_id(iau_name, verbose=False):
     """Obtains the objects's Wiserep ID.
-    
+
     Parameters
     ----------
     iau_name: str
         IAU name of the target (e.g. 2020xne).
     verbose: bool, default 'False'
         If True, print some of the intermediate information
-        
+
     Returns
     -------
     obj_id: str
         The object's Wiserep ID. Returns 'Unknown' if not found
         or None if there is a problem of some other kind.
-    """ 
+    """
     # look for the target ID in the search webpage
-    wiserep_search_url = 'https://www.wiserep.org/search?name='
+    wiserep_search_url = "https://www.wiserep.org/search?name="
     target_search_url = wiserep_search_url + iau_name
     response = get_response(target_search_url)
     if response is None:
         return None
 
     split_text = response.text.split('href="/object/')
     if len(split_text) < 2:
-        print(f'No target with this name found on Wiserep: {iau_name}')
-        return 'Unknown'
+        print(f"No target with this name found on Wiserep: {iau_name}")
+        return "Unknown"
     else:
         obj_id = None  # return None if object ID is not found
         for line in split_text:
             # check only the lines at the bottom of the search page
             if "Click to Object page" in line:
-                if (f'{iau_name}</a>' in line) or (f'{iau_name}, ' in line):
+                if (f"{iau_name}</a>" in line) or (f"{iau_name}, " in line):
                     obj_id = line.split('"')[0]
         if verbose:
-            print('Object ID (Wiserep):', obj_id)
-            
+            print("Object ID (Wiserep):", obj_id)
+
         if obj_id is None:
-            print(f'No target with this name found on Wiserep: {iau_name}')
+            print(f"No target with this name found on Wiserep: {iau_name}")
 
-        return obj_id
+        return obj_id
```

### Comparing `wiserep_api-0.1.0/wiserep_api/classification.py` & `wiserep_api-0.1.1/wiserep_api/classification.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 from wiserep_api.api import get_response, get_object_id
 
+
 def get_target_class(iau_name, verbose=False):
     """Obtains the target's classification (type) from Wiserep.
-    
+
     Parameters
     ----------
     iau_name: str
         IAU name of the target (e.g. 2020xne).
     verbose: bool, default 'False'
         If True, print some of the intermediate information
-        
+
     Returns
     -------
     target_class: str
         The target's classification. Returns 'Unknown' if not found.
-    """    
+    """
     # look for the target ID in the search webpage
     obj_id = get_object_id(iau_name, verbose)
-    if (obj_id is None) or (obj_id=='Unknown'):
+    if (obj_id is None) or (obj_id == "Unknown"):
         return obj_id
 
     # target's webpage
-    target_url = f'https://www.wiserep.org/object/{obj_id}'
+    target_url = f"https://www.wiserep.org/object/{obj_id}"
     response = get_response(target_url)
     if response is None:
         return None
-    
+
     # search for classification
     split_text = response.text.split('Type</span><div class="value"><b>')
-    if len(split_text)>1:
+    if len(split_text) > 1:
         # look for classification under "Type" parameter
-        target_class = split_text[1].split('<')[0]
-        if target_class!='SN':
+        target_class = split_text[1].split("<")[0]
+        if target_class != "SN":
             return target_class
 
     # look for classifications in TNS reports at the bottom of the webpage
-    table = response.text.split('\n <thead><tr>')[-1]
+    table = response.text.split("\n <thead><tr>")[-1]
     simply_a_SN = False
     for row in table.split('<td class="cell-objtype_name">'):
-        target_class = row.split('<')[0]
-        if len(target_class)>0 and target_class!='SN':
+        target_class = row.split("<")[0]
+        if len(target_class) > 0 and target_class != "SN":
             return target_class
-        
-        if target_class=='SN':
+
+        if target_class == "SN":
             simply_a_SN = True
 
     if simply_a_SN is True:
         # Some objects just have the classification as "SN"
-        return 'SN'
+        return "SN"
     else:
-        print(f'Target classification not found: {iau_name}')
-        return 'Unknown'
+        print(f"Target classification not found: {iau_name}")
+        return "Unknown"
```

### Comparing `wiserep_api-0.1.0/wiserep_api/spectra.py` & `wiserep_api-0.1.1/wiserep_api/spectra.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import os
 import pandas as pd
 from astropy.io import fits
 from wiserep_api.api import get_response, get_object_id
 
+
 def exclude_include(url, exclude=None, include=None):
     """Either includes or excludes the given URL according to the
     given patterns.
 
-    Note: only one of the parameters ('exclude' or 'include') can be 
+    Note: only one of the parameters ('exclude' or 'include') can be
     given at a time, not both
 
     Parameters
     ----------
     url : str
         URL string.
     exclude : list, optional
@@ -27,151 +28,156 @@
     err_msg = "'exclude' and 'include' cannot be given at the same time!"
     assert exclude is None or include is None, err_msg
 
     if exclude is not None:
         skip = False
         for pattern in exclude:
             if pattern in url:
-                skip = True 
+                skip = True
 
     if include is not None:
         skip = True
         for pattern in include:
             if pattern in url:
                 skip = False
 
     if exclude is None and include is None:
         skip = False
 
     return skip
 
 
-def download_target_spectra(iau_name, file_type=None, exclude=None, 
-                            include=None, verbose=False):
+def download_target_spectra(
+    iau_name, file_type=None, exclude=None, include=None, verbose=False
+):
     """Downloads the target's spectra from Wiserep.
-    
+
     Parameters
     ----------
     iau_name: str
         IAU name of the target (e.g. 2020xne).
     file_type: str
         File format: either 'ascii' or 'fits'. By default,
         both formats are downloaded.
     exclude: list, default 'None'
         Files with the given string patterns are excluded.
         Cannot be given together with 'include'.
     include: list, default 'None'
-        Files with the given string patterns are inxcluded. 
+        Files with the given string patterns are inxcluded.
         Cannot be given together with 'exclude'.
     verbose: bool, default 'False'
         If True, print some of the extra information
-        
+
     Returns
     -------
     target_class: str
         The target's classification. Returns 'Unknown' if not found.
-    """    
-    if os.path.isdir('spectra') is False:
-        os.mkdir('spectra')
-    
-    assert file_type in [None, 'ascii', 'fits'], "not a valide file type"
-    
+    """
+    if os.path.isdir("spectra") is False:
+        os.mkdir("spectra")
+
+    assert file_type in [None, "ascii", "fits"], "not a valide file type"
+
     # look for the target ID in the search webpage
     obj_id = get_object_id(iau_name, verbose)
-    if (obj_id is None) or (obj_id=='Unknown'):
+    if (obj_id is None) or (obj_id == "Unknown"):
         return obj_id
 
     # target's webpage
-    target_url = f'https://www.wiserep.org/object/{obj_id}'
+    target_url = f"https://www.wiserep.org/object/{obj_id}"
     response = get_response(target_url)
     if response is None:
         return None
-    
+
     # search for spectra URLs
     # ASCII
     txt_urls = []
-    split_text = response.text.split('asciifile=https%3A//')
+    split_text = response.text.split("asciifile=https%3A//")
     for st in split_text:
         url = st.split('"')[0]
-        if (url not in txt_urls) and ('&amp' not in url) and ('DOCTYPE' not in url):
+        if (url not in txt_urls) and ("&amp" not in url) and ("DOCTYPE" not in url):
             txt_urls.append(url)
     if verbose is True:
-        print(f'Found {len(txt_urls)} URLs with spectra (ASCII): {txt_urls}')
-         
+        print(f"Found {len(txt_urls)} URLs with spectra (ASCII): {txt_urls}")
+
     # FITS
     fits_urls = []
-    split_text = response.text.split('https://')
+    split_text = response.text.split("https://")
     for st in split_text:
         url = st.split('"')[0]
-        if (url not in fits_urls) and ('.fits' in url) and ('rel-file' not in url):
-            fits_urls.append(url)        
+        if (url not in fits_urls) and (".fits" in url) and ("rel-file" not in url):
+            fits_urls.append(url)
     if verbose is True:
-        print(f'Found {len(fits_urls)} URLs with spectra (FITS): {fits_urls}')
-    
+        print(f"Found {len(fits_urls)} URLs with spectra (FITS): {fits_urls}")
+
     # download ASCII spectra
-    if file_type == 'ascii' or file_type is None:
+    if file_type == "ascii" or file_type is None:
         for url in txt_urls:
-            # skip files 
+            # skip files
             skip = exclude_include(url, exclude, include)
             if skip is True:
                 if verbose is True:
-                    print(f'Skipping {url}')
+                    print(f"Skipping {url}")
                 continue
 
             # check url
-            response = get_response('http://' + url)
+            response = get_response("http://" + url)
             if response is None:
-                print(f'Nothing found in {url}')
+                print(f"Nothing found in {url}")
 
             # get spectrum
             basename = os.path.basename(url)
-            obj_dir = os.path.join('spectra', iau_name)
+            obj_dir = os.path.join("spectra", iau_name)
             if os.path.isdir(obj_dir) is False:
                 os.mkdir(obj_dir)
             outfile = os.path.join(obj_dir, basename)
-            
-            with open(outfile, 'w') as file:
+
+            with open(outfile, "w") as file:
                 file.write(response.text)
-            
-            if response.text.startswith('BITPIX') or response.text.startswith('SIMPLE'):
+
+            if response.text.startswith("BITPIX") or response.text.startswith("SIMPLE"):
                 # file includes header
-                for i, line in enumerate(response.text.split('\n')):
+                for i, line in enumerate(response.text.split("\n")):
                     split_line = line.split()
                     try:
                         _ = float(split_line[0])
                         _ = float(split_line[1])
                         skiprows = i
                         break
                     except:
                         continue
             else:
                 skiprows = None
-            spec_df = pd.read_csv(outfile, delim_whitespace=True, 
-                                  names=['wave', 'flux', 'flux_err'],
-                                  comment='#', skiprows=skiprows)
+            spec_df = pd.read_csv(
+                outfile,
+                delim_whitespace=True,
+                names=["wave", "flux", "flux_err"],
+                comment="#",
+                skiprows=skiprows,
+            )
             spec_df.to_csv(outfile, index=False)
-        
+
     # download FITS spectra
-    if file_type == 'fits' or file_type is None:
+    if file_type == "fits" or file_type is None:
         for url in fits_urls:
-            # skip files 
+            # skip files
             skip = exclude_include(url, exclude, include)
             if skip is True:
                 if verbose is True:
-                    print(f'Skipping {url}')
+                    print(f"Skipping {url}")
                 continue
 
-            # download file    
-            print(url)   
-            hdu = fits.open('http://' + url)
+            # download file
+            print(url)
+            hdu = fits.open("http://" + url)
 
             basename = os.path.basename(url)
-            obj_dir = os.path.join('spectra', iau_name)
+            obj_dir = os.path.join("spectra", iau_name)
             if os.path.isdir(obj_dir) is False:
                 os.mkdir(obj_dir)
             outfile = os.path.join(obj_dir, basename)
             if os.path.isfile(outfile) is True:
                 overwrite = True
             else:
                 overwrite = False
-                
-            hdu.writeto(outfile, overwrite=overwrite, output_verify='ignore')
+
+            hdu.writeto(outfile, overwrite=overwrite, output_verify="ignore")
```

