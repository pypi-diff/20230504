# Comparing `tmp/shortzy-0.0.6.tar.gz` & `tmp/shortzy-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shortzy-0.0.6.tar", last modified: Wed May  3 20:47:23 2023, max compression
+gzip compressed data, was "shortzy-0.0.7.tar", last modified: Thu May  4 17:39:23 2023, max compression
```

## Comparing `shortzy-0.0.6.tar` & `shortzy-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwx------   0 kevinnadar   (501) staff       (20)        0 2023-05-03 20:47:23.480000 shortzy-0.0.6/
--rwx------   0 kevinnadar   (501) staff       (20)    34523 2023-05-03 20:47:23.580000 shortzy-0.0.6/LICENSE
--rwx------   0 kevinnadar   (501) staff       (20)     6152 2023-05-03 20:47:23.910000 shortzy-0.0.6/PKG-INFO
--rwx------   0 kevinnadar   (501) staff       (20)     5442 2023-05-03 20:47:23.590000 shortzy-0.0.6/README.md
--rwx------   0 kevinnadar   (501) staff       (20)       38 2023-05-03 20:47:23.910000 shortzy-0.0.6/setup.cfg
--rwx------   0 kevinnadar   (501) staff       (20)     1146 2023-05-03 20:47:23.640000 shortzy-0.0.6/setup.py
-drwx------   0 kevinnadar   (501) staff       (20)        0 2023-05-03 20:47:23.510000 shortzy-0.0.6/shortzy/
--rwx------   0 kevinnadar   (501) staff       (20)       25 2023-05-03 20:47:23.700000 shortzy-0.0.6/shortzy/__init__.py
--rwx------   0 kevinnadar   (501) staff       (20)     5227 2023-05-03 20:47:23.720000 shortzy-0.0.6/shortzy/adlinkfly.py
--rwx------   0 kevinnadar   (501) staff       (20)     4552 2023-05-03 20:47:23.760000 shortzy-0.0.6/shortzy/main.py
--rwx------   0 kevinnadar   (501) staff       (20)     5105 2023-05-03 20:47:23.800000 shortzy-0.0.6/shortzy/shareus.py
-drwx------   0 kevinnadar   (501) staff       (20)        0 2023-05-03 20:47:23.520000 shortzy-0.0.6/shortzy.egg-info/
--rwx------   0 kevinnadar   (501) staff       (20)     6152 2023-05-03 20:47:23.800000 shortzy-0.0.6/shortzy.egg-info/PKG-INFO
--rwx------   0 kevinnadar   (501) staff       (20)      256 2023-05-03 20:47:23.800000 shortzy-0.0.6/shortzy.egg-info/SOURCES.txt
--rwx------   0 kevinnadar   (501) staff       (20)        1 2023-05-03 20:47:23.810000 shortzy-0.0.6/shortzy.egg-info/dependency_links.txt
--rwx------   0 kevinnadar   (501) staff       (20)        8 2023-05-03 20:47:23.810000 shortzy-0.0.6/shortzy.egg-info/requires.txt
--rwx------   0 kevinnadar   (501) staff       (20)        8 2023-05-03 20:47:23.810000 shortzy-0.0.6/shortzy.egg-info/top_level.txt
+drwx------   0 kevinnadar   (501) staff       (20)        0 2023-05-04 17:39:22.980000 shortzy-0.0.7/
+-rwx------   0 kevinnadar   (501) staff       (20)    34523 2023-05-04 17:39:23.010000 shortzy-0.0.7/LICENSE
+-rwx------   0 kevinnadar   (501) staff       (20)     6152 2023-05-04 17:39:23.140000 shortzy-0.0.7/PKG-INFO
+-rwx------   0 kevinnadar   (501) staff       (20)     5442 2023-05-04 17:39:23.030000 shortzy-0.0.7/README.md
+-rwx------   0 kevinnadar   (501) staff       (20)       38 2023-05-04 17:39:23.140000 shortzy-0.0.7/setup.cfg
+-rwx------   0 kevinnadar   (501) staff       (20)     1146 2023-05-04 17:39:23.040000 shortzy-0.0.7/setup.py
+drwx------   0 kevinnadar   (501) staff       (20)        0 2023-05-04 17:39:22.980000 shortzy-0.0.7/shortzy/
+-rwx------   0 kevinnadar   (501) staff       (20)       25 2023-05-04 17:39:23.080000 shortzy-0.0.7/shortzy/__init__.py
+-rwx------   0 kevinnadar   (501) staff       (20)     5227 2023-05-04 17:39:23.100000 shortzy-0.0.7/shortzy/adlinkfly.py
+-rwx------   0 kevinnadar   (501) staff       (20)     4594 2023-05-04 17:39:23.100000 shortzy-0.0.7/shortzy/main.py
+-rwx------   0 kevinnadar   (501) staff       (20)     5105 2023-05-04 17:39:23.110000 shortzy-0.0.7/shortzy/shareus.py
+drwx------   0 kevinnadar   (501) staff       (20)        0 2023-05-04 17:39:22.980000 shortzy-0.0.7/shortzy.egg-info/
+-rwx------   0 kevinnadar   (501) staff       (20)     6152 2023-05-04 17:39:23.110000 shortzy-0.0.7/shortzy.egg-info/PKG-INFO
+-rwx------   0 kevinnadar   (501) staff       (20)      256 2023-05-04 17:39:23.110000 shortzy-0.0.7/shortzy.egg-info/SOURCES.txt
+-rwx------   0 kevinnadar   (501) staff       (20)        1 2023-05-04 17:39:23.110000 shortzy-0.0.7/shortzy.egg-info/dependency_links.txt
+-rwx------   0 kevinnadar   (501) staff       (20)        8 2023-05-04 17:39:23.110000 shortzy-0.0.7/shortzy.egg-info/requires.txt
+-rwx------   0 kevinnadar   (501) staff       (20)        8 2023-05-04 17:39:23.140000 shortzy-0.0.7/shortzy.egg-info/top_level.txt
```

### Comparing `shortzy-0.0.6/LICENSE` & `shortzy-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `shortzy-0.0.6/PKG-INFO` & `shortzy-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shortzy
-Version: 0.0.6
+Version: 0.0.7
 Summary: An Unofficial Asynchronous Python version of Adlinkfly and Alternative Website API wrapper
 Home-page: https://github.com/kevinnadar22/shortzy
 Author: Kevin Nadar
 Author-email: jesikamaraj@gmail.com
 License: MIT
 Keywords: python,droplink,gplink,url-shortener,earn money,shareus,adlinkfly
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: shortzy Version: 0.0.6 Summary: An Unofficial
+Metadata-Version: 2.1 Name: shortzy Version: 0.0.7 Summary: An Unofficial
 Asynchronous Python version of Adlinkfly and Alternative Website API wrapper
 Home-page: https://github.com/kevinnadar22/shortzy Author: Kevin Nadar Author-
 email: jesikamaraj@gmail.com License: MIT Keywords: python,droplink,gplink,url-
 shortener,earn money,shareus,adlinkfly Platform: UNKNOWN Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
 Unix Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating
```

### Comparing `shortzy-0.0.6/README.md` & `shortzy-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `shortzy-0.0.6/setup.py` & `shortzy-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'An Unofficial Asynchronous Python version of Adlinkfly and Alternative Website API wrapper'
 
 # Setting up
 setup(
     name="shortzy",
     version=VERSION,
     author="Kevin Nadar",
```

### Comparing `shortzy-0.0.6/shortzy/adlinkfly.py` & `shortzy-0.0.7/shortzy/adlinkfly.py`

 * *Files identical despite different names*

### Comparing `shortzy-0.0.6/shortzy/main.py` & `shortzy-0.0.7/shortzy/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,17 +16,17 @@
         self.api_key = api_key
         self.base_site = base_site
 
         if not self.api_key:
             raise Exception("API key not provided")
 
         if self.base_site == "shareus.in":
-            self.shortener = Shareus(api_key)
+            self.shortener = Shareus(api_key, base_site=base_site)
         else:
-            self.shortener = Adlinkfly(api_key)
+            self.shortener = Adlinkfly(api_key, base_site=base_site)
 
     async def convert(
         self, link: str, silently_fail: bool = False, quick_link: bool = False, alias: str = "", ** kwargs
     ) -> str:
         """
         It converts a link to a short link.
```

### Comparing `shortzy-0.0.6/shortzy/shareus.py` & `shortzy-0.0.7/shortzy/shareus.py`

 * *Files identical despite different names*

### Comparing `shortzy-0.0.6/shortzy.egg-info/PKG-INFO` & `shortzy-0.0.7/shortzy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shortzy
-Version: 0.0.6
+Version: 0.0.7
 Summary: An Unofficial Asynchronous Python version of Adlinkfly and Alternative Website API wrapper
 Home-page: https://github.com/kevinnadar22/shortzy
 Author: Kevin Nadar
 Author-email: jesikamaraj@gmail.com
 License: MIT
 Keywords: python,droplink,gplink,url-shortener,earn money,shareus,adlinkfly
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: shortzy Version: 0.0.6 Summary: An Unofficial
+Metadata-Version: 2.1 Name: shortzy Version: 0.0.7 Summary: An Unofficial
 Asynchronous Python version of Adlinkfly and Alternative Website API wrapper
 Home-page: https://github.com/kevinnadar22/shortzy Author: Kevin Nadar Author-
 email: jesikamaraj@gmail.com License: MIT Keywords: python,droplink,gplink,url-
 shortener,earn money,shareus,adlinkfly Platform: UNKNOWN Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
 Unix Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating
```

