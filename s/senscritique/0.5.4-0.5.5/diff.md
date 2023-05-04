# Comparing `tmp/senscritique-0.5.4.tar.gz` & `tmp/senscritique-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "senscritique-0.5.4.tar", last modified: Wed May  3 22:44:11 2023, max compression
+gzip compressed data, was "senscritique-0.5.5.tar", last modified: Thu May  4 10:23:04 2023, max compression
```

## Comparing `senscritique-0.5.4.tar` & `senscritique-0.5.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:44:11.059105 senscritique-0.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-03 22:43:57.000000 senscritique-0.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-05-03 22:44:11.059105 senscritique-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-03 22:43:57.000000 senscritique-0.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:44:11.059105 senscritique-0.5.4/senscritique/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-03 22:43:57.000000 senscritique-0.5.4/senscritique/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-03 22:43:57.000000 senscritique-0.5.4/senscritique/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-03 22:43:57.000000 senscritique-0.5.4/senscritique/parse_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-03 22:43:57.000000 senscritique-0.5.4/senscritique/process_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-05-03 22:43:57.000000 senscritique-0.5.4/senscritique/process_critiques.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-05-03 22:43:57.000000 senscritique-0.5.4/senscritique/process_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-05-03 22:43:57.000000 senscritique-0.5.4/senscritique/process_listes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-03 22:43:57.000000 senscritique-0.5.4/senscritique/takeout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:44:11.059105 senscritique-0.5.4/senscritique/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 22:43:57.000000 senscritique-0.5.4/senscritique/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-03 22:43:57.000000 senscritique-0.5.4/senscritique/tests/test_senscritique.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-03 22:43:57.000000 senscritique-0.5.4/senscritique/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:44:11.059105 senscritique-0.5.4/senscritique.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-05-03 22:44:10.000000 senscritique-0.5.4/senscritique.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-03 22:44:11.000000 senscritique-0.5.4/senscritique.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 22:44:10.000000 senscritique-0.5.4/senscritique.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-03 22:44:10.000000 senscritique-0.5.4/senscritique.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-03 22:44:10.000000 senscritique-0.5.4/senscritique.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-03 22:44:11.059105 senscritique-0.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-03 22:43:57.000000 senscritique-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:23:04.532029 senscritique-0.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-04 10:22:51.000000 senscritique-0.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-05-04 10:23:04.532029 senscritique-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-04 10:22:51.000000 senscritique-0.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:23:04.528028 senscritique-0.5.5/senscritique/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-04 10:22:51.000000 senscritique-0.5.5/senscritique/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-04 10:22:51.000000 senscritique-0.5.5/senscritique/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-04 10:22:51.000000 senscritique-0.5.5/senscritique/parse_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-05-04 10:22:51.000000 senscritique-0.5.5/senscritique/process_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-05-04 10:22:51.000000 senscritique-0.5.5/senscritique/process_critiques.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-05-04 10:22:51.000000 senscritique-0.5.5/senscritique/process_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-05-04 10:22:51.000000 senscritique-0.5.5/senscritique/process_listes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-04 10:22:51.000000 senscritique-0.5.5/senscritique/takeout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:23:04.532029 senscritique-0.5.5/senscritique/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:22:51.000000 senscritique-0.5.5/senscritique/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-04 10:22:51.000000 senscritique-0.5.5/senscritique/tests/test_senscritique.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-04 10:22:51.000000 senscritique-0.5.5/senscritique/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:23:04.528028 senscritique-0.5.5/senscritique.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-05-04 10:23:04.000000 senscritique-0.5.5/senscritique.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-04 10:23:04.000000 senscritique-0.5.5/senscritique.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 10:23:04.000000 senscritique-0.5.5/senscritique.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-04 10:23:04.000000 senscritique-0.5.5/senscritique.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-04 10:23:04.000000 senscritique-0.5.5/senscritique.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-04 10:23:04.532029 senscritique-0.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-04 10:22:51.000000 senscritique-0.5.5/setup.py
```

### Comparing `senscritique-0.5.4/LICENSE` & `senscritique-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `senscritique-0.5.4/PKG-INFO` & `senscritique-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: senscritique
-Version: 0.5.4
+Version: 0.5.5
 Summary: SensCritique Takeout on PyPI
 Home-page: https://github.com/woctezuma/SensCritique-Takeout
-Download-URL: https://github.com/woctezuma/SensCritique-Takeout/archive/0.5.4.tar.gz
+Download-URL: https://github.com/woctezuma/SensCritique-Takeout/archive/0.5.5.tar.gz
 Author: Wok
 Author-email: wok@tuta.io
 Keywords: senscritique,takeout,takeaway
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Games/Entertainment
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `senscritique-0.5.4/README.md` & `senscritique-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `senscritique-0.5.4/senscritique/parse_utils.py` & `senscritique-0.5.5/senscritique/parse_utils.py`

 * *Files identical despite different names*

### Comparing `senscritique-0.5.4/senscritique/process_collection.py` & `senscritique-0.5.5/senscritique/process_collection.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,16 +23,15 @@
 
     data = {}
     for item in collection_items:
         user_rating = item.find_all('div', {'class': 'elco-collection-rating user'})
         item_type_p = item.find('div', {'class': re.compile("^d-media-[a-z]+$")})
         item_type = "unknown"
         if item_type_p:
-            if 'data-sc-play-type' in item_type_p:
-                item_type = item_type_p['data-sc-play-type']
+            item_type = item_type_p.get('data-sc-play-type') or "unknown"
         name = item.find_all('a', {'class': 'elco-anchor'})
         game_system = item.find_all('span', {'class': 'elco-gamesystem'})
         release_date = item.find_all('span', {'class': 'elco-date'})
         description = item.find_all('p', {'class': 'elco-baseline elco-options'})
         author = item.find_all('a', {'class': 'elco-baseline-a'})
         site_rating = item.find_all('a', {'class': 'erra-global'})
```

### Comparing `senscritique-0.5.4/senscritique/process_critiques.py` & `senscritique-0.5.5/senscritique/process_critiques.py`

 * *Files identical despite different names*

### Comparing `senscritique-0.5.4/senscritique/process_generic.py` & `senscritique-0.5.5/senscritique/process_generic.py`

 * *Files identical despite different names*

### Comparing `senscritique-0.5.4/senscritique/process_listes.py` & `senscritique-0.5.5/senscritique/process_listes.py`

 * *Files identical despite different names*

### Comparing `senscritique-0.5.4/senscritique/takeout.py` & `senscritique-0.5.5/senscritique/takeout.py`

 * *Files identical despite different names*

### Comparing `senscritique-0.5.4/senscritique/tests/test_senscritique.py` & `senscritique-0.5.5/senscritique/tests/test_senscritique.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,14 +34,26 @@
             user_name=self.test_get_user_example(),
             data_type='collection',
             verbose=True,
         )
         senscritique.print_data(data)
         self.assertEqual(len(data), 6)
 
+    def test_presence_of_different_item_types(self):
+        data = senscritique.parse(
+            user_name=self.test_get_user_example(),
+            data_type='collection',
+            verbose=True,
+        )
+        all_types = {element['item_type'] for element in data.values()}
+        senscritique.print_data(all_types)
+        self.assertIn('unknown', all_types)
+        self.assertIn('videos', all_types)
+        self.assertEqual(len(all_types), 2)
+
     def test_parse_critiques(self):
         data = senscritique.parse(
             user_name='MrMez',
             data_type='critiques',
             verbose=True,
         )
         senscritique.print_data(data)
```

### Comparing `senscritique-0.5.4/senscritique/utils.py` & `senscritique-0.5.5/senscritique/utils.py`

 * *Files identical despite different names*

### Comparing `senscritique-0.5.4/senscritique.egg-info/PKG-INFO` & `senscritique-0.5.5/senscritique.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: senscritique
-Version: 0.5.4
+Version: 0.5.5
 Summary: SensCritique Takeout on PyPI
 Home-page: https://github.com/woctezuma/SensCritique-Takeout
-Download-URL: https://github.com/woctezuma/SensCritique-Takeout/archive/0.5.4.tar.gz
+Download-URL: https://github.com/woctezuma/SensCritique-Takeout/archive/0.5.5.tar.gz
 Author: Wok
 Author-email: wok@tuta.io
 Keywords: senscritique,takeout,takeaway
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Games/Entertainment
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `senscritique-0.5.4/senscritique.egg-info/SOURCES.txt` & `senscritique-0.5.5/senscritique.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `senscritique-0.5.4/setup.py` & `senscritique-0.5.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='senscritique',
-    version='0.5.4',
+    version='0.5.5',
     author='Wok',
     author_email='wok@tuta.io',
     description='SensCritique Takeout on PyPI',
     keywords=['senscritique', 'takeout', 'takeaway'],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/woctezuma/SensCritique-Takeout',
-    download_url='https://github.com/woctezuma/SensCritique-Takeout/archive/0.5.4.tar.gz',
+    download_url='https://github.com/woctezuma/SensCritique-Takeout/archive/0.5.5.tar.gz',
     packages=setuptools.find_packages(),
     install_requires=[
         'beautifulsoup4',
         'requests',
         'lxml',
     ],
     test_suite='nose.collector',
```

