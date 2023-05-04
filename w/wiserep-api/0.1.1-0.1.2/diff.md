# Comparing `tmp/wiserep_api-0.1.1.tar.gz` & `tmp/wiserep_api-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiserep_api-0.1.1.tar", last modified: Thu May  4 05:24:09 2023, max compression
+gzip compressed data, was "wiserep_api-0.1.2.tar", last modified: Thu May  4 05:35:25 2023, max compression
```

## Comparing `wiserep_api-0.1.1.tar` & `wiserep_api-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-04 05:24:09.175104 wiserep_api-0.1.1/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1080 2023-05-02 06:17:37.000000 wiserep_api-0.1.1/LICENSE
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       25 2023-05-02 06:18:42.000000 wiserep_api-0.1.1/MANIFEST.in
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4106 2023-05-04 05:24:09.175104 wiserep_api-0.1.1/PKG-INFO
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3618 2023-05-04 05:21:20.000000 wiserep_api-0.1.1/README.md
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       30 2023-05-02 08:10:24.000000 wiserep_api-0.1.1/requirements.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       38 2023-05-04 05:24:09.175104 wiserep_api-0.1.1/setup.cfg
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1161 2023-05-03 06:34:19.000000 wiserep_api-0.1.1/setup.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-04 05:24:09.171104 wiserep_api-0.1.1/tests/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)        0 2022-06-28 14:16:32.000000 wiserep_api-0.1.1/tests/__init__.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      309 2023-05-04 03:16:44.000000 wiserep_api-0.1.1/tests/test_classification.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2246 2023-05-04 03:16:44.000000 wiserep_api-0.1.1/tests/test_download_spectra.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      387 2023-05-04 03:16:44.000000 wiserep_api-0.1.1/tests/test_search.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-04 05:24:09.171104 wiserep_api-0.1.1/wiserep_api/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      266 2023-05-04 03:01:55.000000 wiserep_api-0.1.1/wiserep_api/__init__.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       46 2023-05-04 05:23:20.000000 wiserep_api-0.1.1/wiserep_api/_version.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2910 2023-05-03 06:34:19.000000 wiserep_api-0.1.1/wiserep_api/api.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1749 2023-05-03 06:34:19.000000 wiserep_api-0.1.1/wiserep_api/classification.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3433 2023-05-04 03:46:52.000000 wiserep_api-0.1.1/wiserep_api/search.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2878 2023-05-04 03:16:44.000000 wiserep_api-0.1.1/wiserep_api/snid.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5782 2023-05-03 06:34:19.000000 wiserep_api-0.1.1/wiserep_api/spectra.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-04 05:24:09.175104 wiserep_api-0.1.1/wiserep_api.egg-info/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4106 2023-05-04 05:24:09.000000 wiserep_api-0.1.1/wiserep_api.egg-info/PKG-INFO
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      490 2023-05-04 05:24:09.000000 wiserep_api-0.1.1/wiserep_api.egg-info/SOURCES.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)        1 2023-05-04 05:24:09.000000 wiserep_api-0.1.1/wiserep_api.egg-info/dependency_links.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       30 2023-05-04 05:24:09.000000 wiserep_api-0.1.1/wiserep_api.egg-info/requires.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       18 2023-05-04 05:24:09.000000 wiserep_api-0.1.1/wiserep_api.egg-info/top_level.txt
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-04 05:35:25.635905 wiserep_api-0.1.2/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1080 2023-05-02 06:17:37.000000 wiserep_api-0.1.2/LICENSE
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       51 2023-05-04 05:31:12.000000 wiserep_api-0.1.2/MANIFEST.in
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4129 2023-05-04 05:35:25.635905 wiserep_api-0.1.2/PKG-INFO
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3641 2023-05-04 05:27:21.000000 wiserep_api-0.1.2/README.md
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       30 2023-05-02 08:10:24.000000 wiserep_api-0.1.2/requirements.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       38 2023-05-04 05:35:25.635905 wiserep_api-0.1.2/setup.cfg
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1134 2023-05-04 05:33:37.000000 wiserep_api-0.1.2/setup.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-04 05:35:25.631905 wiserep_api-0.1.2/tests/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)        0 2022-06-28 14:16:32.000000 wiserep_api-0.1.2/tests/__init__.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      309 2023-05-04 03:16:44.000000 wiserep_api-0.1.2/tests/test_classification.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2246 2023-05-04 03:16:44.000000 wiserep_api-0.1.2/tests/test_download_spectra.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      387 2023-05-04 03:16:44.000000 wiserep_api-0.1.2/tests/test_search.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-04 05:35:25.631905 wiserep_api-0.1.2/wiserep_api/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      266 2023-05-04 03:01:55.000000 wiserep_api-0.1.2/wiserep_api/__init__.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       46 2023-05-04 05:34:36.000000 wiserep_api-0.1.2/wiserep_api/_version.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2910 2023-05-03 06:34:19.000000 wiserep_api-0.1.2/wiserep_api/api.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1749 2023-05-03 06:34:19.000000 wiserep_api-0.1.2/wiserep_api/classification.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3433 2023-05-04 03:46:52.000000 wiserep_api-0.1.2/wiserep_api/search.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2878 2023-05-04 03:16:44.000000 wiserep_api-0.1.2/wiserep_api/snid.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5782 2023-05-03 06:34:19.000000 wiserep_api-0.1.2/wiserep_api/spectra.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-04 05:35:25.635905 wiserep_api-0.1.2/wiserep_api/static/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      744 2023-05-04 01:46:48.000000 wiserep_api-0.1.2/wiserep_api/static/spectral_types.json
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-04 05:35:25.635905 wiserep_api-0.1.2/wiserep_api.egg-info/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4129 2023-05-04 05:35:25.000000 wiserep_api-0.1.2/wiserep_api.egg-info/PKG-INFO
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      529 2023-05-04 05:35:25.000000 wiserep_api-0.1.2/wiserep_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)        1 2023-05-04 05:35:25.000000 wiserep_api-0.1.2/wiserep_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       30 2023-05-04 05:35:25.000000 wiserep_api-0.1.2/wiserep_api.egg-info/requires.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       18 2023-05-04 05:35:25.000000 wiserep_api-0.1.2/wiserep_api.egg-info/top_level.txt
```

### Comparing `wiserep_api-0.1.1/LICENSE` & `wiserep_api-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wiserep_api-0.1.1/PKG-INFO` & `wiserep_api-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: wiserep_api
-Version: 0.1.1
+Version: 0.1.2
 Summary: API to access WiserRep data from command lines
 Home-page: https://github.com/temuller/wiserep_api
 Author: Tomás Enrique Müller-Bravo
 Author-email: t.e.muller-bravo@ice.csic.es
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # WiseRep API
 API to access WiserRep data from command lines
 
 [![repo](https://img.shields.io/badge/GitHub-temuller%2Fwiserep_api-blue.svg?style=flat)](https://github.com/temuller/wiserep_api)
@@ -82,15 +82,15 @@
 from wiserep_api import snid
 
 sne_list = np.genfromtxt('SNIa-91T-like_wiserep.txt', dtype=str, delimiter='\n')
 snid_commmand = 'snid inter=0 plot=0 aband=0 usetype=Ia-91T'
 
 for sn in sne_list:
     directory = os.path.join('spectra', sn)
-    snid.run_snid(directory)
+    snid.run_snid(directory, command=snid_commmand)
 ```
 
 ### Getting the classification
 
 The spectral type of a given target can also be retrived:
 
 ```python
```

### Comparing `wiserep_api-0.1.1/README.md` & `wiserep_api-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 from wiserep_api import snid
 
 sne_list = np.genfromtxt('SNIa-91T-like_wiserep.txt', dtype=str, delimiter='\n')
 snid_commmand = 'snid inter=0 plot=0 aband=0 usetype=Ia-91T'
 
 for sn in sne_list:
     directory = os.path.join('spectra', sn)
-    snid.run_snid(directory)
+    snid.run_snid(directory, command=snid_commmand)
 ```
 
 ### Getting the classification
 
 The spectral type of a given target can also be retrived:
 
 ```python
```

### Comparing `wiserep_api-0.1.1/setup.py` & `wiserep_api-0.1.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,17 +18,17 @@
     author_email="t.e.muller-bravo@ice.csic.es",
     license="MIT",
     description="API to access WiserRep data from command lines",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/temuller/wiserep_api",
     packages=setuptools.find_packages(),
-    python_requires=">=3.8",
+    python_requires=">=3.9",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=requirements,
-    # package_data={"idsred": ["lamps/*", "standards/*", "extinction/*"]},
+    package_data={"wiserep_api": ["static/*"]},
     include_package_data=True,
 )
```

### Comparing `wiserep_api-0.1.1/tests/test_download_spectra.py` & `wiserep_api-0.1.2/tests/test_download_spectra.py`

 * *Files identical despite different names*

### Comparing `wiserep_api-0.1.1/wiserep_api/api.py` & `wiserep_api-0.1.2/wiserep_api/api.py`

 * *Files identical despite different names*

### Comparing `wiserep_api-0.1.1/wiserep_api/classification.py` & `wiserep_api-0.1.2/wiserep_api/classification.py`

 * *Files identical despite different names*

### Comparing `wiserep_api-0.1.1/wiserep_api/search.py` & `wiserep_api-0.1.2/wiserep_api/search.py`

 * *Files identical despite different names*

### Comparing `wiserep_api-0.1.1/wiserep_api/snid.py` & `wiserep_api-0.1.2/wiserep_api/snid.py`

 * *Files identical despite different names*

### Comparing `wiserep_api-0.1.1/wiserep_api/spectra.py` & `wiserep_api-0.1.2/wiserep_api/spectra.py`

 * *Files identical despite different names*

### Comparing `wiserep_api-0.1.1/wiserep_api.egg-info/PKG-INFO` & `wiserep_api-0.1.2/wiserep_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: wiserep-api
-Version: 0.1.1
+Version: 0.1.2
 Summary: API to access WiserRep data from command lines
 Home-page: https://github.com/temuller/wiserep_api
 Author: Tomás Enrique Müller-Bravo
 Author-email: t.e.muller-bravo@ice.csic.es
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # WiseRep API
 API to access WiserRep data from command lines
 
 [![repo](https://img.shields.io/badge/GitHub-temuller%2Fwiserep_api-blue.svg?style=flat)](https://github.com/temuller/wiserep_api)
@@ -82,15 +82,15 @@
 from wiserep_api import snid
 
 sne_list = np.genfromtxt('SNIa-91T-like_wiserep.txt', dtype=str, delimiter='\n')
 snid_commmand = 'snid inter=0 plot=0 aband=0 usetype=Ia-91T'
 
 for sn in sne_list:
     directory = os.path.join('spectra', sn)
-    snid.run_snid(directory)
+    snid.run_snid(directory, command=snid_commmand)
 ```
 
 ### Getting the classification
 
 The spectral type of a given target can also be retrived:
 
 ```python
```

