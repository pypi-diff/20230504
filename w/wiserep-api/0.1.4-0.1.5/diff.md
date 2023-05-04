# Comparing `tmp/wiserep_api-0.1.4.tar.gz` & `tmp/wiserep_api-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiserep_api-0.1.4.tar", last modified: Thu May  4 08:11:59 2023, max compression
+gzip compressed data, was "wiserep_api-0.1.5.tar", last modified: Thu May  4 13:30:27 2023, max compression
```

## Comparing `wiserep_api-0.1.4.tar` & `wiserep_api-0.1.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-04 08:11:59.140195 wiserep_api-0.1.4/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1080 2023-05-02 06:17:37.000000 wiserep_api-0.1.4/LICENSE
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       51 2023-05-04 05:31:12.000000 wiserep_api-0.1.4/MANIFEST.in
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4129 2023-05-04 08:11:59.140195 wiserep_api-0.1.4/PKG-INFO
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3641 2023-05-04 05:27:21.000000 wiserep_api-0.1.4/README.md
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       30 2023-05-02 08:10:24.000000 wiserep_api-0.1.4/requirements.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       38 2023-05-04 08:11:59.140195 wiserep_api-0.1.4/setup.cfg
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1134 2023-05-04 05:33:37.000000 wiserep_api-0.1.4/setup.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-04 08:11:59.136195 wiserep_api-0.1.4/tests/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)        0 2022-06-28 14:16:32.000000 wiserep_api-0.1.4/tests/__init__.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      309 2023-05-04 03:16:44.000000 wiserep_api-0.1.4/tests/test_classification.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2326 2023-05-04 07:16:40.000000 wiserep_api-0.1.4/tests/test_download_spectra.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      475 2023-05-04 07:25:36.000000 wiserep_api-0.1.4/tests/test_search.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-04 08:11:59.136195 wiserep_api-0.1.4/wiserep_api/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      266 2023-05-04 03:01:55.000000 wiserep_api-0.1.4/wiserep_api/__init__.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       46 2023-05-04 08:09:33.000000 wiserep_api-0.1.4/wiserep_api/_version.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2844 2023-05-04 07:21:49.000000 wiserep_api-0.1.4/wiserep_api/api.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1749 2023-05-03 06:34:19.000000 wiserep_api-0.1.4/wiserep_api/classification.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3433 2023-05-04 03:46:52.000000 wiserep_api-0.1.4/wiserep_api/search.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3427 2023-05-04 08:07:12.000000 wiserep_api-0.1.4/wiserep_api/snid.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5790 2023-05-04 07:19:34.000000 wiserep_api-0.1.4/wiserep_api/spectra.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-04 08:11:59.140195 wiserep_api-0.1.4/wiserep_api/static/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      744 2023-05-04 01:46:48.000000 wiserep_api-0.1.4/wiserep_api/static/spectral_types.json
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-04 08:11:59.140195 wiserep_api-0.1.4/wiserep_api.egg-info/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4129 2023-05-04 08:11:59.000000 wiserep_api-0.1.4/wiserep_api.egg-info/PKG-INFO
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      529 2023-05-04 08:11:59.000000 wiserep_api-0.1.4/wiserep_api.egg-info/SOURCES.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)        1 2023-05-04 08:11:59.000000 wiserep_api-0.1.4/wiserep_api.egg-info/dependency_links.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       30 2023-05-04 08:11:59.000000 wiserep_api-0.1.4/wiserep_api.egg-info/requires.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       18 2023-05-04 08:11:59.000000 wiserep_api-0.1.4/wiserep_api.egg-info/top_level.txt
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-04 13:30:27.746963 wiserep_api-0.1.5/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1080 2023-05-02 06:17:37.000000 wiserep_api-0.1.5/LICENSE
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       51 2023-05-04 05:31:12.000000 wiserep_api-0.1.5/MANIFEST.in
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4129 2023-05-04 13:30:27.746963 wiserep_api-0.1.5/PKG-INFO
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3641 2023-05-04 05:27:21.000000 wiserep_api-0.1.5/README.md
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       30 2023-05-02 08:10:24.000000 wiserep_api-0.1.5/requirements.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       38 2023-05-04 13:30:27.746963 wiserep_api-0.1.5/setup.cfg
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1134 2023-05-04 05:33:37.000000 wiserep_api-0.1.5/setup.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-04 13:30:27.746963 wiserep_api-0.1.5/tests/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)        0 2022-06-28 14:16:32.000000 wiserep_api-0.1.5/tests/__init__.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2326 2023-05-04 07:16:40.000000 wiserep_api-0.1.5/tests/test_download_spectra.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      893 2023-05-04 12:28:16.000000 wiserep_api-0.1.5/tests/test_properties.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      475 2023-05-04 07:25:36.000000 wiserep_api-0.1.5/tests/test_search.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-04 13:30:27.746963 wiserep_api-0.1.5/wiserep_api/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      283 2023-05-04 12:23:09.000000 wiserep_api-0.1.5/wiserep_api/__init__.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       46 2023-05-04 13:30:00.000000 wiserep_api-0.1.5/wiserep_api/_version.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2844 2023-05-04 07:21:49.000000 wiserep_api-0.1.5/wiserep_api/api.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3748 2023-05-04 12:32:22.000000 wiserep_api-0.1.5/wiserep_api/properties.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3433 2023-05-04 03:46:52.000000 wiserep_api-0.1.5/wiserep_api/search.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3427 2023-05-04 08:34:32.000000 wiserep_api-0.1.5/wiserep_api/snid.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5790 2023-05-04 07:19:34.000000 wiserep_api-0.1.5/wiserep_api/spectra.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-04 13:30:27.746963 wiserep_api-0.1.5/wiserep_api/static/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      744 2023-05-04 01:46:48.000000 wiserep_api-0.1.5/wiserep_api/static/spectral_types.json
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-04 13:30:27.746963 wiserep_api-0.1.5/wiserep_api.egg-info/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4129 2023-05-04 13:30:27.000000 wiserep_api-0.1.5/wiserep_api.egg-info/PKG-INFO
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      521 2023-05-04 13:30:27.000000 wiserep_api-0.1.5/wiserep_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)        1 2023-05-04 13:30:27.000000 wiserep_api-0.1.5/wiserep_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       30 2023-05-04 13:30:27.000000 wiserep_api-0.1.5/wiserep_api.egg-info/requires.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       18 2023-05-04 13:30:27.000000 wiserep_api-0.1.5/wiserep_api.egg-info/top_level.txt
```

### Comparing `wiserep_api-0.1.4/LICENSE` & `wiserep_api-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wiserep_api-0.1.4/PKG-INFO` & `wiserep_api-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiserep_api
-Version: 0.1.4
+Version: 0.1.5
 Summary: API to access WiserRep data from command lines
 Home-page: https://github.com/temuller/wiserep_api
 Author: Tomás Enrique Müller-Bravo
 Author-email: t.e.muller-bravo@ice.csic.es
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `wiserep_api-0.1.4/README.md` & `wiserep_api-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `wiserep_api-0.1.4/setup.py` & `wiserep_api-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `wiserep_api-0.1.4/tests/test_download_spectra.py` & `wiserep_api-0.1.5/tests/test_download_spectra.py`

 * *Files identical despite different names*

### Comparing `wiserep_api-0.1.4/wiserep_api/api.py` & `wiserep_api-0.1.5/wiserep_api/api.py`

 * *Files identical despite different names*

### Comparing `wiserep_api-0.1.4/wiserep_api/classification.py` & `wiserep_api-0.1.5/wiserep_api/properties.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,68 @@
 from wiserep_api.api import get_response, get_object_id
 
+def get_target_property(iau_name, property_name, verbose=False):
+    """Obtains the target's property from Wiserep.
+
+    Properties: ``type``, ``redshift``, ``host``, ``coords``
+    and ``coords_deg``.
+
+    Parameters
+    ----------
+    iau_name: str
+        IAU name of the target (e.g. 2020xne).
+    property_name : str
+        Name of the target's property.
+    verbose: bool, default 'False'
+        If True, print some of the intermediate information
+
+    Returns
+    -------
+    target_property: str or float
+        The value of the target's property.
+    """
+    # look for the target ID in the search webpage
+    obj_id = get_object_id(iau_name, verbose)
+    if obj_id is None:
+        return None
+
+    # target's webpage
+    target_url = f"https://www.wiserep.org/object/{obj_id}"
+    response = get_response(target_url)
+    if response is None:
+        return None
+
+    properties_dict = {'type':'Type',
+                       'redshift':'Redshift',
+                       'host':'Host Name',
+                       'coords':'RA/DEC (J2000)',
+                       'coords_deg':'RA/DEC (J2000)',
+                       } 
+    assert property_name in properties_dict.keys(), "Not a valid property name!"
+    prop_str = properties_dict[property_name]
+
+    # search for the property
+    if property_name=='coords':
+        split_text = response.text.split(f'{prop_str}</span><b><div class="value">')
+    elif property_name=='coords_deg':
+        split_text = response.text.split(f'{prop_str}</span><b><div class="value">')
+        if len(split_text)>1:
+            split_text = split_text[1].split('div class="alter-value">')
+    else:
+        split_text = response.text.split(f'{prop_str}</span><div class="value"><b>')
+
+    if len(split_text) > 1:
+        target_property = split_text[1].split("<")[0]
+    else:
+        target_property = ''
+        
+    if property_name=='redshift' and len(target_property)>0:
+        target_property = float(target_property)
+
+    return target_property
 
 def get_target_class(iau_name, verbose=False):
     """Obtains the target's classification (type) from Wiserep.
 
     Parameters
     ----------
     iau_name: str
```

### Comparing `wiserep_api-0.1.4/wiserep_api/search.py` & `wiserep_api-0.1.5/wiserep_api/search.py`

 * *Files identical despite different names*

### Comparing `wiserep_api-0.1.4/wiserep_api/snid.py` & `wiserep_api-0.1.5/wiserep_api/snid.py`

 * *Files identical despite different names*

### Comparing `wiserep_api-0.1.4/wiserep_api/spectra.py` & `wiserep_api-0.1.5/wiserep_api/spectra.py`

 * *Files identical despite different names*

### Comparing `wiserep_api-0.1.4/wiserep_api/static/spectral_types.json` & `wiserep_api-0.1.5/wiserep_api/static/spectral_types.json`

 * *Files identical despite different names*

### Comparing `wiserep_api-0.1.4/wiserep_api.egg-info/PKG-INFO` & `wiserep_api-0.1.5/wiserep_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiserep-api
-Version: 0.1.4
+Version: 0.1.5
 Summary: API to access WiserRep data from command lines
 Home-page: https://github.com/temuller/wiserep_api
 Author: Tomás Enrique Müller-Bravo
 Author-email: t.e.muller-bravo@ice.csic.es
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `wiserep_api-0.1.4/wiserep_api.egg-info/SOURCES.txt` & `wiserep_api-0.1.5/wiserep_api.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 tests/__init__.py
-tests/test_classification.py
 tests/test_download_spectra.py
+tests/test_properties.py
 tests/test_search.py
 wiserep_api/__init__.py
 wiserep_api/_version.py
 wiserep_api/api.py
-wiserep_api/classification.py
+wiserep_api/properties.py
 wiserep_api/search.py
 wiserep_api/snid.py
 wiserep_api/spectra.py
 wiserep_api.egg-info/PKG-INFO
 wiserep_api.egg-info/SOURCES.txt
 wiserep_api.egg-info/dependency_links.txt
 wiserep_api.egg-info/requires.txt
```

